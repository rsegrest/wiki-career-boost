# Agent Memory Browser — Implementation Spec

## Overview

A Next.js web GUI to browse, search, edit, and visualize the Hermes agent's
persistent memory layers. Three tabs: (1) Text Memory — MEMORY.md / USER.md,
(2) Holographic Memory — fact_store.db facts with entity graph, (3) Session
Memory — browse recent sessions. All changes write back to the real files/db.

## Data Sources

1. **MEMORY.md** — `~/.hermes/memories/MEMORY.md` (durable agent notes)
2. **USER.md** — `~/.hermes/memories/USER.md` (user profile facts)
3. **memory_store.db** — `~/.hermes/memory_store.db` (holographic fact store)
   - `facts` table: fact_id, content, category, tags, trust_score, retrieval_count, helpful_count, created_at, updated_at
   - `entities` table: entity_id, name, entity_type, aliases, created_at
   - `fact_entities` junction table: fact_id → entity_id
   - `facts_fts` virtual table (FTS5): full-text search on content + tags
   - `memory_banks` table: bank_name, vector, dim, fact_count
4. **state.db** — `~/.hermes/state.db` (session history, read-only)
   - `sessions` table: id, title, source, model, started_at, ended_at, message_count, tool_call_count
   - `messages` table: id, session_id, role, content, timestamp

## Architecture

```
agent-memory-browser/
├── src/
│   ├── app/
│   │   ├── layout.tsx              # Root layout, dark theme
│   │   ├── page.tsx                # Main view with tab navigation
│   │   └── api/
│   │       ├── memory/
│   │       │   ├── route.ts        # GET/PUT MEMORY.md and USER.md
│   │       │   └── save.ts         # POST save text memory
│   │       ├── facts/
│   │       │   ├── route.ts        # GET list/search facts, POST new fact
│   │       │   ├── [id]/
│   │       │   │   └── route.ts    # GET/PUT/DELETE single fact
│   │       │   └── search.ts       # GET FTS5 search
│   │       ├── entities/
│   │       │   └── route.ts        # GET entities with fact counts
│   │       └── sessions/
│   │           └── route.ts        # GET recent sessions (read-only)
│   ├── components/
│   │   ├── TextMemoryTab.tsx       # MEMORY.md + USER.md editor
│   │   ├── FactsTab.tsx            # Fact list + detail panel
│   │   ├── FactCard.tsx            # Single fact row with trust slider
│   │   ├── FactDetail.tsx          # Expanded fact view with entity links
│   │   ├── EntityGraph.tsx         # Force-directed graph (cytoscape)
│   │   ├── EntityList.tsx          # Entity sidebar with fact counts
│   │   ├── SessionsTab.tsx         # Session list (read-only)
│   │   ├── SessionCard.tsx         # Session row with metadata
│   │   ├── SearchBar.tsx           # Unified search across all layers
│   │   └── TabNav.tsx              # Tab navigation component
│   ├── lib/
│   │   ├── db.ts                   # SQLite connection helpers
│   │   ├── types.ts                # TypeScript interfaces
│   │   └── paths.ts                # File paths (memory dir, db locations)
│   └── hooks/
│       ├── useFacts.ts             # Fact CRUD + search
│       ├── useTextMemory.ts        # MEMORY.md/USER.md load/save
│       ├── useSessions.ts          # Session list
│       └── useEntityGraph.ts      # Entity graph data
├── next.config.ts
├── tailwind.config.ts
├── package.json
└── README.md
```

## Tech Stack

- Next.js 15 (App Router, TypeScript)
- Tailwind CSS v4 + shadcn/ui (dark theme, same as local-llm-chat)
- better-sqlite3 (direct SQLite access, server-side only)
- cytoscape.js (entity relationship graph)
- lucide-react (icons)

## Key Design Decisions

1. **Read-only sessions** — Session tab is read-only. No editing messages.
2. **Write-back** — Edits to MEMORY.md/USER.md and facts DB write to the real files. No mocks.
3. **Server-side SQLite** — better-sqlite3 runs in Node.js (API routes). No client-side DB access.
4. **FTS5 search** — Use the existing facts_fts virtual table for fact search.
5. **Entity graph** — Force-directed graph showing entities and their connected facts.
6. **Trust score slider** — Visual slider (0.0-1.0) with color coding (red→yellow→green).
7. **Dark theme** — Same palette as local-llm-chat: bg #1a1a2e, text #e0e0e0, accent #00d4aa.

## Task Breakdown (12 tasks)

| # | Task | Depends On |
|---|------|------------|
| 1 | Scaffold Next.js 15 + shadcn/ui + Tailwind | — |
| 2 | SQLite db helper + types + file paths | 1 |
| 3 | Text Memory API routes (load/save MEMORY.md + USER.md) | 2 |
| 4 | Text Memory tab UI (editor with live preview) | 3 |
| 5 | Facts API routes (list, search, CRUD, trust update) | 2 |
| 6 | Facts tab UI (list + detail + trust slider + search) | 5 |
| 7 | Entities API route (list with fact counts) | 5 |
| 8 | Entity graph visualization (cytoscape force-directed) | 7 |
| 9 | Sessions API route (list recent, read-only) | 2 |
| 10 | Sessions tab UI (list + metadata display) | 9 |
| 11 | Unified search bar + tab navigation + polish | 6,8,10 |
| 12 | README + GitHub repo + deploy | 11 |
---
title: "Kanban: Nomad Cost-of-Living Dashboard"
created: 2026-05-30
type: comparison
tags: [kanban, portfolio, project-management]
---

# Kanban: Nomad Cost-of-Living Dashboard

**Goal:** Interactive dashboard comparing nomad cities on cost, wifi, safety, family-friendliness using your travel wiki data.

**Time Budget:** 1–2 weekends (8–16 hours)
**Ship Date Target:** June 5, 2026 (before cruise)

---

## Backlog

| # | Task | Est. | Priority | Notes |
|---|------|------|----------|-------|
| 1 | Export wiki city data to JSON | 30 min | P0 | Parse existing entity files |
| 2 | Scaffold Next.js project with shadcn/ui + Recharts | 30 min | P0 | `npx shadcn@latest init` + recharts |
| 3 | Design data schema for city comparisons | 1 hr | P0 | Cost, wifi, safety, family, climate |
| 4 | Build city comparison table (sortable, filterable) | 2 hr | P0 | TanStack Table or shadcn DataTable |
| 5 | Add radar/spider chart for city multi-metric view | 1.5 hr | P0 | Recharts RadarChart |
| 6 | Add cost breakdown bar chart | 1 hr | P0 | Monthly cost by category |
| 7 | Add interactive filters (region, budget, family-friendly) | 1.5 hr | P0 | Multi-select dropdowns |
| 8 | Add city detail modal/page | 1 hr | P1 | Click row → full profile |
| 9 | Add "Rick's visited" badge overlay | 30 min | P1 | Personal touch |
| 10 | Deploy to Vercel | 30 min | P0 | Git push → Vercel auto-deploy |
| 11 | Write README + add screenshots | 30 min | P1 | Show your data in action |
| 12 | Draft LinkedIn post | 30 min | P1 | "I built a dashboard from my nomad data" |

## In Progress

| # | Task | Started | Notes |
|---|------|---------|-------|
| — | — | — | — |

## Done

| # | Task | Completed | Notes |
|---|------|-----------|-------|
| — | — | — | — |

---

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Styling:** Tailwind + shadcn/ui
- **Charts:** Recharts
- **Data:** Static JSON exported from wiki
- **Deploy:** Vercel

## Blockers / Risks

- Data completeness — not all cities have full data
- Design decisions — which metrics matter most?
- Static data means manual updates when wiki changes

## Success Criteria

- [ ] Live demo with at least 15 cities
- [ ] Interactive filtering and sorting works
- [ ] 1 LinkedIn post showing the dashboard in action

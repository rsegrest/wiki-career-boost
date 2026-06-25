---
title: "Kanban: GitHub Profile README Generator"
created: 2026-05-30
updated: 2026-06-24
type: comparison
tags: [kanban, portfolio, project-management, hermes-dashboard]
---

# Kanban: GitHub Profile README Generator

**Goal:** Build a web app that reads a GitHub user's repos and generates a polished profile README with stats, badges, and highlights.

**Time Budget:** 1–2 weekends (8–16 hours)
**Live Hermes Board:** `github-readme-generator` board — 11/12 done, 1 archived
**Status:** Shipped — deployed to Vercel, README written, LinkedIn post drafted. Social sharing task archived (per Rick's no-auto-post rule).

---

## Live Hermes Kanban Tasks

| ID | Task | Status | Original # |
|---|---|---|---|
| t_9d15bbcf | Scaffold Next.js project with shadcn/ui | done | 1 |
| t_a2a4c58b | Set up GitHub API integration (REST + GraphQL) | done | 2 |
| t_9f078750 | Fetch user profile + top repos + language stats | done | 3 |
| t_f3959327 | Design README template structure | done | 4 |
| t_ac4ced0c | Build LLM prompt for README generation | done | 5 |
| t_5282ff23 | Build UI - username input + preview panel | done | 6 |
| t_a6d6d45b | Generate markdown output with copy button | done | 7 |
| t_f1e629ce | Add GitHub stats cards (generated badges) | done | 8 |
| t_75717a7f | Deploy to Vercel | done | 9 |
| t_ded4b72b | Write project README + add screenshot/GIF | done | 10 |
| t_66f4bc17 | Draft LinkedIn post | done | 11 |
| t_a35d9a79 | Share on LinkedIn + relevant subreddits | archived | 12 |

**Note:** Task 12 (social sharing) was archived per Rick's standing rule: no social media posting without explicit approval. LinkedIn post draft exists and is ready to post when Rick gives the go-ahead.

---

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Styling:** Tailwind + shadcn/ui
- **APIs:** GitHub REST API, OpenAI API (gpt-4o-mini)
- **State:** React hooks (no state library needed)
- **Deploy:** Vercel (free tier)

## Success Criteria

- [x] Live demo deployed to Vercel
- [x] Generates a README I'd actually use on my own profile
- [ ] LinkedIn post published with engagement (drafted, pending Rick's approval to post)

## Blockers / Risks

- GitHub API rate limits (60 req/hr unauthenticated, 5000 with PAT) — handled with PAT
- LLM output inconsistency — addressed through prompt iteration
- No offline capability — requires GitHub API + OpenAI API (acceptable for demo)

## Next Steps

1. Rick reviews the live demo and LinkedIn draft
2. If approved, un-archive task 12 and post
3. Add to portfolio site when rebuilt
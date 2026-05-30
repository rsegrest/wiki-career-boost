---
title: "Kanban: GitHub Profile README Generator"
created: 2026-05-30
type: comparison
tags: [kanban, portfolio, project-management]
---

# Kanban: GitHub Profile README Generator

**Goal:** Build a web app that reads a GitHub user's repos and generates a polished profile README with stats, badges, and highlights.

**Time Budget:** 1–2 weekends (8–16 hours)
**Ship Date Target:** June 5, 2026 (before cruise)

---

## Backlog

| # | Task | Est. | Priority | Notes |
|---|------|------|----------|-------|
| 1 | Scaffold Next.js project with shadcn/ui | 30 min | P0 | `npx shadcn@latest init` |
| 2 | Set up GitHub API integration (REST + GraphQL) | 1 hr | P0 | PAT token, rate limit handling |
| 3 | Fetch user profile + top repos + language stats | 1 hr | P0 | `/users/{user}`, `/users/{user}/repos` |
| 4 | Design README template structure | 1 hr | P0 | Header, stats, top repos, skills, social |
| 5 | Build LLM prompt for README generation | 1 hr | P0 | OpenAI API, gpt-4o-mini is fine |
| 6 | Build UI: username input + preview panel | 2 hr | P0 | Form + split-pane preview |
| 7 | Generate markdown output with copy button | 30 min | P0 | `react-markdown` or raw string |
| 8 | Add GitHub stats cards (generated badges) | 1 hr | P1 | github-readme-stats or custom |
| 9 | Deploy to Vercel | 30 min | P0 | Git push → Vercel auto-deploy |
| 10 | Write README + add screenshot/GIF | 30 min | P1 | Good README = more stars |
| 11 | Draft LinkedIn post | 30 min | P1 | Ship together with code |
| 12 | Share on LinkedIn + relevant subreddits | 15 min | P2 | r/webdev, r/reactjs, r/cscareerquestions |

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
- **APIs:** GitHub REST API, OpenAI API
- **State:** React hooks (no state library needed)
- **Deploy:** Vercel (free tier)

## Blockers / Risks

- GitHub API rate limits (60 req/hr unauthenticated, 5000 with PAT)
- LLM output inconsistency — may need prompt iteration
- No offline capability — requires GitHub API + OpenAI API

## Success Criteria

- [ ] Live demo at `ricksegrest.com` or Vercel subdomain
- [ ] Generates a README I'd actually use on my own profile
- [ ] 1 LinkedIn post published with engagement

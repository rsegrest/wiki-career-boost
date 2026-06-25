---
title: "Kanban: Nomad Cost-of-Living Dashboard"
created: 2026-05-30
updated: 2026-06-24
type: comparison
tags: [kanban, portfolio, project-management, hermes-dashboard]
---

# Kanban: Nomad Cost-of-Living Dashboard

**Goal:** Interactive dashboard comparing nomad cities on cost, wifi, safety, family-friendliness using your travel wiki data.

**Time Budget:** 1–2 weekends (8–16 hours)
**Live Hermes Board:** `nomad-cost-dashboard` board — 11/12 done, 1 archived
**Status:** Shipped — deployed to Vercel, README written, LinkedIn post drafted. "Rick's visited" badge feature archived as not worth the effort.

---

## Live Hermes Kanban Tasks

| ID | Task | Status | Original # |
|---|---|---|---|
| t_9c7ed77f | Export wiki city data to JSON | done | 1 |
| t_389ada6f | Scaffold Next.js project with shadcn/ui + Recharts | done | 2 |
| t_2dd6a77f | Design data schema for city comparisons | done | 3 |
| t_f7be1d12 | Build city comparison table (sortable, filterable) | done | 4 |
| t_3452ecf9 | Add radar/spider chart for city multi-metric view | done | 5 |
| t_288d9a62 | Add cost breakdown bar chart | done | 6 |
| t_f2489d34 | Add interactive filters (region, budget, family-friendly) | done | 7 |
| t_fe57ab58 | Add city detail modal/page | done | 8 |
| t_f8ac6745 | Add "Rick's visited" badge overlay | archived | 9 |
| t_db3c77c9 | Deploy to Vercel | done | 10 |
| t_6ba9ac61 | Write project README + add screenshots | done | 11 |
| t_419f85cf | Draft LinkedIn post | done | 12 |

**Note:** Task 9 ("Rick's visited" badge) was archived — deemed not worth the effort for the value it adds. Core dashboard functionality is complete.

---

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Styling:** Tailwind + shadcn/ui
- **Charts:** Recharts
- **Data:** Static JSON exported from travel wiki
- **Deploy:** Vercel

## Success Criteria

- [x] Live demo with at least 15 cities
- [x] Interactive filtering and sorting works
- [ ] LinkedIn post published with engagement (drafted, pending Rick's approval to post)

## Blockers / Risks

- Data completeness — not all cities have full data (handled by showing N/A where missing)
- Design decisions — which metrics matter most? (resolved: cost, wifi, safety, family-friendly)
- Static data means manual updates when wiki changes (acceptable for portfolio piece)

## Next Steps

1. Rick reviews the live demo and LinkedIn draft
2. If approved, post LinkedIn article
3. Add to portfolio site when rebuilt
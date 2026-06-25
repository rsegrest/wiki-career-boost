---
title: "Portfolio Project Kanban Hub"
created: 2026-05-30
updated: 2026-06-24
type: comparison
tags: [kanban, portfolio, project-management, hub, hermes-dashboard]
---

# Portfolio Project Kanban Hub

**Goal:** Track and manage portfolio projects showcasing Rick's triad: React + M&S + AI.

**Hermes Boards:** 3 boards, all viewable from the Hermes dashboard. Switch with `hermes kanban boards switch <slug>`.

---

## Projects

| Project | Status | Board Slug | Tasks | Wiki |
|---------|--------|------------|-------|------|
| AI UX Critique Tool | Shipped — testing & improving | `default` | 10/10 done | [[kanban/ai-ux-critique-tool]] |
| GitHub README Generator | Shipped — awaiting social approval | `github-readme-generator` | 11/12 done, 1 archived | [[kanban/github-readme-generator]] |
| Nomad Cost Dashboard | Shipped — awaiting social approval | `nomad-cost-dashboard` | 11/12 done, 1 archived | [[kanban/nomad-cost-dashboard]] |

---

## All Three Projects Shipped

All three portfolio projects have been built and deployed to Vercel by autonomous Hermes kanban workers. Each has a live demo, GitHub repo, and README. LinkedIn posts have been drafted but NOT published — per Rick's standing rule, social media posting requires explicit approval.

### UX Critique Tool — Post-Ship Status

All 10 kanban tasks completed. Project is live and deployed at `/home/rick/projects/ux-critique-tool/` with a GitHub repo at `rsegrest/ux-critique-tool`. Now in iteration mode:
- Testing with real screenshots across various UI types
- Refining the critique prompt for accuracy and consistency
- Improving bounding box coordinate precision
- Polishing the UI based on user feedback
- LinkedIn post drafted, pending Rick's approval to publish

See [[kanban/ai-ux-critique-tool]] for full architectural decisions, the prompt spec, and success criteria checklist.

### GitHub README Generator — Shipped

11/12 tasks completed by kanban workers. Deployed to Vercel. Features:
- GitHub username input with live preview
- Fetches user profile, top repos, language stats via GitHub API
- LLM generates polished README markdown with stats and badges
- Copy-to-clipboard output
- Task 12 (social sharing) archived per no-auto-post rule

See [[kanban/github-readme-generator]] for task IDs and details.

### Nomad Cost Dashboard — Shipped

11/12 tasks completed by kanban workers. Deployed to Vercel. Features:
- Sortable, filterable city comparison table
- Radar chart for multi-metric city comparison
- Cost breakdown bar charts
- Interactive filters (region, budget, family-friendly)
- City detail modal
- Data exported from travel wiki as static JSON
- Task 9 ("Rick's visited" badge) archived — not worth the effort

See [[kanban/nomad-cost-dashboard]] for task IDs and details.

---

## Ship Checklist (Every Project)

- [x] Live demo deployed (all 3)
- [x] GitHub repo with good README (all 3)
- [x] Screenshots/GIF in README (all 3)
- [x] LinkedIn post drafted (all 3)
- [ ] Posted on LinkedIn (pending Rick's approval — all 3)
- [ ] Added to portfolio site (if rebuilt)

---

## Log

| Date | Project | Action | Notes |
|------|---------|--------|-------|
| 2026-05-30 | All | Wiki kanban pages created | Backlog tasks defined |
| 2026-06-22 | UX Critique Tool | All 10 tasks completed | Deployed, README written |
| 2026-06-23 | All | Hermes kanban boards restructured | 3 boards: default (UX), github-readme-generator, nomad-cost-dashboard |
| 2026-06-23 | GitHub README | 12 tasks created + linked | 4 running, 8 waiting on scaffold |
| 2026-06-23 | Nomad Dashboard | 12 tasks created + linked | 2 ready, 10 waiting on scaffold |
| 2026-06-24 | GitHub README | 11/12 done, 1 archived | Social sharing task archived per no-auto-post rule |
| 2026-06-24 | Nomad Dashboard | 11/12 done, 1 archived | "Rick's visited" badge archived — not worth the effort |
| 2026-06-24 | All | Wiki kanban pages updated to match Hermes board state | All 3 projects now show as shipped |
---
title: "Portfolio Project Kanban Hub"
created: 2026-05-30
updated: 2026-06-23
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
| GitHub README Generator | In Progress | `github-readme-generator` | 0/12 done, 4 running | [[kanban/github-readme-generator]] |
| Nomad Cost Dashboard | In Progress | `nomad-cost-dashboard` | 0/12 done, 2 ready | [[kanban/nomad-cost-dashboard]] |

---

## UX Critique Tool — Post-Ship Status

All 10 kanban tasks completed. Project is live and deployed. Now in iteration mode:
- Testing with real screenshots across various UI types
- Refining the critique prompt for accuracy and consistency
- Improving bounding box coordinate precision
- Polishing the UI based on user feedback
- Social sharing and LinkedIn post pending final polish

See [[kanban/ai-ux-critique-tool]] for full architectural decisions, the prompt spec, and success criteria checklist.

---

## GitHub README Generator — Active Board

12 tasks created on the `github-readme-generator` board. Scaffold, GitHub API, template design, and LLM prompt tasks are running in parallel (no dependencies). Remaining tasks depend on scaffold completion.

Tech: Next.js 15 + shadcn/ui + OpenAI gpt-4o-mini + GitHub REST API. Deploy target: Vercel.

---

## Nomad Cost Dashboard — Active Board

12 tasks created on the `nomad-cost-dashboard` board. Data export and scaffold tasks are ready (no dependencies). Remaining tasks depend on scaffold completion.

Tech: Next.js 15 + shadcn/ui + Recharts. Data: static JSON from travel wiki. Deploy target: Vercel.

---

## Ship Checklist (Every Project)

- [ ] Live demo deployed
- [ ] GitHub repo with good README
- [ ] Screenshots/GIF in README
- [ ] LinkedIn post drafted
- [ ] Posted on LinkedIn
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

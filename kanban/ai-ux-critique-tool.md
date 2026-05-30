---
title: "Kanban: AI-Powered UX Critique Tool"
created: 2026-05-30
type: comparison
tags: [kanban, portfolio, project-management]
---

# Kanban: AI-Powered UX Critique Tool

**Goal:** Web app where you paste a UI screenshot and an LLM critiques it using Nielsen's 10 heuristics, WCAG guidelines, and Gestalt principles.

**Time Budget:** 1–2 weekends (8–16 hours)
**Ship Date Target:** June 5, 2026 (before cruise)

---

## Backlog

| # | Task | Est. | Priority | Notes |
|---|------|------|----------|-------|
| 1 | Scaffold Next.js project with shadcn/ui | 30 min | P0 | `npx shadcn@latest init` |
| 2 | Build image upload component (drag + drop, paste) | 1 hr | P0 | React Dropzone or native |
| 3 | Integrate OpenAI Vision API (gpt-4o/gpt-4o-mini) | 1 hr | P0 | Image input + structured output |
| 4 | Craft system prompt with Nielsen heuristics + WCAG | 1.5 hr | P0 | Need to nail this for quality |
| 5 | Design critique output format (structured JSON) | 1 hr | P0 | Category, severity, suggestion, reference |
| 6 | Build critique display UI (cards, severity colors) | 2 hr | P0 | shadcn Card, Badge, Collapsible |
| 7 | Add "before/after" mockup suggestion feature | 2 hr | P1 | Use AI to suggest redesigns (harder) |
| 8 | Add example screenshots (Dribbble, bad UI examples) | 30 min | P1 | Demo without uploading |
| 9 | Deploy to Vercel | 30 min | P0 | Git push → Vercel auto-deploy |
| 10 | Write README + add screenshot/GIF | 30 min | P1 | Show it critiquing a real UI |
| 11 | Draft LinkedIn post | 30 min | P1 | "I built an AI UX reviewer" |
| 12 | Share on LinkedIn + Designer News + Reddit | 15 min | P2 | r/webdev, r/userexperience |

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
- **AI:** OpenAI GPT-4o Vision API
- **State:** React hooks
- **Deploy:** Vercel

## Blockers / Risks

- Vision API cost — gpt-4o is cheaper, gpt-4o-mini even cheaper
- Output quality depends heavily on prompt engineering
- May need few-shot examples in prompt for consistent formatting
- No offline — requires OpenAI API

## Success Criteria

- [ ] Live demo that generates a critique I'd share with a designer
- [ ] Catches at least 3 real issues on a known-bad UI screenshot
- [ ] 1 LinkedIn post with engagement from UX + AI communities

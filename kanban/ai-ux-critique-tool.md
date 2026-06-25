---
title: "Kanban: AI-Powered UX Critique Tool"
created: 2026-05-30
updated: 2026-06-24
type: comparison
tags: [kanban, portfolio, project-management, hermes-dashboard]
sources: [freelance-portfolio-strategy.md]
---

# Kanban: AI-Powered UX Critique Tool

**Goal:** Web app where you paste a UI screenshot and an LLM critiques it using Nielsen's 10 heuristics, WCAG guidelines, and Gestalt principles. Annotated image overlay with numbered markers.

**Time Budget:** 2 weekends (16-20 hours)
**Live Hermes Board:** `default` board (slug: default), 10/10 tasks done
**Status:** Shipped — in testing & iteration mode

---

## Live Hermes Kanban Tasks

| ID | Task | Status | Depends On |
|---|---|---|---|
| t_e0339420 | Scaffold Next.js + shadcn/ui project | done | — |
| t_1acea534 | Image upload + drop zone component | done | T1 |
| t_324d3757 | Craft structured UX critique prompt | done | T1 |
| t_38d3a25c | API route + vision model integration | done | T1, T3 |
| t_1110294a | Critique display UI with severity badges | done | T2, T4 |
| t_ba819091 | Annotated image overlay with bounding boxes | done | T5 |
| t_a72bab0c | Example screenshots + demo mode | done | T6 |
| t_f2c747da | Deploy to Vercel | done | T7 |
| t_e6dbb8ad | README case study + GitHub repo polish | done | T8 |
| t_069bff13 | LinkedIn post + social sharing | done | T9 |

## Task Dependency Graph

```
T1 Scaffold ──┬──> T2 Image Upload ──┐
              │                        ├──> T5 Critique UI ──> T6 Overlay ──> T7 Examples ──> T8 Deploy ──> T9 README ──> T10 LinkedIn
              └──> T3 Prompt ──> T4 API ┘
```

T2 and T3 run in parallel after T1. T4 waits for T3 (needs the prompt). T5 waits for T2 + T4 (needs upload + API). Everything after T5 is sequential.

## Tech Stack

- **Framework:** Next.js 15 (App Router) + React 19 + TypeScript
- **Styling:** Tailwind CSS + shadcn/ui (dark theme)
- **AI:** OpenAI GPT-4o Vision (primary) or Anthropic Claude 3.5 Sonnet (alternative)
- **Image Input:** react-dropzone (drag-drop + paste)
- **Animation:** framer-motion
- **Deploy:** Vercel
- **API Keys:** Rick has OpenAI and Anthropic keys configured

## Key Architectural Decisions

1. **Structured JSON output** — the prompt forces the vision model to return findings as JSON with bounding box coordinates, not freeform text
2. **Bounding box overlay** — the killer feature. Numbered markers on the screenshot linked to critique cards. This is what makes the demo shareable.
3. **Model-agnostic via Vercel AI SDK** — can swap between OpenAI and Anthropic without changing code
4. **Usage limit** — 5 critiques per IP per day to prevent API credit burn on the free demo

## The Prompt (The IP)

The system prompt instructs the vision model to analyze against:
1. **Nielsen's 10 Usability Heuristics** — visibility of system status, match real world, user control, consistency, error prevention, recognition over recall, flexibility/efficiency, aesthetic/minimalist, error recovery, help/docs
2. **WCAG 2.1 AA** — color contrast (4.5:1), focus indicators, alt text inference, text spacing
3. **Gestalt Principles** — proximity, similarity, continuity, closure, common region

Output schema per finding:
```json
{
  "finding": "Low contrast text on button",
  "heuristic_violated": "WCAG 1.4.3 Contrast (Minimum)",
  "severity": "serious",
  "confidence": "high",
  "recommendation": "Increase button text contrast to at least 4.5:1 ratio",
  "bounding_box": {"x": 15.2, "y": 42.3, "width": 22.1, "height": 8.5}
}
```

## Success Criteria

- [x] Live demo that generates a critique I'd share with a designer
- [x] Catches at least 3 real issues on a known-bad UI screenshot
- [x] Bounding box annotations accurately point to problem areas
- [x] Polished dark theme UI that looks professional
- [x] 1 LinkedIn post drafted (task t_069bff13 done — pending Rick's approval to publish)
- [x] GitHub repo with stellar README

## Blockers / Risks

- Vision API cost — GPT-4o is ~$0.01-0.03 per image. Add usage limits.
- Bounding box accuracy — vision models aren't perfect at spatial coordinates. May need to tolerate some imprecision.
- Output quality depends heavily on prompt engineering — T3 is the most important task
- No offline mode — requires API key (acceptable for demo)
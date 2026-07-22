---
title: Project Tracker
created: 2026-07-21
updated: 2026-07-21
type: concept
tags: [project, tracker, index, meta, portfolio]
confidence: high
---

# Project Tracker

> Master tracker of every project I've worked on — status, models used, and last activity.
>
> Companion to `~/wiki-personal/concepts/project-plans-index.md` (priority order & plans) and this wiki's [[portfolio-project-ideas]] (full idea catalog #1–56+).

---

## Active / In Progress

| ID | Project | Description | Status | Models Used | Last Worked |
|----|---------|-------------|--------|-------------|-------------|
| MC | **Mission Control** | Agent OS dashboard for Hermes — sessions, tools, skills, cron, kanban. Port 3006. | ✅ Tier 1–2 done; **Tier 3 on hold** (Kanban/TODO + wiki viewer planned) | Claude Code Opus 4.8 (core merge), Sonnet 5 (adapter), glm-5.2 (orchestration), DeepSeek V4 Flash/Pro (Tier 1–2 UX) | 2026-07-15 |
| PS | **Personal Site** | Dark-only Vite+React portfolio gallery. Port 3010. | ✅ Blog scaffold + 4 seed posts + Travel nav link; **needs** hero/CTA/resume/layout polish + real posts | DeepSeek V4 Pro (main coding), DeepSeek V4 Flash (blog/polish), early Tencent HY3 design (+ some Gemini 3.5 Flash) | 2026-07-14 |
| TM | **Travel Map** | D3 geo SVG map of places visited. Port 3007. | ✅ Multi-year years UX; **needs** dark theme swap + blog integration + state data | (not fully audited) | 2026-07-15 |
| HP | **Hyperfocus Planner** | AI-powered TO-DO that breaks long-term goals into daily plans. | 🔄 Phase 1: OpenAI planning + Google Calendar OAuth | ChatGPT Codex | 2026-07-11 |
| LC | **Local LLM Chat** | Polished ChatGPT-style UI for local Ollama/LM Studio with personality presets. | 🔄 Scaffolded, spec written, not yet built | DeepSeek V4 Flash (scaffold) | 2026-07-11 |
| WS | **Writing Sprint App** | Write or Die-inspired sprint app with consequences + NaNoWriMo support. | 📋 Spec written, not started | — | 2026-07-15 (spec) |

## Shipped / Deployed (needs testing & data)

| ID | Project | Description | Status | Models Used | Last Worked |
|----|---------|-------------|--------|-------------|-------------|
| UX | **UX Critique Tool** | AI-powered UX critique using Vision API + Nielsen heuristics. Vercel. | ✅ SHIPPED — **needs further testing** before promotion | DeepSeek V4 Flash | 2026-06-22 |
| ND | **Nomad Cost Dashboard** | Cost-of-living comparison dashboard with Recharts. Vercel. | ✅ SHIPPED — **needs more data sets** to be useful; 11/12 tasks done, 1 archived | DeepSeek V4 Flash | 2026-06 |
| GR | **GitHub README Generator** | Agentic tool that reads repos and generates polished READMEs. Vercel. | ✅ SHIPPED — **needs further testing** before promotion; 11/12 tasks done, 1 archived | DeepSeek V4 Flash | 2026-06 |
| MB | **Agent Memory Browser** | SQLite CRUD + graph viz for Hermes agent memory. Port 3001. | ✅ DONE — composed into Mission Control; **needs further testing** | Hermes scaffold + Claude Code | 2026-07-11 |
| TV | **Agent Tool Visualizer** | Real-time polling feed of agent tool executions. Port 3004. | ✅ DONE — composed into Mission Control; **needs further testing** | Hermes scaffold + Claude Code | 2026-07-11 |
| CT | **Agent Cron Monitor** | Cron timeline, health monitor, job CRUD. Port 3002. | ✅ DONE — composed into Mission Control; **needs further testing** | Hermes scaffold + Claude Code | 2026-07-11 |
| SH | **Agent Session Browser** | FTS5 search + conversation tree + export. Port 3003. | ✅ DONE — composed into Mission Control; **needs further testing** | Hermes scaffold + Claude Code | 2026-07-11 |

## Side / Experimental

| ID | Project | Description | Status | Models Used | Last Worked |
|----|---------|-------------|--------|-------------|-------------|
| IG | **Image Gen Composer** | Flask app — CivitAI collection browser + ComfyUI image gen. Port 7777. | 🔧 Running, occasional use | DeepSeek V4 Flash | 2026-04-27 |
| GC | **Game Clawtroller** | Casino games with agent interface. | 🔧 Experimental | DeepSeek V4 Flash | 2026-04-06 |
| AP | **Agentic Patterns MVPs** | Collection of agent design pattern MVPs. | 🔧 Experimental | DeepSeek V4 Flash | 2026-06-29 |
| 8B | **8-Bit Game Dev Resources** | Downloaded reference library from awesome-8bitgamedev. | 📦 Reference archive | DeepSeek V4 Flash | 2026-07-17 |

## Planned / Spec'd

| ID | Project | Description | Status | Models Used | Last Worked |
|----|---------|-------------|--------|-------------|-------------|
| DT | **Digital Twin** | Visual simulation of a real-world system (traffic, queue, supply chain). | 📋 Available | — | — |
| RO | **Resume Optimizer** | RAG-based resume + job description analysis. | 📋 Available | — | — |
| SP | **Skill/Plugin Manager** (#54) | Agent OS skill/plugin file CRUD + admin panel. | 📋 Available | — | — |
| — | *Many more in portfolio-project-ideas.md (#4–49)* | — | 📋 Available | — | — |

---

## Legend

| Icon | Meaning |
|------|---------|
| ✅ | Complete / shipped |
| 🔄 | In active development |
| 🔧 | Experimental / occasional use |
| 📋 | Planned / spec written |
| 📦 | Reference / archive |

## Notes

- **"Shipped / Deployed (needs testing & data)"** projects are live and functional but need real-world testing and/or richer data before I promote them as portfolio centerpieces.
  - **Nomad Cost Dashboard** specifically needs more city data sets to be genuinely useful.
  - **UX Critique Tool, GitHub README Generator, Agent OS MVPs** need thorough testing to shake out edge cases.
- **Mission Control** and **Personal Site** are the two primary active projects. Everything else is lower priority.
- **Agent OS MVPs** (#50–53) are individually done and composed into Mission Control. They still run on their original ports but are superseded by the unified dashboard.
- **Model preference:** Flash for bulk code/analysis, Pro or GLM-5.2 for complex coding, GLM-5.2 for prose drafts, Grok + humanizer for voice editing.
- **Cost preference:** Revert to Flash after heavy sessions. Don't cheap out on launch copy.

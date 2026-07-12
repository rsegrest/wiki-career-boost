---
title: Portfolio Project Ideas for Career Networking
created: 2026-05-30
updated: 2026-07-11
type: concept
tags: [portfolio, side-project, career, react, ai, networking, open-source]
sources: []
status: active
---

# Portfolio Project Ideas for Career Networking

> Curated project ideas that showcase Rick's rare triad: React + M&S + AI.
> Each idea is chosen for maximum conversation-starting potential on LinkedIn, GitHub, and at meetups.

---

## Idea Index

> **⭐ July 2 picks:** #4 (Digital Twin — traffic flow), #5 (Resume Optimizer), #9 (Personal OS Dashboard), #9a (Agent OS Mission Control), #11 (Local LLM Chat), #15 (Codebase Explorer), #50-54 (Agent OS MVP series)

| # | Idea | Category | Status | Skills |
|---|------|----------|--------|--------|
| 1 | [AI-Powered UX Critique Tool](#1-ai-powered-ux-critique-tool) | Quick Win | SHIPPED | Vision API, UX heuristics, overlay annotation |
| 2 | [Nomad Cost-of-Living Dashboard](#2-nomad-cost-of-living-dashboard) | Quick Win | SHIPPED | Data viz, Recharts, filterable tables |
| 3 | [GitHub Profile README Generator](#3-github-profile-readme-generator) | Quick Win | SHIPPED | GitHub API, LLM generation, copy UX |
| ⭐4 | [Digital Twin of a Simple System](#4-digital-twin-of-a-simple-system) | M&S | Available | Canvas/SVG, state machine, LLM advisor |
| ⭐5 | [AI Resume Optimizer](#5-ai-resume-optimizer) | Medium | Available | RAG, PDF parsing, vector DB |
| 6 | [React + PowerApps Bridge Demo](#6-react--powerapps-bridge-demo) | Medium | Available | PCF, enterprise integration |
| 7 | [Open-Source Agentic Development Toolkit](#7-open-source-agentic-development-toolkit) | Showcase | Available | Playwright, agent orchestration, npm |
| 8 | [React Component Library for Simulation Viz](#8-react-component-library-for-simulation-visualizations) | Showcase | Available | D3, Storybook, npm |
| ⭐9 | [Personal "Operating System" Dashboard](#9-personal-operating-system-dashboard) | Showcase | Available | Multi-API, LLM insights, local storage |
| ⭐9a | [Agent OS — Mission Control for Hermes](#9a-agent-os--mission-control-for-hermes-new-july-2026) | Showcase | Available | WebSocket, SQLite, Recharts, agent infra |
| 10 | [AI Meeting Transcript Analyzer](#10-ai-meeting-transcript-analyzer) | Practical | Available | Structured output, document processing |
| ⭐11 | [Local LLM Chat Interface](#11-local-llm-chat-interface) | Practical | Available | Streaming, Ollama, real-time UX |
| 12 | [AI-Powered Obsidian Wiki Explorer](#12-ai-powered-obsidian-wiki-explorer) | Practical | Available | Graph viz, embeddings, vector search |
| 13 | ["Roast My Landing Page"](#13-roast-my-landing-page) | Viral | Available | Browser automation, shareable cards |
| 14 | [AI Agent Sandbox](#14-ai-agent-sandbox) | Viral | Available | Multi-agent, WebSocket, function calling |
| ⭐15 | [Interactive "Explain This Codebase" Explorer](#15-interactive-explain-this-codebase-explorer) | Viral | Available | Code analysis, graph viz, GitHub API |
| 16 | [Budget Proposal Estimator](#16-budget-proposal-estimator-non-proprietary) | Career-Signal | Available | Complex forms, financial viz, domain expertise |
| 17 | [Electron + AI Desktop App Template](#17-electron--ai-desktop-app-template) | Career-Signal | Available | Electron, desktop AI, system integration |
| 18 | [AI Code Review Dashboard](#18-ai-code-review-dashboard) | Career-Signal | Available | GitHub API, code analysis, diff UX |
| 19 | [Digital Twin of a Simple System](#19-digital-twin-of-a-simple-system) | M&S Anchor | Available | Canvas/SVG, simulation, LLM advisor |
| 20 | [Monte Carlo Retirement Planner](#20-monte-carlo-retirement-planner) | M&S | Available | Statistical simulation, Web Workers, D3 |
| 21 | [Agent-Based Epidemic Simulator](#21-agent-based-epidemic-simulator) | M&S | Available | SIR model, canvas animation, LLM advisor |
| 22 | [Queueing Theory Visualizer](#22-queueing-theory-visualizer) | M&S | Available | Operations research, animated SVG, math viz |
| 23 | [AI Hallucination Detector](#23-ai-hallucination-detector) | AI Safety | Available | RAG verification, text highlighting, grounding |
| 24 | [LLM Prompt Version Control & A/B Tester](#24-llm-prompt-version-control--ab-tester) | AI Safety | Available | Eval methodology, dev tooling, diff viewer |
| 25 | [AI Decision Audit Trail](#25-ai-decision-audit-trail) | AI Safety | Available | Logging architecture, monitoring, observability |
| 26 | [Natural Language SQL Query Builder](#26-natural-language-sql-query-builder) | Data + AI | Available | NL-to-SQL, database, multi-turn conversation |
| 27 | [AI-Powered API Explorer](#27-ai-powered-api-explorer--postman-alternative) | Data + AI | Available | HTTP protocol, API design, dev tooling |
| 28 | [Spreadsheet AI Formulas Assistant](#28-spreadsheet-ai-formulas-assistant) | Data + AI | Available | Practical AI, spreadsheet UX, non-technical design |
| 29 | [AI Storyboard Generator](#29-ai-storyboard-generator) | Creative | Available | Multi-modal AI, image gen, PDF export |
| 30 | [AI Color Palette Generator from Images](#30-ai-color-palette-generator-from-images) | Creative | Available | Canvas API, color theory, design tooling |
| 31 | [AI Music Mood Board](#31-ai-music-mood-board) | Creative | Available | Audio API, multi-modal, Spotify integration |
| 32 | [AI-Powered Meal Planner](#32-ai-powered-meal-planner) | Life Tool | Available | Complex forms, AI planning, practical UX |
| 33 | [ESA / Education Savings Tracker](#33-esa--education-savings-tracker) | Life Tool | Available | Financial tracking, regulatory logic, data viz |
| 34 | [AI Family Calendar Optimizer](#34-ai-family-calendar-optimizer) | Life Tool | Available | Calendar integration, scheduling, iCal export |
| 35 | [Proposal Win/Loss Analyzer](#35-proposal-winloss-analyzer) | Gov/Defense | Available | Proposal scoring, RFP eval rubric, radar chart |
| 36 | [Contract Vehicle Comparison Tool](#36-contract-vehicle-comparison-tool) | Gov/Defense | Available | Gov contracting, comparison tables, regulatory |
| 37 | [Security Clearance Eligibility Quiz](#37-security-clearance-eligibility-quiz) | Gov/Defense | Available | Clearance domain, multi-step wizard, progress viz |
| 38 | [AI Agent Orchestrator Dashboard](#38-ai-agent-orchestrator-dashboard) | Dev Infra | Available | Real-time monitoring, queue mgmt, operational UX |
| 39 | [Cron Job Visualizer & Health Monitor](#39-cron-job-visualizer--health-monitor) | Dev Infra | Available | System monitoring, timeline viz, failure analysis |
| 40 | [Self-Hosted AI Dashboard (Home Lab Monitor)](#40-self-hosted-ai-dashboard-home-lab-monitor) | Dev Infra | Available | Hardware metrics, real-time dashboard, Ollama API |
| 41 | [Accessible Color Contrast Simulator](#41-accessible-color-contrast-simulator) | Accessibility | Available | WCAG, Canvas image processing, inclusive design |
| 42 | [Screen Reader Preview Tool](#42-screen-reader-preview-tool) | Accessibility | Available | Accessibility tree, DOM parsing, dev education |
| 43 | [Form Accessibility Auditor](#43-form-accessibility-auditor) | Accessibility | Available | Form a11y, axe-core, automated testing |
| 44 | [AI-Powered Link Preview Generator](#44-ai-powered-link-preview-generator) | Content | Available | HTML parsing, metadata extraction, card design |
| 45 | [AI Knowledge Base Generator](#45-ai-knowledge-base-generator) | Content | Available | Document processing, embeddings, clustering |
| 46 | [AI-Powered Changelog Generator](#46-ai-powered-changelog-generator) | Content | Available | Git parsing, release notes, dev tooling |
| 47 | [AI-Powered Flashcard Generator](#47-ai-powered-flashcard-generator) | Education | Available | Content extraction, spaced repetition, Anki export |
| 48 | [Interactive Regex Teacher](#48-interactive-regex-teacher) | Education | Available | Real-time text processing, educational UX |
| 49 | [AI-Powered Code Snippet Explainer](#49-ai-powered-code-snippet-explainer) | Education | Available | Code comprehension, syntax highlighting, education |
| ⭐50 | [Agent Memory Browser](#50-agent-memory-browser) | Agent OS | ✅ DONE :3001 | SQLite CRUD, graph viz, file watching, admin UX |
| ⭐51 | [Agent Tool Execution Visualizer](#51-agent-tool-execution-visualizer) | Agent OS | ✅ DONE :3004 | Polling feed, real-time UI, JSON viewer, replay |
| ⭐52 | [Agent Cron Timeline & Health Monitor](#52-agent-cron-timeline--health-monitor) | Agent OS | ✅ DONE :3002 | System monitoring, cron parsing, timeline viz, job CRUD |
| ⭐53 | [Agent Session History Browser](#53-agent-session-history-browser) | Agent OS | ✅ DONE :3003 | FTS5 search, conversation tree, export UX |
| ⭐54 | [Agent Skill/Plugin Manager](#54-agent-skillplugin-manager) | Agent OS | Available | File CRUD, YAML parsing, admin panel UX |
| ⭐55 | [Hyperfocus Planner](#55-hyperfocus-planner-arcday) | Productivity | ✅ IN PROGRESS | AI planning, calendar integration, goal decomposition |

---

## Round 1 — Original Ideas (May 2026)

### Quick Wins (1-3 weekends)

### 1. AI-Powered UX Critique Tool
**What:** A web app where you paste a screenshot of any UI and an LLM critiques it using Nielsen's 10 heuristics, WCAG guidelines, and Gestalt principles.
**Stack:** React + OpenAI Vision API + shadcn/ui
**Why it networks:** Combines your UX expertise + AI skills. Tweet/LinkedIn post: "I built an AI that critiques UX like a senior designer." Instant engagement from both UX and AI communities.
**Shareable output:** Live demo + blog post on accuracy testing
**Status:** SHIPPED — deployed to Vercel, GitHub repo at rsegrest/ux-critique-tool, 10/10 kanban tasks done

### 2. Nomad Cost-of-Living Dashboard
**What:** Interactive dashboard using your travel wiki data — compare cities on cost, wifi, safety, family-friendliness.
**Stack:** Next.js + Recharts + your wiki data
**Why it networks:** Shows you "eat your own dog food" (using data you personally collected). Perfect for digital nomad/dev communities. Tangible proof of full-stack + data viz skills.
**Shareable output:** Live site + case study on building with real data
**Status:** SHIPPED — deployed to Vercel, 11/12 kanban tasks done, 1 archived

### 3. GitHub Profile README Generator
**What:** An agentic tool that reads someone's GitHub repos, summarizes their tech stack, and generates a polished profile README with stats, badges, and project highlights.
**Stack:** React frontend + Python FastAPI backend + GitHub API + LLM
**Why it networks:** Solves a real problem every developer has. Easy for others to use and share. Network effect: every person who uses it sees your name.
**Shareable output:** Live tool + "I built this in a weekend" thread
**Status:** SHIPPED — deployed to Vercel, 11/12 kanban tasks done, 1 archived

---

### Medium Projects (2-4 weeks)

### 4. Digital Twin of a Simple System
**What:** A visual simulation of a real-world system (traffic flow, coffee shop queue, supply chain) where users can tweak parameters and watch emergent behavior. Add an AI agent that "optimizes" the system.
**Stack:** React canvas/SVG + state machine + LLM advisor
**Why it networks:** Directly uses your M&S Master's. Bridges simulation + web + AI. NASA-adjacent work. Defense contractors understand "digital twin" language.
**Shareable output:** Interactive demo + "From M&S to Web: Building Digital Twins in React" article

### 5. AI Resume Optimizer
**What:** Upload your resume + a job description. The app uses RAG to suggest specific rewrites, skills to highlight, and gap analysis.
**Stack:** Next.js + OpenAI + vector DB (Pinecone) + PDF parsing
**Why it networks:** Meta — the tool helps with job searching while you job search. "I built the tool I wish I had" is a classic narrative. Recruiters and career coaches will share it.
**Shareable output:** Live tool + "How I used AI to optimize my own resume" case study

### 6. React + PowerApps Bridge Demo
**What:** Show how to extend PowerApps with custom React components. A tutorial + working example of a complex component (e.g., interactive map, data viz) embedded in PowerApps.
**Stack:** React + PowerApps Component Framework (PCF)
**Why it networks:** Positions you as someone who bridges low-code and pro-code. Huge enterprise market (every company using Microsoft 365). You already have the PowerApps context.
**Shareable output:** YouTube tutorial + GitHub template repo

---

### Showcase Projects (Ongoing)

### 7. Open-Source Agentic Development Toolkit
**What:** A lightweight library for building autonomous web agents (like a mini-Browserbase). Agents that can navigate sites, fill forms, extract data, and make decisions.
**Stack:** TypeScript + Playwright + OpenAI + your own orchestration logic
**Why it networks:** Agentic AI is white-hot. Contributing to this space puts you in conversations with top engineers. Your NASA precision + React UX skills = reliable, observable agents.
**Shareable output:** npm package + documentation site + conference talk

### 8. React Component Library for Simulation Visualizations
**What:** A Storybook-hosted library of React components for visualizing simulation data: time-series charts, agent-based grids, network graphs, parameter sliders.
**Stack:** React + D3/Recharts + Storybook + TypeScript
**Why it networks:** Serves a niche (M&S + web dev) that no one else owns. Could become the go-to for simulation engineers who need web UIs. Your IEEE publication background gives credibility.
**Shareable output:** npm package + demo Storybook + "Why simulation needs better UI" blog series

### 9. Personal "Operating System" Dashboard
**What:** A private Next.js app that integrates your life data: travel plans, learning goals, job applications, GitHub activity, health metrics. Uses AI to suggest priorities and surface insights.
**Stack:** Next.js + various APIs + LLM + local-first storage
**Why it networks:** Shows you build tools for your own life. The "quantified self" + "personal AI" angle is trendy. You can share sanitized screenshots and architecture decisions without exposing proprietary work.
**Shareable output:** Architecture blog post + "How I built my own AI assistant" thread

### 9a. Agent OS — Mission Control for Hermes (NEW — July 2026)
**What:** A visual cockpit / agent harness GUI that wraps Hermes Agent with real-time observability and control. Distinct from #9 (which is personal life data) — this is agent infrastructure monitoring. The full vision is a composed dashboard of discrete MVP pieces (see #50-54 below) that can each ship independently and later tie together into a unified mission control interface.
**Stack:** Next.js or Electron + WebSocket + SQLite + Recharts + Hermes APIs
**Why it networks:** Agent observability/management is exploding (LangSmith, Helicone, Langfuse) but nobody has a self-hosted, local-first agent OS dashboard. You've been running Hermes for months with real infrastructure (cron, skills, memory, kanban) — this shows you understand agent systems at the infrastructure level, not just API-calling. The "I built mission control for my AI agent" story is compelling for hiring managers at any AI-focused company.
**Shareable output:** Live demo + "How I built an Agent OS" architecture series + screenshots of the dashboard in action
**Composes from:** #50 (Memory Browser), #51 (Tool Execution Visualizer), #52 (Cron Timeline & Health Monitor), #53 (Session History Browser), #54 (Skill/Plugin Manager)

---

### ⭐55 Hyperfocus Planner (ArcDay) — Productivity Project

**What:** An autonomous AI-powered TO-DO application that ingests long-term goals and objectives, then automatically breaks them down into prioritized daily action items using LLM reasoning and calendar integration.

**Stack:** Next.js 16 + Tailwind4 + shadcn/ui + better-sqlite3 + OpenAI API + Google Calendar OAuth

**Why it's worth it:** This is a practical productivity tool that combines your AI expertise with real workflow automation. Long-term goals don't magically become done — they need systematic decomposition. An AI assistant that handles the heavy lifting of "what should I work on today?" is genuinely useful. The autonomous nature (ingesting goals, creating plans) shows you understand LLM agent patterns: planning, tool use, iterative refinement. Perfect for your own workflow and highly relatable to anyone drowning in strategic objectives.

**Shareable output:** Live demo + "How AI can turn vague goals into daily checklists" case study + GitHub repo with full implementation details

**Key Features:**
- **Goal Ingestion:** Import from text, Notion exports, or manual entry of long-term objectives
- **AI Planning Engine:** Uses LLM to break down goals into milestone → weekly tasks → daily actions hierarchy
- **Dynamic Replanning:** As you complete or reschedule items, AI recalibrates the entire plan forward
- **Calendar Sync:** Google OAuth integration to actually schedule your daily plan blocks
- **Priority Scoring:** AI analyzes urgency vs. importance and surfaces what matters most today
- **Progress Tracking:** Visual progress bars showing goal completion percentage across all active goals

**Skills Gap Filled:** Autonomous planning agents, calendar API integration, hierarchical task decomposition, multi-step LLM workflows with stateful memory

---

## Round 2 Brainstorm (June 2026)

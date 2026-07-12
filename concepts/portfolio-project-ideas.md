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

> New ideas generated after shipping the first 3 portfolio projects (UX Critique Tool, GitHub README Generator, Nomad Cost Dashboard). Organized by what they demonstrate and what skills gaps they fill.

### Category 1: Tools You'd Actually Use

#### 10. AI Meeting Transcript Analyzer
**What:** Upload a Teams/Zoom transcript or paste the text. AI extracts action items, decisions, risks, open questions, and generates a formatted summary + follow-up email draft.
**Stack:** Next.js + OpenAI + structured JSON output + clipboard/copy UX
**Why it's worth it:** Rick is on Teams calls all day at NASA. This is a tool he'd actually use. Shows RAG, NLP, and clean UX for structured output. The "I built this for my own meetings" story is gold on LinkedIn.
**Skills gap filled:** None of the 3 shipped projects show structured document processing or email/template generation.

#### 11. Local LLM Chat Interface (Personality Switcher)
**What:** A polished ChatGPT-style UI that connects to a local Ollama instance. Model picker, streaming responses, conversation history, and a personality/system-preset system that lets users switch between AI personalities (e.g. "Code Reviewer", "Writing Coach", "Devil's Advocate", "Simulation Advisor") — each with its own system prompt, default model, and temperature. Users can create, edit, and save their own personality presets.
**Stack:** Next.js 15 + Ollama API + streaming (SSE) + localStorage
**Why it's worth it:** Rick already has Ollama running on the NUC and BigRickPC. A privacy-first local chat UI is a real tool. Shows streaming (none of the shipped projects stream), model selection UX, and local AI integration. The "runs entirely on your hardware" angle is increasingly relevant. The personality switcher differentiates it from every bootcamp chat clone — mirrors Hermes persona/system-prompt tuning and makes a compelling LinkedIn story: "I built a local AI personality manager because I got tired of rewriting system prompts."
**Skills gap filled:** Streaming UI, local LLM integration, real-time UX, system-prompt management UX.
**Status:** In development — Phase 1: OpenAI planning integration, Google Calendar OAuth

---

### ⭐55 | [Hyperfocus Planner](#55-hyperfocus-planner-arcday) | Productivity | ✅ IN PROGRESS | AI TO-DO list, goal breakdown, daily planning


---

## Implementation Spec: Local LLM Chat Interface (#11)

> Full build spec for the next portfolio project. Designed to be loaded into a fresh Hermes session with the kanban skill for task decomposition and worker dispatch.

### Project: local-llm-chat

**Repo:** rsegrest/local-llm-chat
**Deploy:** Vercel (works with any OpenAI-compatible endpoint via dev proxy; production needs an accessible LLM endpoint)
**Local dev:** Any OpenAI-compatible server — Ollama (localhost:11434, 192.168.1.157:11434), LM Studio (192.168.1.XXX:1234), vLLM, llama.cpp, cloud APIs

> **Architecture decision: OpenAI-compatible API (Option B).** The chat client targets the OpenAI chat completions format (`/v1/chat/completions`, `/v1/models`). This works with Ollama (which exposes `/v1/` alongside its native API), LM Studio, vLLM, llama.cpp server, and any OpenAI-compatible cloud API. One codebase, every backend. No Ollama-specific endpoints — no `/api/chat`, no `/api/tags`, no JSON-line stream conversion. Native SSE throughout.

> **Multi-endpoint support.** Users configure named endpoints (e.g. "NUC Ollama", "BigRickPC LM Studio", "Cloud GLM") with base URL + optional API key. Endpoints are stored in localStorage and selectable from the UI. Each conversation remembers which endpoint it used. This supports Rick's setup: multiple LM Studio instances on different GPU PCs, Ollama on the NUC, and cloud endpoints.

### Architecture Overview

```
local-llm-chat/
├── src/
│   ├── app/
│   │   ├── layout.tsx              # Root layout, dark theme, fonts
│   │   ├── page.tsx                # Main chat view
│   │   └── api/
│   │       ├── chat/route.ts       # OpenAI-compatible /v1/chat/completions proxy with SSE streaming
│   │       └── models/route.ts     # OpenAI-compatible /v1/models proxy (lists available models)
│   ├── components/
│   │   ├── ChatWindow.tsx          # Message list + scroll behavior + streaming display
│   │   ├── ChatInput.tsx           # Text input + send button + keyboard shortcuts
│   │   ├── MessageBubble.tsx       # Individual message (user vs assistant styling)
│   │   ├── ModelPicker.tsx          # Dropdown of available models (fetched from active endpoint)
│   │   ├── EndpointPicker.tsx      # Dropdown of configured endpoints (NUC Ollama, BigRickPC LM Studio, etc.)
│   │   ├── EndpointEditor.tsx      # Modal for adding/editing/deleting endpoint configs
│   │   ├── PersonalityPicker.tsx   # Dropdown/sidebar of personality presets
│   │   ├── PersonalityEditor.tsx    # Modal for creating/editing personality presets
│   │   ├── ConversationSidebar.tsx  # Conversation list (new, rename, delete)
│   │   ├── SettingsBar.tsx          # Temperature slider, endpoint/model/personality pickers
│   │   └── EmptyState.tsx           # Welcome screen with preset suggestions
│   ├── lib/
│   │   ├── llmClient.ts           # OpenAI-compatible API client (fetch wrappers, type defs)
│   │   ├── storage.ts              # localStorage CRUD for conversations + presets + endpoints
│   │   ├── types.ts                # TypeScript interfaces (see below)
│   │   └── defaultPresets.ts       # 5 built-in personality presets + 2 default endpoints
│   └── hooks/
│       ├── useChat.ts              # Chat state + streaming logic
│       ├── useConversations.ts     # Conversation list management
│       ├── usePersonalities.ts     # Personality preset management
│       └── useEndpoints.ts        # Endpoint config management (CRUD, active endpoint)
├── next.config.ts
├── tailwind.config.ts
├── package.json
└── README.md
```

### TypeScript Types (src/lib/types.ts)

```typescript
export interface Message {
  role: 'user' | 'assistant' | 'system';
  content: string;
  timestamp: number;
  model?: string;           // which model generated this (for assistant messages)
  personality?: string;    // which personality was active
  endpointId?: string;      // which endpoint was used (for assistant messages)
}

export interface Conversation {
  id: string;
  title: string;
  messages: Message[];
  createdAt: number;
  updatedAt: number;
  model: string;            // last-used model for this conversation
  endpointId: string;       // which endpoint this conversation uses
  personalityId: string;   // active personality
  temperature: number;
}

export interface Personality {
  id: string;
  name: string;
  emoji: string;            // avatar emoji (simple, no image assets needed)
  systemPrompt: string;
  defaultModel?: string;    // optional model override
  defaultTemperature?: number;
  description: string;      // one-liner shown in picker
  isBuiltIn: boolean;       // built-in vs user-created
}

export interface LLMEndpoint {
  id: string;
  name: string;             // display name (e.g. "NUC Ollama", "BigRickPC LM Studio")
  baseUrl: string;          // e.g. http://localhost:11434/v1, http://192.168.1.157:1234/v1
  apiKey?: string;          // optional — most local servers don't need it
  type: 'ollama' | 'lmstudio' | 'vllm' | 'llamacpp' | 'openai-compatible';  // for UI label/icon
  isDefault: boolean;       // one endpoint is default for new conversations
  isBuiltIn: boolean;       // built-in vs user-created
}

export interface LLMModel {
  id: string;               // model identifier (e.g. "glm-5.2", "qwen3.5-9b")
  name?: string;            // display name if different from id
}
```

### API Routes

> All routes accept an `endpointId` in the request body (or query param) to select which configured endpoint to proxy to. The endpoint's `baseUrl` and optional `apiKey` are looked up from the endpoint config (passed from client localStorage).

**POST /api/chat** (src/app/api/chat/route.ts)
- Accepts: `{ endpointId, model, messages, stream, options: { temperature } }`
- Looks up the endpoint config (baseUrl + apiKey) from the request body
- Proxies to `{endpoint.baseUrl}/chat/completions` (OpenAI-compatible)
- Streams the response back via SSE — pass through the OpenAI SSE stream natively (no format conversion needed)
- Error handling: if endpoint is unreachable, return friendly error JSON

**GET /api/models** (src/app/api/models/route.ts)
- Accepts: `?endpointId=<id>&baseUrl=<url>&apiKey=<key>` (endpoint config passed from client)
- Proxies to `{endpoint.baseUrl}/models` (OpenAI-compatible)
- Returns simplified `{ models: LLMModel[] }`
- Caches for 60 seconds per endpoint (models don't change often)

### Core Hooks

**useChat** (src/hooks/useChat.ts)
- Manages active conversation messages
- `sendMessage(content: string)` — appends user message, calls /api/chat with the conversation's endpointId + model, streams assistant response token-by-token into state
- `isStreaming` state for UI feedback (typing indicator, disable send button)
- `abortController` ref to allow "Stop generating" button
- Error handling: if endpoint is unreachable, show friendly error in chat (not a crash)

**useConversations** (src/hooks/useConversations.ts)
- Load/save conversation list from localStorage
- `createConversation(personalityId, endpointId, model)`, `deleteConversation(id)`, `renameConversation(id, title)`
- Auto-title: first 50 chars of first user message
- Persists on every message append

**usePersonalities** (src/hooks/usePersonalities.ts)
- Load/save personality presets from localStorage
- Built-in presets (isBuiltIn=true) are seeded on first run, user can clone but not delete
- `createPersonality()`, `updatePersonality(id, patch)`, `deletePersonality(id)`
- `clonePersonality(id)` — duplicate a built-in to customize

**useEndpoints** (src/hooks/useEndpoints.ts)
- Load/save endpoint configs from localStorage
- Built-in endpoints seeded on first run (see Default Endpoints below)
- `createEndpoint()`, `updateEndpoint(id, patch)`, `deleteEndpoint(id)`
- `getActiveEndpoint()` — returns the currently-selected endpoint
- `setActiveEndpoint(id)` — switch the active endpoint (affects new messages)
- Cannot delete built-in endpoints (but can edit their URLs)
- Endpoint configs include: name, baseUrl, apiKey (optional), type (ollama/lmstudio/vllm/llamacpp/openai-compatible)

### Built-in Personality Presets (src/lib/defaultPresets.ts)

1. **General Assistant** 🤖 — Default. No system prompt (or minimal "You are a helpful assistant.")
2. **Code Reviewer** 🔍 — "You are a senior code reviewer. Be direct, cite line numbers, flag security issues first. Prefer concise feedback over praise. Use bullet points."
3. **Writing Coach** ✍️ — "You are a supportive writing coach. Suggest specific alternatives rather than just pointing out problems. Explain why a change improves the text. Maintain the author's voice."
4. **Devil's Advocate** 😈 — "You are a rigorous intellectual adversary. Challenge every assumption the user makes. Force them to defend their position. Be respectful but relentless. End with one question they haven't considered."
5. **Simulation Advisor** 📊 — "You are a modeling and simulation expert with a Master's in M&S. Help design simulations: suggest parameters, identify emergent behaviors to watch, recommend visualization approaches. Reference domain concepts (state machines, Monte Carlo, agent-based modeling)."

### Default Endpoints (src/lib/defaultPresets.ts)

Seeded on first run (isBuiltIn=true, editable but not deletable):

1. **NUC Ollama** — `http://localhost:11434/v1` — type: ollama — no API key
2. **BigRickPC Ollama** — `http://192.168.1.157:11434/v1` — type: ollama — no API key

Users add their own endpoints (e.g. LM Studio on GPU PCs, cloud APIs) via the EndpointEditor modal.

### UI Layout

- **Left sidebar** (260px, collapsible): Conversation list with active highlight, "New Chat" button at top
- **Main area**: Chat window (scrollable message bubbles, user right-aligned, assistant left-aligned)
- **Top bar**: Endpoint picker (dropdown), personality picker (dropdown with emoji + name), model picker (dropdown — models fetched from active endpoint), temperature slider (collapsible settings)
- **Bottom**: Chat input (auto-growing textarea, Enter to send, Shift+Enter for newline, Stop button while streaming)
- **Dark theme**: bg #1a1a2e, text #e0e0e0, accent #00d4aa (matches shipped projects and email preferences)
- **Responsive**: Sidebar collapses on mobile, chat fills screen

### Key Behaviors

1. **Streaming**: OpenAI-compatible SSE stream from /v1/chat/completions. API route passes it through natively. useChat hook parses SSE events and appends tokens to the current assistant message in real-time.
2. **Endpoint switching**: Changing endpoint updates the conversation's endpointId. Model picker refreshes to show models available on the new endpoint. Show a subtle divider ("Switched to BigRickPC LM Studio").
3. **Personality switching**: Changing personality mid-conversation injects the new system prompt for the NEXT message (doesn't retroactively change history). Show a subtle divider in the chat ("Switched to Code Reviewer").
4. **Model switching**: Changing model updates the conversation's model. Different models (from the same or different endpoints) can be used within the same conversation.
5. **Persistence**: All conversations, personalities, and endpoints in localStorage. No backend database — this is a local-first tool. Export/import as JSON for backup.
6. **No-auth**: Local tool, no login. If deployed to Vercel, it needs at least one accessible LLM endpoint (cloud API or exposed local server).
7. **Markdown rendering**: Assistant messages render markdown (code blocks with syntax highlighting, lists, bold, headers). Use react-markdown + rehype-highlight.
8. **Code copy buttons**: Each code block gets a "Copy" button in the top-right corner.

### Kanban Task Breakdown (13 tasks)

| # | Task | Depends On | Notes |
|---|------|-------------|-------|
| 1 | Scaffold Next.js 15 + shadcn/ui + Tailwind | — | App Router, TypeScript, dark theme |
| 2 | OpenAI-compatible API client + types (llmClient.ts, types.ts) | 1 | Fetch wrappers for /v1/chat/completions + /v1/models, type defs, LLMEndpoint type |
| 3 | /api/models route + ModelPicker + EndpointPicker | 2 | Proxy to /v1/models, endpoint-aware model listing, endpoint dropdown |
| 4 | /api/chat route with SSE streaming | 2 | Proxy to /v1/chat/completions, pass through OpenAI SSE natively |
| 5 | useChat hook + ChatWindow + MessageBubble | 3,4 | Streaming display, scroll-to-bottom, typing indicator |
| 6 | ChatInput component + keyboard shortcuts | 5 | Auto-grow textarea, Enter to send, Stop button |
| 7 | defaultPresets.ts + usePersonalities hook + PersonalityPicker | 2 | 5 built-in presets, localStorage CRUD, dropdown UI |
| 7a | defaultEndpoints + useEndpoints hook + EndpointEditor modal | 2 | 2 built-in endpoints, localStorage CRUD, endpoint config UI |
| 8 | PersonalityEditor modal | 7 | Create/edit/clone/delete presets, system prompt textarea, model override, temperature |
| 9 | useConversations hook + ConversationSidebar | 5 | Conversation list, new/rename/delete, localStorage persistence, auto-title |
| 10 | SettingsBar (endpoint/model/personality pickers, temperature) | 3,7,7a | Collapsible settings, reflects active conversation state |
| 11 | Markdown rendering + code copy buttons | 5 | react-markdown + rehype-highlight, per-code-block Copy button |
| 12 | README + deploy to Vercel + GitHub repo | 11 | Screenshots, architecture diagram, setup instructions |

### Dependencies (package.json)

- next ^15
- react ^19, react-dom ^19
- tailwindcss ^4
- @shadcn/ui (component lib — use CLI to add components)
- react-markdown + rehype-highlight (markdown rendering)
- lucide-react (icons — comes with shadcn)

### Environment

Endpoints are configured in the UI (stored in localStorage), not env vars. For development/seed purposes:

- **NUC Ollama**: `http://localhost:11434/v1` (no API key)
- **BigRickPC Ollama**: `http://192.168.1.157:11434/v1` (no API key)
- **LM Studio (any GPU PC)**: `http://192.168.1.XXX:1234/v1` (no API key)
- **Cloud APIs**: `https://api.example.com/v1` (with API key)

All endpoints use the OpenAI-compatible API format (`/v1/chat/completions`, `/v1/models`).

### LinkedIn Post Angle

"I built a local AI personality manager. Instead of rewriting system prompts every time I wanted a different AI persona — code reviewer, writing coach, devil's advocate — I built a chat UI that lets me switch personalities with a dropdown. It talks to any OpenAI-compatible backend — Ollama, LM Studio, vLLM, cloud APIs — so I can point it at any of my GPU PCs or cloud endpoints. Runs entirely on my own hardware. No API keys, no monthly fees, no data leaving my network. Open source — try it with your own local model."

#### 12. AI-Powered Obsidian Wiki Explorer
**What:** Visual graph of wiki pages with AI semantic search — "find pages about cost-of-living in Southeast Asia" returns results by meaning, not keyword. Plus "what should I read next" recommendations.
**Stack:** React + D3/cytoscape graph + Ollama embeddings + SQLite
**Why it's worth it:** Rick is already building wikis (3 vaults). This shows he can build tools around his own workflow. Graph visualization + semantic search is a rare combo. Nobody else has "AI-powered Obsidian explorer" in their portfolio.
**Skills gap filled:** Graph/network visualization, embeddings, vector search.

### Category 2: Viral / Attention-Getters

#### 13. "Roast My Landing Page"
**What:** Paste a URL, the app takes a screenshot, AI delivers a brutal-but-funny UX critique in the voice of a sarcastic design critic. Rate limit to prevent abuse. Shareable roast cards with the screenshot + top 3 burns.
**Stack:** Next.js + Playwright (screenshot) + Vision API + shareable card generation
**Why it's worth it:** The UX Critique Tool is professional and B2B. This is the viral B2C version. "My AI roasted your landing page" is inherently shareable. Shows browser automation + vision + personality-driven prompt engineering. Could go viral on X/Reddit.
**Skills gap filled:** Browser automation, shareable content generation, humor in prompts.

#### 14. AI Agent Sandbox
**What:** A visual playground where you watch AI agents interact in real time. Agents navigate a simple web environment, solve puzzles, trade resources, or cooperate on tasks. You can tweak their system prompts and watch behavior change.
**Stack:** React + WebSocket + LLM function calling + canvas/grid visualization
**Why it's worth it:** Agent orchestration is the hottest space in AI right now. A visual, interactive agent simulator is rare — most agent demos are terminal-based and boring. This shows multi-agent coordination, real-time UI, and function calling. Defense-tech companies (Anduril, Palantir) would drool over this.
**Skills gap filled:** Multi-agent orchestration, real-time UI, function calling, WebSocket streaming.

#### 15. Interactive "Explain This Codebase" Explorer
**What:** Paste a GitHub repo URL. AI reads the code, generates an interactive visual breakdown — architecture diagram, key files, data flow, entry points. Click any node to see AI explanation of that module.
**Stack:** Next.js + GitHub API + LLM + interactive graph viz (react-flow or d3)
**Why it's worth it:** Every developer has stared at an unfamiliar codebase wishing someone would explain it. This solves a real pain point. Network effect — people share it when their repo gets explained. Shows: code understanding, graph visualization, GitHub API.
**Skills gap filled:** Code analysis, interactive graph UX, large-context LLM usage.

### Category 3: Career-Signal Pieces

#### 16. Budget Proposal Estimator (Non-Proprietary)
**What:** Input project parameters (scope, team size, timeline, complexity), AI suggests cost breakdown, risk factors, and timeline with confidence intervals. Not the NASA app — a clean, public version.
**Stack:** Next.js + shadcn forms + LLM + Recharts for cost visualization
**Why it's worth it:** Rick is literally building a proposal/budget app at work with "potential six-figure savings." This lets him tell that story without revealing proprietary details. Shows: complex form UX, domain expertise, AI + finance. Hiring managers who see this will ask about the real version — and he can talk about the impact.
**Skills gap filled:** Complex form UX, financial data visualization, domain expertise demonstration.

#### 17. Electron + AI Desktop App Template
**What:** Open-source starter template showing how to integrate AI into an Electron + React + TypeScript desktop app. Include streaming chat, system tray, local file access, and AI-powered search.
**Stack:** Electron + React + TypeScript + Ollama/OpenAI + Tailwind
**Why it's worth it:** Rick is building exactly this at work but can't show it. A clean open-source template version is shareable and proves the skill. Electron + AI is a niche almost nobody has portfolio pieces for. Enterprise companies building desktop AI tools would notice.
**Skills gap filled:** Electron, desktop AI, system integration. Directly mirrors the current work project.

#### 18. AI Code Review Dashboard
**What:** Paste a GitHub PR URL or upload a diff. AI reviews the code with structured feedback: security issues, performance, style, bugs, suggestions. Interactive diff viewer with inline AI comments.
**Stack:** Next.js + GitHub API + LLM + diff viewer (react-diff-viewer)
**Why it's worth it:** Code review tooling is booming (CodeRabbit, etc.). Building your own shows deep understanding of code quality, security, and developer tooling. Useful for own repos. Shows: GitHub API, code analysis, diff UX.
**Skills gap filled:** Code analysis, security awareness, developer tooling UX.

### Category 4: The M&S Anchor

#### 19. Digital Twin of a Simple System
**What:** Interactive simulation of a real-world system (traffic flow, coffee shop queue, supply chain). Users tweak parameters and watch emergent behavior. An AI agent "optimizes" the system and explains its strategy.
**Stack:** React canvas/SVG + state machine + LLM advisor
**Why it's worth it:** The strongest M&S piece. Directly leverages Rick's Master's degree. "Digital twin" is defense-industry language. Bridges NASA world with React/AI world. No other web developer has an M&S degree — this is the moat.
**Skills gap filled:** M&S demonstration, canvas/SVG animation, simulation visualization.

---

## Round 3 Brainstorm (June 2026)

> 15 more ideas pushing into new territory: simulation/M&S depth, AI safety/observability, data+AI, creative/generative, and practical life tools.

### Category 5: Simulation & M&S (your moat)

#### 20. Monte Carlo Retirement Planner
**What:** Input your salary, savings rate, investment mix, expected Social Security, and the simulator runs 10,000 trials with market volatility + inflation randomness. Visualize outcomes as a probability distribution — "87% chance you hit $2M by 65." Let users drag sliders and watch the distribution shift in real time.
**Stack:** React + D3 histogram + Web Worker (for the Monte Carlo loop) + Tailwind
**Why it's worth it:** Personal finance + simulation + interactive viz is a potent combo. Rick would actually use this for his own retirement planning. Every dev knows Monte Carlo conceptually but almost none can build an interactive one. Shows statistical thinking, Web Workers for performance, and data viz.
**Skills gap filled:** Statistical simulation, probability distributions, Web Worker performance.

#### 21. Agent-Based Epidemic Simulator
**What:** A grid-based simulation where each cell is a person with health state (SIR model — Susceptible, Infected, Recovered). Users tweak transmission rate, recovery time, mobility. Watch waves propagate in real time. AI agent suggests intervention strategies ("lock down at 30% infection to flatten the curve").
**Stack:** React canvas + state machine + LLM advisor + Recharts for time-series
**Why it's worth it:** Directly uses M&S coursework. Epidemic modeling is universally understood post-COVID. The AI advisor layer turns it from a toy into an intelligent tool. Defense/government orgs (DARPA, BARDA, FEMA) use exactly this kind of modeling. Shows: agent-based modeling, real-time simulation, public health domain awareness.
**Skills gap filled:** Agent-based modeling, SIR models, real-time canvas animation.

#### 22. Queueing Theory Visualizer
**What:** Visual simulation of different queue configurations — single server, multi-server, priority queue, round-robin. Show Little's Law in action. Users add/remove servers and watch wait times change. AI explains the math and recommends optimal configuration.
**Stack:** React + animated SVG + state machine + LLM
**Why it's worth it:** Queueing theory is used in everything from call centers to DevOps to ER triage. A visual, interactive tool for it doesn't exist as a polished web app. Niche but deeply useful. Shows: operations research, real-time animation, mathematical visualization.
**Skills gap filled:** Operations research, animated SVG, mathematical UX.

### Category 6: AI Safety / Trust / Observability

#### 23. AI Hallucination Detector
**What:** Paste text + a source document. AI checks each claim against the source and flags unsupported statements with confidence scores. Color-coded output: green (supported), yellow (partially supported), red (unsupported/hallucinated).
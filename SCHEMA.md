# Wiki Schema

## Domain
Career advancement for a full-stack web application developer specializing in UX, React front-end, AI/Agentic Development, with a Master's in Modeling & Simulation.

Topics: skill acquisition, portfolio building, resume/LinkedIn optimization, job market intelligence, interview prep, personal branding, open-source contributions, side projects, conference talks, certifications, networking.

## File Types

### `entities/`
People, organizations, companies, technologies, tools, frameworks, certifications, conferences.

### `concepts/`
Topics: React patterns, agentic AI architectures, UX heuristics, system design, M&S fundamentals, career pivots, salary negotiation, behavioral interview techniques.

### `comparisons/`
Side-by-side: React vs Vue vs Angular, job offer A vs B, AI frameworks, portfolio platform choices, resume formats.

### `queries/`
Filed answers worth keeping: "How do I price freelance AI work?", "What should a senior React dev know in 2026?"

### `raw/`
Immutable source material — job postings scraped, LinkedIn posts saved, GitHub repo READMEs, course syllabi, conference talk transcripts, resume drafts, portfolio screenshots.

## Tag Taxonomy

**Role:** full-stack, frontend, backend, ux-designer, ai-engineer, agent-developer, consultant, freelancer, staff-engineer, principal-engineer, engineering-manager

**Technology:** react, typescript, nodejs, python, nextjs, tailwind, graphql, aws, docker, kubernetes, openai, anthropic, langchain, langgraph, fastapi, postgres, redis, websocket, webassembly

**Concept:** system-design, ux-research, accessibility, performance-optimization, state-management, api-design, testing, ci-cd, prompt-engineering, rag, fine-tuning, mcp, agent-orchestration, simulation, digital-twin

**Career:** job-search, interview, salary-negotiation, resume, linkedin, portfolio, networking, mentorship, conference, certification, side-project, open-source, freelance, consulting, promotion, pivot

**Artifact:** resume, cover-letter, github-repo, case-study, blog-post, talk-slides, video-demo, design-system, architecture-doc, proof-of-concept, white-paper

**Market:** startup, enterprise, faang, remote, hybrid, govcon, defense, fintech, healthtech, edtech, climate-tech

## Conventions

### Frontmatter
```yaml
---
title: "Page Title"
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | comparison | query
tags: [tag1, tag2]
sources: [raw/articles/source.md]
status: draft | review | published | archived
---
```

### Links
- Wikilinks: `[[page-name]]` — for wiki cross-references
- External: `[text](url)` — for external URLs
- Citations: `^[raw/articles/source.md]` — provenance on claims

### Provenance
Every job posting analysis, salary data point, or interview experience must cite its raw source.

### Naming
- `entities/jane-doe.md` — people
- `entities/google.md` — organizations
- `concepts/react-server-components.md` — topics
- `comparisons/job-offer-a-vs-b.md` — decisions
- `queries/senior-react-salary-2026.md` — filed answers

### Review Threshold
- Pages > 5,000 words: split or summarize
- Topics > 10 sub-pages: create hub page

### Log Rotation
When `log.md` exceeds 500 entries, rename to `log-YYYY.md` and start fresh.

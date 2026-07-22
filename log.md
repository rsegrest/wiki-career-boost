# Wiki Log

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> When this file exceeds 500 entries, rotate: rename to log-YYYY.md, start fresh.

## [2026-05-30] create | Career wiki initialized
- Domain: Career advancement for full-stack web developer (React, UX, AI/Agentic, M&S)
- Structure created with SCHEMA.md, index.md, log.md
- Categories: Role, Technology, Concept, Career, Artifact, Market
## [2026-05-30] create | Seed professional profile
- Created entities/rick-segrest-pro.md
- Full-stack developer profile with React, UX, AI/Agentic, M&S focus
- Documented skills, artifacts, career goals, target markets, known gaps
- Updated index.md — Total pages: 1

## [2026-05-30] ingest | LinkedIn profile
- Source: https://www.linkedin.com/in/ricksegrest
- Extracted: headline, about, posts, certifications, publications, projects
- Raw: raw/articles/linkedin-ricksegrest-2026.md
- Updated entities/rick-segrest-pro.md with LinkedIn data
- Created entities/amentum.md (current employer)
- Created entities/uah.md (alma mater)
- Discovered: 4 LinkedIn certifications (AI, XAI, Python DS, 2020)
- Discovered: 6 publications (game engines, VoIP, journalism)
- Discovered: Dyreqt-as-a-Service project (Mar 2022)
- Updated index.md — Total pages: 3

## [2026-05-30] update | Profile corrections from user input
- Corrected employment: Rick works AT NASA (7+ years) via Amentum staffing contract, not FOR Amentum directly
- Added clearance status: Previously Secret, now dormant (not needed at NASA)
- Added current team tech: Microsoft PowerApps (new stack, just started)
- Added low-code/no-code to skills and target markets
- Corrected NASA entity: entities/nasa.md created
- Updated entities/amentum.md: staffing contractor, not direct employer
- User noted: VoIP publications are an interesting branding angle
- Updated index.md — Total pages: 4

## [2026-05-30] create | Portfolio project ideas concept
- Created concepts/portfolio-project-ideas.md
- 9 project ideas across Quick Wins (1–3 weekends), Medium (2–4 weeks), Showcase (ongoing)
- Each chosen for maximum LinkedIn/GitHub/meetup conversation potential
- Key themes: React + M&S + AI triad, NASA pedigree, UX expertise, PowerApps bridge
- Recommended sequence: GitHub README Generator → AI UX Critique → Digital Twin → Open Source
- Updated index.md — Total pages: 5

## [2026-05-30] create | Kanban boards for portfolio projects
- Created kanban/ directory for project tracking
- Created kanban/portfolio-kanban-hub.md — Hub page with deadline, decision matrix, daily standup template
- Created kanban/github-readme-generator.md — 12 tasks, P0/P1/P2 priorities, 8–16hr budget
- Created kanban/ai-ux-critique-tool.md — 12 tasks, tech stack, blockers identified
- Created kanban/nomad-cost-dashboard.md — 12 tasks, data export strategy
- Recommendation: Pick ONE project to ship before June 5; 6 days = 12–24 hours available
- Updated index.md — Total pages: 9

## [2026-06-22] update | Compensation, position context, and organizational risks
- Updated entities/rick-segrest-pro.md with full compensation/benefits table and current position context
- Updated entities/amentum.md with ESSCA contract status, insourcing pressure, growth ceiling
- Updated entities/nasa.md with insourcing initiative and current project details
- Key facts added:
  - Salary: $170K (from $135K in 2019), raises below inflation
  - Leave: 172 hrs/yr, 401(k) ~50% of 6%, health via wife's plan
  - Lateral move to new group — better environment, older/professional team
  - Building proposal/budget planning app (potential "six-figure" impact)
  - Previous group: stressful, lost both parents in 18 months, took 6mo leave, callous customer
  - ESSCA contract up for re-bid — rate adjustment possible
  - NASA insourcing initiative — Rick does NOT want gov employment
  - Amentum growth ceiling — limited advancement opportunity
- Preparation for comparisons/career-move-vs-side-hustle-vs-maximize-current.md

## [2026-06-22] update | Salary correction, remote work, ESSCA timeline, benefits portability
- Corrected starting salary: $130K + $5K signing bonus (not $135K)
- Year 2: <3% raise, actually earned LESS after bonus
- Annual bonuses: $200–300/yr pittance at contract year end (March)
- 401(k) match confirmed at ~50% of 6% ≈ $5,100/yr; balance portable if leaving
- Health insurance via wife's plan — portable, not tied to Amentum
- Remote work: ~50%, non-negotiable for family; previous group pushed back illegally
- ESSCA proposals due 11 March 2026 — award expected imminently
- NASA insourcing: general initiative, no direct communication about Rick's position
- Current app: Electron+React+TypeScript+Dataverse via pacx (transferable skills)
- All three entity pages updated with refined details

## [2026-06-22] create | Three-way career comparison page
- Created comparisons/career-move-vs-side-hustle-vs-maximize-current.md
- 18.7KB comprehensive analysis covering:
  - Path A: Maximize Current (stay, ship app, leverage ESSCA II)
  - Path B: Career Move (new employer, React+AI intersection)
  - Path C: Side-Hustle (freelance while keeping $170K day job)
  - ESSCA II award variable (3 scenarios)
  - Risk matrix, income calculations, decision framework
  - Recommended A+C hybrid strategy with B preparation
  - 7 open questions for follow-up
- Updated index.md — Total pages: 10
- Added ESSCA II award date: 30 September 2026 (user confirmed)
- Amentum likely to retain contract per Rick's assessment

## [2026-06-22] ingest | ESSCA II RFP documents from SAM.gov
- Source: /home/rick/essca_rfp/ (17 files — RFP sections, amendments, pricing model, Q&A)
- Created queries/essca-ii-rfp-analysis.md
- Key findings:
  - Contract: $3.248B max, 8.5 years, single-award IDIQ
  - ERI benchmark rates extracted for all ES levels at MSFC
  - Rick at $81.42/hr vs ES-8 benchmark $84.46/hr — ~$6K below benchmark
  - RFP includes escalation rates for CY2027-2035 (typically 3-4%/yr)
  - RFP requires offerors to address compensation gaps for incumbent retention
  - NASA evaluates workforce compensation as a proposal subfactor
  - Incumbent rates (L-5-A) are controlled attachments — not downloaded
- Updated index.md — Total pages: 11
- This is a MAJOR data source for the career comparison page

## [2026-06-22] ingest | Remote React+AI job market salary research
- Created queries/react-ai-job-market-salary-2026.md
- Sources: Levels.fyi, Glassdoor, Indeed, ZipRecruiter, Built In, Upwork, Toptal, Contra
- Key findings:
  - Rick is underpaid by $20K-$50K vs market for React+AI skills
  - Senior Full-Stack + AI (remote): $180K-$220K base
  - AI Engineer w/ full-stack (remote): $200K-$250K base
  - Staff Engineer + AI (remote): $210K-$280K base, $280K-$450K TC
  - Freelance React+AI: $120-$175/hr realistic for Rick
  - "AI Engineer" title carries 15-25% premium over "Senior Full-Stack"
  - NASA experience valued at defense-tech (Anduril, Palantir) — 10-15% premium
  - 30+ companies hiring for React+AI intersection (listed in report)
- Updated index.md — Total pages: 12

## [2026-06-22] create | Freelance acquisition & portfolio strategy
- Created concepts/freelance-portfolio-strategy.md
- Key additions:
  - UX team experience positioning (Full-Stack Product Engineer, AI UX Engineer)
  - Toptal closed — Contra/Upwork/Wellfound/direct outreach ranked alternatives
  - 4-week acquisition playbook (profiles, bids, outreach, momentum)
  - Productized service packages ($3K-$25K fixed-price)
  - Portfolio build priority: UX Critique Tool first, Resume Optimizer second
  - Same portfolio serves both freelance AND salaried job applications
  - Updated rick-segrest-pro.md — added UX team experience as differentiator
## [2026-06-22] update | AI UX Critique Tool kanban board created in Hermes
- Created 10 live Hermes Kanban tasks (t_e0339420 through t_069bff13)
- Task graph: T1 scaffold -> T2 upload + T3 prompt (parallel) -> T4 API -> T5 UI -> T6 overlay -> T7 examples -> T8 deploy -> T9 README -> T10 LinkedIn
- T1 (scaffold) immediately picked up by dispatcher — running
- Updated wiki kanban page with live task IDs and refined plan
- Added bounding box overlay as killer feature (not in original May plan)
- Added Vercel AI SDK for model-agnostic support (OpenAI + Anthropic)
- Updated index.md — Total pages: 13

## [2026-06-23] ingest | NASA civil service GS pay research
- Created queries/nasa-civil-service-gs-pay.md
- Key findings:
  - Rick would enter at GS-13 (Step 5-10) or GS-14 (Step 1-3)
  - GS-13 Step 10: $153K — $17K below current $170K
  - GS-14 Step 10: $181K — only $11K above, takes 10+ years to reach
  - GS pay cap: ~$183K (2025), ~$192K (2026 projected)
  - FERS pension requires 20+ years to be meaningful
  - Rick is 49 — starting now means pension doesn't vest meaningfully until age 69
  - 20 years x $25K/yr pay cut = $500K lost salary for $37K/yr pension starting at 69
  - Break-even at age 82+ — terrible trade
  - Confirmed: NASA civil service makes no sense for Rick
- Updated index.md — Total pages: 14

## [2026-06-24] update | Portfolio project ideas — Round 4 brainstorm

- Added 15 new ideas (35-49) to concepts/portfolio-project-ideas.md
- Categories: Gov/Defense (35-37), Dev Infrastructure (38-40), Accessibility (41-43), Content/Knowledge (44-46), Education (47-49)
- Updated idea index table — now 49 ideas total
- Updated build priority list with all 49 ideas
- All 4 rounds documented with sources

- Updated concepts/portfolio-project-ideas.md with 25 new ideas (10-34)
- Added linked idea index table at top of page (34 ideas, status, skills)
- Marked ideas 1-3 as SHIPPED in the index
- Round 2 (10-19): Tools you'd use, viral, career-signal, M&S anchor
- Round 3 (20-34): M&S depth (Monte Carlo, epidemic sim, queueing), AI safety (hallucination detector, prompt versioning, audit trail), data+AI (NL-SQL, API explorer, spreadsheet formulas), creative (storyboard, color palette, music mood board), life tools (meal planner, ESA tracker, family calendar)
- Updated build priority with all 34 ideas ranked
- Updated index.md — Total pages: 14

## [2026-06-24] update | All kanban wiki pages synced to Hermes board state

- All 3 portfolio projects now show as SHIPPED in the career wiki
- kanban/ai-ux-critique-tool.md:
  - Updated date to 2026-06-24
  - Checked all 6 success criteria boxes (was all unchecked)
  - Clarified LinkedIn post is drafted, pending Rick's approval
- kanban/github-readme-generator.md:
  - Complete rewrite from stale backlog-only page to shipped status
  - Added all 12 Hermes task IDs (t_9d15bbcf through t_a35d9a79)
  - 11 done, 1 archived (social sharing — per no-auto-post rule)
  - Checked success criteria, noted LinkedIn draft pending approval
- kanban/nomad-cost-dashboard.md:
  - Complete rewrite from stale backlog-only page to shipped status
  - Added all 12 Hermes task IDs (t_9c7ed77f through t_419f85cf)
  - 11 done, 1 archived ("Rick's visited" badge — not worth the effort)
  - Checked success criteria, noted LinkedIn draft pending approval
- kanban/portfolio-kanban-hub.md:
  - Updated project table: all 3 now show as Shipped
  - Updated ship checklist: 4/6 items checked (deploy, repo, README, LinkedIn draft done; posting + portfolio site pending)
  - Added per-project shipped summaries with features and archived task reasons
  - Added 3 new log entries (GitHub README shipped, Nomad Dashboard shipped, wiki pages synced)
- Updated index.md — kanban board descriptions now show shipped status

## [2026-06-25] create | Sabrina Ramonov AI business & career video summaries

- Created concepts/sabrina-ramonov-ai-business-videos.md
- Source: 41 career/business-focused videos from @sabrina_ramonov (Dec 2025 – Jun 2026)
- Key themes: 1-person AI business models, income streams, personal branding (0→3M followers), AI skills for career advancement, industry commentary (AI layoffs, job market)
- Cross-references: career-move-vs-side-hustle-vs-maximize-current, freelance-portfolio-strategy, react-ai-job-market-salary-2026
- Companion tech wiki page: wiki-tech/concepts/sabrina-ramonov-ai-tools-videos.md
- Updated index.md — Total pages: 15

## [2026-06-26] create | Wife's SLP compensation analysis and career options

- Created entities/wife-slp-profile.md — CCC-SLP profile, compensation, benefits, work environment
- Created entities/restore-therapy-services.md — Company profile, ratings, compensation patterns, PTO/scheduling issues
- Created queries/slp-compensation-analysis-2026.md — Full market research: pay comparison, leave comparison, 6 career options ranked
- Key findings:
  - Wife at $35/hr is $7-8/hr below Huntsville/Madison market avg ($42-43/hr)
  - $15-35K below national medians (ASHA SNF $105.5K, BLS $95.4K)
  - Expected ~20% CCC raise did not materialize — consistent with Restore's no-raise pattern (8+ yrs per reviews)
  - 80 hrs PTO/yr below market (typical 10-15 days + separate sick)
  - Restore forces PTO for census gaps, only 4 paid holidays
  - Top options: teletherapy ($45-52/hr remote), hospital ($100K+), competing offer to negotiate, PRN side work, school system
  - Teletherapy confirmed viable in AL: 37 remote openings, VocoVision/Soliant actively recruiting
- Updated index.md — Total pages: 18
- Email with full analysis sent to rsegrest77@gmail.com

## [2026-07-02] update | Portfolio project ideas — Round 5 (Agent OS MVP series)

- Reframed #9: kept Personal OS Dashboard, added #9a Agent OS Mission Control as separate idea
- Added 5 new Agent OS MVP ideas (#50-54): Memory Browser, Tool Execution Visualizer, Cron Timeline, Session History Browser, Skill/Plugin Manager
- Each MVP ships independently, composes into #9a Agent OS dashboard later
- Updated idea index (now 54+9a ideas), build priority, sources
- File: wiki-career/concepts/portfolio-project-ideas.md


## [2026-07-11] update | Agent OS portfolio status
- Updated portfolio-project-ideas.md with current build status
- #50 Memory Browser: DONE (port 3001)
- #51 Tool Visualizer: DONE (port 3004, polling)
- #52 Cron Monitor: DONE (port 3002, + job CRUD)
- #53 Session Browser: DONE (port 3003, FTS5)
- #54 Skill/Plugin Manager: NOT STARTED
- #9a Mission Control: NOT STARTED
- Build pattern documented: Hermes scaffolds + CLAUDE.md -> Claude Code sonnet builds -> Hermes verifies
- Font updated across all 5 projects: Geist + system-ui sans-serif

## [2026-07-20] update | Active build models + status on portfolio master list
- Added section **Active build status & models used** to concepts/portfolio-project-ideas.md
- Audited Hermes state.db + git attributions for Personal Site and Mission Control
- #9a Mission Control: IN PROGRESS :3006 — T1/T2 done, T3 hold; models: Claude Opus 4.8, Sonnet 5, glm-5.2, DeepSeek V4 Flash/Pro
- #56 Personal Site (agent-portfolio-gallery): added to index — IN PROGRESS :3010; models: DeepSeek V4 Pro/Flash, early HY3 (+ Gemini Flash)
- Documented Tier 3 hold + Kanban/TODO + wiki viewer tied to Mission Control
- Cross-linked day-to-day plans at ~/wiki-personal/concepts/project-plans-index.md

## [2026-07-20] update | Writing stack + Phase 1 model map on master list
- Extended portfolio-project-ideas.md models section: Phase 1 leftovers → model table; writing/editing stack (GLM-5.2, Grok 4.5, humanizer)
- Linked personal wiki concepts/writing-voice-and-models.md for gold-sample voice calibration
- Note: Gemini not for this work; Flash not for publishable prose; don't pinch pennies on launch copy

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
  - ⚠️ **Corrected 2026-10-11:** low-code/Power Apps is **capability, not a target market** —
    Rick dislikes the work, gov tenants limit it, and AI features there raise IA problems. Never pitch it.
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
  - ⚠️ **Corrected 2026-10-11:** that was the RFP's *expected* award date. The performance
    start has since slipped to **~May 2027** with **ESSCA I extended** to bridge the gap —
    see `queries/essca-ii-rfp-analysis.md` and the banner on the career comparison page.
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
- 2026-10-04: Added a cross-vault Goals pointer to index.md → personal vault concepts/goals-pay-debt-house-remote-abroad.
  Reframes this vault portfolio/freelance work as the instrument for goal 3a (location-independent income):
  contract income needs no employer permission, so it is the version of work-from-anywhere that does not
  depend on the ~50%-remote day job or the unresolved NASA/ITAR foreign-work-location question.

## [2026-10-11] create | concepts/rcca-app-venture.md — the RCCA app assessed as a venture

- **New page** `concepts/rcca-app-venture.md`: a **Teledyne Brown** friend's **Root Cause Corrective
  Action** tool, already prototyped by Rick — assessed as a money-making asset rather than only a
  build. Companion to Path C and to the personal vault's near-term income plan.
- **Methodology is public, not proprietary** — DO IT² is published (Duke Okes, *Root Cause Analysis*,
  ASQ Quality Press 2009, Appendix B guide + worksheet) and Curtiss-Wright publishes an RCCA supplier
  guideline with the same spine. **No licence needed, but also no moat in the method** — the moat has
  to be the guided cause-tree reasoning UX the prototype already implements.
- **⚠️ Gating legal question:** the v0.3 requirements *document* was written by the friend inside an
  employer context → **written ownership/permission answer required before any commercial use**.
- **Compliance gate checked 2026-10-11:** **CMMC Phase 2 suspended 13 July 2026** (DoW CIO, 60-day
  review of structure/cost/assessment model; the C3PAO L2 and DIBCAC L3 assessments had been due to
  take effect **10 Nov 2026**) — while **Level 1/2 self-assessments and the whole of DFARS
  252.204-7012 / NIST SP 800-171 Rev 2 / SPRS still stand**. The binding requirement for a hosted app
  is **DFARS 7012 (D): an external cloud service provider needs FedRAMP-Moderate-equivalent security**
  → the cheap viable posture is a **no-CUI deployment**, which keeps FedRAMP off the critical path.
  The spec's own **CMP-006** already refuses to claim CUI hosting just because STIG-style config is
  supported; hold that line.
- **Monetization ranked by time-to-first-dollar:** paid pilot at the friend's org ($10–25K) →
  productized RCCA engagement ($15–50K) → workshop/training ($2–8K) → SaaS at ~$199/mo/site
  (12–24 months; **do not start before a pilot pays**).
- **Prototype verified on disk:** 279-row converted baseline (270 reqs: Must 212/Should 57/Could 1),
  62 source files ~9,500 lines, **114 tests, 0 type errors, 21 defects / 0 open**, running under
  systemd user units on port 4180 + cloudflared tunnel. Not in version control.
- **Open questions recorded:** document ownership; whether the friend's employer would actually *buy*
  it; whether the friend can be publicly named; the no-CUI assumption itself (does a quality org want
  nonconformance reports attached to technical drawings?); and how far the prototype is from a v1 a
  stranger could buy.
- Cross-linked: personal vault `concepts/near-term-income-plan`, Path C comparison, and the
  $120–175/hr band from `queries/react-ai-job-market-salary-2026`.

## [2026-10-11] correction | ESSCA II schedule superseded — the raise lever re-derived

**Rick's direct input: the ESSCA II performance start is delayed to ~May 2027, and ESSCA I has been
extended to fill the gap.** The "phase-in window Oct 2026 – Jan 2027" this vault had been planning
against was the RFP's *planned* schedule (captured 2026-06-22), and the 30 Sep 2026 award date was an
*expected* date that later pages — including a wiki-personal page written today — hardened into fact.

Swept and corrected in one pass:
- `queries/essca-ii-rfp-analysis.md` — schedule-status block; timeline, insourcing context, sources
- `comparisons/career-move-vs-side-hustle-vs-maximize-current.md` — revision banner + 10 date fixes
  (Key Actions, timing risk, the ESSCA II Variable, recommended-strategy phases, open questions)
- `wiki-personal/concepts/near-term-income-plan.md` — lever re-ranked #1 → #4; "this lever expires"
  retracted; ES-8-vs-ES-7 classification called out as the contingency it is
- `wiki-personal/concepts/goals-pay-debt-house-remote-abroad.md` + `long-term-projects-tracker.md` (FI-005)
- **New open question:** whether the award itself has been made — unconfirmed as of 2026-10-11

Also fixed a derived-figure inconsistency on the RFP page: the annual ERI delta appears as $6,165
(rounded annuals), $6,323 (3.04 × 2,080) or $6,352 (2,088). The page now says to quote the **hourly**
delta and state the hours basis.

## [2026-10-11] update | RCCA is a partnership — the gate moves to the friend's employment agreement

Rick: **he and the friend are starting a business together; both own the requirements and the
prototype; the plan is to build on spec.** `concepts/rcca-app-venture.md` revised accordingly —
§1 structure + co-founder row; **§3 rewritten** (the live legal question is now the *friend's*
employment agreement, not ownership between the partners); §6 split arithmetic ($10–25K pilot →
$5–12.5K to Rick at 50/50) and on-spec economics; §7 risk rows (employment agreement; on-spec, no
revenue until a sale); §8 gating questions; open questions marked answered/added.

## [2026-10-11] maintenance | normalized bare wikilinks to explicit `[[dir/page]]` form
- Sweep across all four vaults: **45 links** rewritten from bare names (which resolve only by
  Obsidian name-matching) to explicit paths. Form-only change; display text unchanged.
- Also made **0 directory-index links** resolvable (`[[wiki-tech/hermes-agent/index|hermes-agent]]` → `[[hermes-agent/index|hermes-agent]]`).
- Remaining dangling links are **pre-existing** and need a content decision, not a form fix:
  ~229 point at pages that exist nowhere (tool names, dated cross-references in the auto-generated
  x-monitor pages). The x-monitor ones will recur unless the generator emits explicit links.

## [2026-10-11] create | concepts/freelance-outreach-targets.md

Fulfils the Path C checklist item "identify 10 local/regional companies" (now checked off on
[[concepts/freelance-portfolio-strategy]]). Ten targets ordered by **conversion x rate**, in three tiers:
warm network (the LinkedIn "moved commercial" sweep, ex-colleagues with budgets, referral partners incl.
MSPs), the verified local SMB ecosystem (Huntsville/Madison Chamber — Ashley Engles-Ross 256-535-2043;
Catalyst Center 256-428-8190; UAH I2C 256.824.6058; UAH SBDC 256-824-7232), and product companies plus
the AI/agent community where the arcade-skill launch does the persuading.

**Rate correction recorded on the strategy page too:** marketplace medians for AI/automation work are
**~$27-30/hr** with Upwork now charging a 0-15% variable fee, so platforms are discovery/credibility and
the $120-175/hr band only exists in direct relationships. That reorders the plan: the outreach list is the
rate-critical path, not an optional extra.

## [2026-10-11] update | Metro analysis added to the outreach page

Rick asked whether the ~100-mile metros (Nashville, Birmingham, Chattanooga) and ~250-mile metros
(Atlanta, Memphis, Knoxville, Louisville, Montgomery, Auburn) are better markets than defence-heavy
Huntsville. Analysis added to [[concepts/freelance-outreach-targets]]:

- **The defence problem is sector-shaped, not city-shaped** — what varies by metro is the ratio of
  commercial, document-heavy employers, so the selection criterion is sector density x competition x
  drivability, not distance.
- **Ranked:** Birmingham primary (UAB ~$12.1B impact, Regions/Protective HQs, lower competition);
  Chattanooga second (logistics + insurance + gigabit/quantum startup scene, low competition);
  Nashville rich but competitive and best reached via associations; Atlanta deepest competition;
  Memphis/Louisville worth one conference each; **Knoxville (ORNL = DOE) and Montgomery (state gov)
  skipped as the same government-buyer problem**; Auburn is a warm channel, not a market.
- **Multiplier:** two regional industry-association memberships beat ten cities of directory prospecting.

## [2026-10-11] update | Market choice: Chattanooga primary; Auburn upgraded; Birmingham demoted

Rick picked **Chattanooga** (tech-oriented, high-growth, and he wants to visit), and corrected the Auburn
assessment — verified: Auburn Research Park's **77-acre expansion was approved June 2026** (240+ acres total)
with a **45-acre Advanced Manufacturing Research District** announced 28 Apr 2026 anchored by the RFID Lab.
Birmingham is demoted *by choice*: the sector fit is best on paper, but he has never found it attractive to
visit — and travel appetite is now recorded as a real selection criterion.

Added to [[concepts/freelance-outreach-targets]]: the Chattanooga shortlist — ChaTech (melissa@chatech.org;
sponsorship via austin@chatech.org), the Chamber (200+ events/yr), **CO.LAB Office Hours** (join the expert
roster as the AI person — the highest-leverage move), the INCubator — plus the two sector plays (insurance:
Unum ~$13.3B + BCBST ~$6.2B; freight: Kenco, U.S. Xpress, Covenant), **F3 Future of Freight, Sept 15-17
2027 in Chattanooga**, and FreightWaves' pre-built **FreightTech100** target list.

**Cross-link worth chasing:** an advanced-manufacturing research park full of supplier-quality workflows is
exactly where the RCCA product wants design partners — Auburn's new district is a candidate for both the
freelance offer and the venture ([[concepts/rcca-app-venture]]).

## [2026-10-11] update | Ag / co-op channel added, and a second vertical for the RCCA product

Rick raised his brother-in-law, **general counsel at Alabama Farmers Cooperative (Decatur)**, as a market:
an industry slow to adopt technology, therefore full of unharvested low-hanging fruit. Verified rather than
assumed — AFC is ~37 member associations, ~90 retail locations, 2,300+ employees (revenue estimates vary,
~$698M per RocketReach); and the sector literature says the same thing in print (Springer Jan 2026 on
cooperatives' digital-transformation barriers; legacy-ERP-in-agriculture work describing "paper records,
spreadsheets and disconnected systems"). **No IA problem — it is a private commercial co-op.**

Added to [[concepts/freelance-outreach-targets]] as **the warmest door on the list**, with the traps stated
plainly (family risk; a GC opens doors but signs no POs; 6-18 month governance; harvest vs the Dec-Feb budget
window; the ERP vendor may claim the space; keep the family relationship out of public material) and the
wedge — **an AI assistant over the co-op's contracts, sold to the pain the general counsel personally owns**.

**Bonus finding, recorded on [[concepts/rcca-app-venture]]:** **SQF code clause 2.5.3 mandates a CAPA
programme** in food and feed manufacturing, so the RCCA product has a **second vertical at zero extra build
cost** with a warm door into it (AFC's feed/processing operations; poultry integrators and feed mills are
dense in the region). Thinly served by small-plant vendors, which proves the market.

## [2026-10-11] create | concepts/services-page-copy.md + the ag insight message

Rick's direction: for any of these markets, build a **professional business page showing sample
applications** — demonstrating real value to potential customers, especially non-technical ones, with
ideas they may not know exist.

- `concepts/services-page-copy.md` — publication-ready copy for a **Services** page: hero, **six
  role-based scenarios** in before/after form (the contract pile, the invoice pile, the forms nobody
  types, the repeating emails, the audit binder, the thirty-year veteran's head), the safety answers
  (runs on your network / you approve what goes out / your systems stay / you can walk away), the
  $750 assessment -> $3,500 two-week build ladder, who he works with, and an about paragraph.
  **Rule recorded:** show what it does, never name the machinery — no model names or AI-vocabulary words
  for this reader.
- Build notes captured: site is `~/code/2026/portfolio-gallery` (**rsegrest/ricksegrest.com**, `master`,
  Vite+React+TS, Vercel) -> add `src/pages/ServicesPage.tsx`, a route, and a NavBar link; phase 2 is an
  interactive demo served from `public/demos/` following the existing pattern.
- The outreach page gained the **insight-only message to Rick's brother-in-law** (three questions: who is
  drowning in documents, an introduction, and how the co-op buys software) with an explicit clean exit and
  an optional, clearly-labelled hypothesis line.

## [2026-10-11] create | concepts/side-income-map.md + the corrective-action glossary

Rick asked that all of these ideas be documented in the wiki. Added:

- `concepts/side-income-map.md` — **the single entry point** for the money thread: 10 threads with time to
  first dollar and the page each lives on (freelance services, warm outreach, Chattanooga, the ag/co-op
  channel, the RCCA venture, RCCA's food/feed CAPA vertical, the deferred ESSCA II raise, the visibility
  engine, referral partners, the house sale) plus a **ruled-out table with reasons** (investing, reselling,
  Power Apps, gov/defence AI, marketplace bidding, Toptal) so none of them get re-proposed.
- `concepts/rcca-app-venture.md` — new section **"The same problem has four names — which is the market
  map."** CAPA = Corrective And Preventive Action, the food/medical name for the process aerospace calls
  RCCA and automotive calls 8D. AS9100/AS9110, SQF 2.5.3, BRC, FDA 21 CFR 820, ISO 13485 and IATF 16949 all
  *mandate* it. One engine, four regulated industries, and the advice is to **use the buyer's word for it
  in the buyer's industry**.

## [2026-10-11] research | Ag market intelligence — the community map and what they actually say

Rick asked whether agriculture has discussion boards or whether that market is "too high-tech". It is the
opposite: **AgTalk/NewAgTalk has run since the early 2000s** (Machinery Talk alone: 533,907 threads /
4.45M posts; **Computer Talk** — software Q&A — 15,285 threads / 84,500 posts), alongside r/farming (~219K),
r/Agriculture, Agrivillage, Agriculture Information and country boards.

Read two r/farming threads via the **reddit-reading** skill (anonymous backend, one 429 sleep each):
1. *"For those thinking I'll just write some software to help farmers"* — "Ag software is mostly in 2004";
   nothing interoperates; "the secrecy of each software"; support calls as a negative revenue model; the
   EMR comparison including a $7M hospital system that still required paper charting as well. **A co-op
   employee** describes being "the in-between guy" as service spreads thin.
2. *"What software is missing in farming?"* — **"right now I use Excel"** for equipment maintenance; a farm
   with no irrigation records despite a five-year legal requirement; herd-health/drug logs stuck in software
   "that can't link to phones"; hay direct-sales needing inventory + bookkeeping + **offline**; and a grower
   furious that a $120K vendor also harvests their data.

Documented as `concepts/ag-market-intelligence.md` with the buyer-side layer too (**NGFA** — ~700 companies
incl. farmer-owned co-ops, Model Feed Quality Assurance Program since 1994; **AFIA** — Quality and Animal
Food Safety Committee, Safe Feed/Safe Food), the four positioning consequences for the offer, and the
**listening plan** (read, don't post; collect verbatim complaints; the "what should I build?" opener is worn
out). Etiquette note recorded: farmers are sceptical of vendors, not of technology.

## [2026-10-11] research | AgTalk Computer Talk mined — the audit-output gap is the finding

Worked through AgTalk as requested. **Cloudflare blocks my browser on the site root** (there is even a Sept
2026 support thread about it), but **individual thread URLs render through `web_extract`** and the search
endpoint is GET-able — so the board is repeatably mineable with no login. Recorded the recipe.

Best finds, in the farmers' own words:
- **"Been searching for the farm 'brain' that ties everything together for years but it does not exist"** —
  plus a stack of Granular + Fieldnet + QuickBooks + "lot's of spreadsheets: I don't think they're
  replaceable", a custom ERP attempt that "failed expensively", and a maintenance tool killed by "not enough
  buy-in from the guy I put in charge of it".
- **"What is the best farm record keeping"**: wants field records + machinery maintenance + GAP records
  "that will be 3rd party audited".
- **The wedge:** "Fieldview... has all of the data that you need to be compliant. But Fieldview is TERRIBLE
  for any other report format, and unless you print off every application for every field **you will not pass
  an audit**." The market leader is good at capture and bad at output.
- A farmer who **built his own Excel workbook for state/federal pesticide records and gives it away free**;
  notebooks for custom-work/landlord billing; and repeated "**we don't raise enough cattle to worth buying an
  expensive program**".

Four repeatable patterns documented in `concepts/ag-market-intelligence.md` §5: "too small for the expensive
program"; "better than an Excel spreadsheet"; **the audit-output gap**; and integration/adoption failure.
Offer consequence recorded: in this market the **audit binder is the headline scenario**, not one of six, and
two new scenarios (pesticide application records; custom-work/landlord billing) were added.

## [2026-10-11] create | Services page, agriculture variant (branch `services-page`, `/services/agriculture`)

Rick asked for a second services page on the secondary branch. Built
`src/pages/ServicesAgriculturePage.tsx` (route `/services/agriculture`) beside the general page, cross-linked
both ways, nav unchanged.

It leads with the **audit-output** wedge the AgTalk mining produced: "Your records already exist. Make them
answer the auditor." — six farm jobs (spray records, GAP/third-party audit binder, landlord and custom-work
billing, equipment maintenance, herd/treatment records, per-state mileage for fuel-tax filings), four answers
for the sceptical buyer (nothing leaves your network; works with no signal; your stack stays; you own the
output), a "what this is not" list, and three starts ending in the **free one-season "send me your records,
I'll send back the audit view"** offer — recorded as the reusable conversion device because it is the demo,
the qualification and a zero-risk first step at once.

Verified in a browser against a production build: both routes render (general page: 6 scenarios + a link to
the ag variant; ag page: 6 farm jobs, "What this is not", both price points, link back). Committed on the
branch (**not** master, so nothing deploys); branch pushed, master untouched. Editorial rule recorded on the
copy page: never lift a named forum user's words onto a commercial page — paraphrase the themes.

## [2026-10-11] create | concepts/demand-test-playbook.md — validated the smoke test, corrected the starting point

Rick proposed the YC-style splash-page/email-capture test with a modern upgrade (an interactive demo of one
real feature), plus a possible á la carte product suite sharing data, and asked where to start.

**Recorded:** the approach is right, and in this business the door need not be fake — the "send me one
season's records, I'll send back the audit view" promise is deliverable by hand today, making it a concierge
MVP with revenue attached. Behaviour (records actually sent) beats emails as a signal; benchmarks ~11% median
waitlist conversion, so ~200 qualified visitors is the minimum honest sample, and 0 visitors is not a test.

**Correction found while checking the competition:** landlord/custom-work billing — my first instinct for the
starting point — is **already contested** (Traction Ag invoices sharecrop/custom work automatically on its Pro
tier; Agnomy does ag invoicing + payments at 1%; nxtAcre bundles invoicing, imports and roles), and farm
accounting is contested and partly free (Farm-Ledger free tier). **Do not start there.**

**Where to start instead: spray/application records → the compliance view.** Four reasons: 40 CFR 170.311
legally requires the application record be retained for two years; the market leader is criticised precisely
for failing at audit *output*; the current workaround is a homemade Excel workbook and handwriting; and the
deliverable is a document, so the demo and the manual service are the same thing. Suite framing recorded as
**one records layer with per-job output modules**, and naming candidates listed (descriptive beats clever for
this audience).

## [2026-10-11] build | sprayproof MVP — the demand test, built and verified

Rick confirmed the model (gate the artifact, not the data entry) and asked for it as a new site. Built
`~/code/2026/sprayproof`: FastAPI + one static page, no build step, own git repo, **local only** (no remote,
nothing deployed). Domain core TDD'd — **14 tests passing** — covering record completeness against the
40 CFR 170.311 field set, the compliance view, export tiers, and permissive CSV ingestion (header synonyms,
any delimiter, junk ignored).

**Pricing implemented as decided:** free = import records and see the whole view; **export is the paid
artifact**, tiered by applications per year ($79 up to 250, $149 unlimited — placeholders). The gate is one
function in `app/tiers.py`.

**Verified end-to-end:** `/api/export` returns **402** on free and **200 + a 955-byte document** on $79; the
page renders six sample applications (4 complete, 2 incomplete, 151 acres, four highlighted cells, two gaps)
with the export locked and the paywall shown, and choosing $79 enables the export and clears the paywall.
`BUILD_LOG.md` was carried from the first line of code with the RED -> GREEN sequence recorded.

## [2026-10-11] design | sprayproof restyled as a printed almanac (dark neon theme retired)

Rick: the dark/neon theme was inappropriate for an agriculture application. Direction given: wheat background,
grassy green and sky blue accents, traditional conservative layout, serif fonts, cues from the Farmers'
Almanac. Rewrote `static/index.html` — palette (wheat paper, grass, sky, brick for flags), type (Bitter slab
serif masthead + Source Serif 4 body, small-caps labels, system fallbacks), layout (double-ruled centred
masthead, Roman-numeral sections, boxed panels, ruled ledger with a `†` on cells needing attention, figure
boxes, seal badge) and a **print stylesheet** so the ledger prints clean — printing the record is the product.

Element ids and the JS contract were preserved, and the behaviour was re-verified against the running service:
6 applications, 4 complete, 2 needing attention, 151 acres, 4 flagged cells, 2 gaps, document locked on Free
and unlocked on the $79 tier. Computed styles confirm wheat `rgb(247,241,225)`, Bitter 62px masthead, Source
Serif body, and no dark-mode leak. Committed and pushed to `rsegrest/sprayproof` (private); the design
direction is recorded in `concepts/demand-test-playbook.md`.

## [2026-10-11] research | Domain naming — what is actually available, and the layer-vs-module question

Rick found `sprayproof.com` unavailable and asked for the other ideas. Rather than paste a list, checked
**34 candidates against the Verisign registry**: eighteen plain descriptors and sixteen compounds, plus six
alternative-TLD variants. **Taken:** sprayproof, sprayledger, sprayrecord(s), spraylog, applicationrecords,
fieldledger, fieldrecords, rowrecords, recordrow, cropledger, fieldbook, recordbinder, farmpaper,
quietrecords, recordlayer, spraybook, cropbook, rowbook, tankbook, ledgerbook, sprayjournal, cropjournal,
fieldjournal, growerrecords, spraypaper, cropnotes, spraynotes, farmrecords, growerbook, ledgerrow.
**Available .com:** **growerledger**, **furrowrecords**, **sprayregister**, **applicationledger**,
**applicatorrecords**. (`sprayproof.farm` and `sprayproof.ag` also came back available, but those checks were
looser and need registrar confirmation.)

Recorded the naming criteria and a recommendation in `concepts/demand-test-playbook.md` §8: name the **layer**
rather than the first module, because the product is one records layer with per-job outputs — so
**GrowerLedger.com** as the umbrella ("GrowerLedger — Spray Records"), or **SprayRegister.com** if naming the
first product tightly. Advised against splitting brand from domain. Flagged that registry WHOIS is not a
purchase guarantee.

## [2026-10-11] naming | The Stokes umbrella — available, with one caution and one word to drop

Rick proposed **stokesagtech.com** as an umbrella brand under which individual apps are routed, using his
mother's maiden name: his grandfather **John D. Stokes was a farmer**. Checked availability — `stokesagtech`,
`stokesag`, `stokesagriculture`, `stokesagservices`, `stokesagtechgroup`, `stokesfarmtech`, `stokesagtools`
and `jdstokesag` are **all available** (only `stokesfarm.com` is taken), a far better field than the five of
thirty-four generic descriptors.

Verified the collision risk rather than assuming one: **Stokes Seeds** (founded 1881, 140+ years, Thorold ON
plus four US locations including LaBelle FL, selling into the Southeast) already owns the "Stokes" ear in
vegetable growing; **Stokes Agricultural Services Ltd** (UK) holds that company name; and **Stocks Ag** (UK)
is one letter away. Different product classes make legal risk low, but a formal USPTO search in the
software/records classes is the right next step before buying.

Recorded in `concepts/demand-test-playbook.md` §8: keep the surname (it passes the phone test and the
grandfather story is a credibility asset in a vendor-sceptical market), **drop "AgTech"** (venture vocabulary,
and the wrong signal on a truck door), and recommend the umbrella **StokesAg.com** with modules reading
"Stokes Ag — Spray Register" — plus the routing plan (paths first, subdomains later, a small module registry
in the app when the second module arrives).

## [2026-10-11] naming | Registry facts on STOKES — and one earlier recommendation reversed

Checked TSDR rather than guessing. **"STOKES" is a live registered US trademark of Stokes Seeds, Limited**:
Reg. 2,962,111 (standard-character claim — the word in any style) and Reg. 3,040,436, both LIVE, both renewed
in 2025, both claiming acquired distinctiveness in whole, counsel of record Barclay Damon LLP. **Goods are
"vegetable seeds and flower seeds", International Class 031 only** — software is Class 9/42, so the
registration does not cover the product Rick would sell.

The nuance is that the industries are identical and the customers overlap (Stokes Seeds sells to commercial
growers from four US locations including LaBelle, Florida). Same field, different goods, same buyers is the
shape of a confusion argument; the wide goods gap is what keeps it a judgment call rather than a blocker.
Also noted: **Stokes Agricultural Services Ltd** (UK, live) and **Stocks Ag** (UK, one letter away).

**Reversed one piece of my own earlier advice:** keep **"AgTech"** in the umbrella. I had argued to drop it
because farmers do not say "agtech" — but it is now the *distinguishing* word that keeps "Stokes AgTech" from
reading as a seed company or as the UK machinery firm. The recommendation is therefore: umbrella **Stokes
AgTech** (`stokesagtech.com`, available) for differentiation, plain product names underneath ("Spray
Register") where the farmer's trust decision actually happens, and the grandfather line in the About/footer.
Alternative if the surname feels too close: **J.D. Stokes Ag** (`jdstokesag.com`, available). Recorded in
`concepts/demand-test-playbook.md` §8 with the registry detail, flagged as research rather than legal advice.

## [2026-10-11] naming | John Deere checked — one assumption was wrong in Rick's favour

Rick worried that "John D. Stokes" / "J.D. Stokes" would attract John Deere's lawyers, and had already decided
to avoid their green/yellow. Checked the registry instead of guessing:

- **The "JD" registration (Reg. 1,062,200, filed 1975, typeset word mark, Deere & Company) is DEAD — expired
  5 Jan 2008.** Deere filed a **new "JD" application on 31 Aug 2026** (pending; goods/services unverified
  behind a paywall at the aggregator that surfaced it). So they are actively claiming the initials again, but
  no live registration is known to cover software.
- **What they enforce is the green-and-yellow trade dress:** a 2017 Kentucky decision held FIMCO's green and
  yellow on **sprayers and wheeled ag equipment** infringed and diluted Deere's marks, with the colours found
  "famous" since the late 1960s.
- **Reading the marks as wholes:** "J.D. Stokes" and "John Deere" share only a common given-name initial; the
  dominant element is the surname Stokes. Different dominant element, different goods — confusion unlikely,
  and a dilution claim over a records app named for a grandfather is a stretch. Worst realistic case is a
  letter.

Recorded in `concepts/demand-test-playbook.md` §8 with three cheap rules (never render it as "JD"; **no
green-and-yellow signature — which touches our own palette: brand green #3f6f2a + mustard #c1912a sits close
to Deere's dress, so make wheat/brick/sky the identity if a Stokes name is used**; avoid Deere product names
like Operations Center/GreenStar for modules). Recommendation given the three accumulated collisions: brand =
**Stokes AgTech**, story = "Named for John D. Stokes, who farmed", products = Spray Register etc. — the
personal name as story, not logo.

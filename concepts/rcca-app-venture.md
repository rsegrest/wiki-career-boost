---
title: RCCA App — Venture Assessment (Teledyne Brown friend's idea)
created: 2026-10-11
updated: 2026-10-12
type: concept
tags: [venture, app, defense, quality, rcca, income, side-hustle, product, partnership]
sources: [local prototype ~/code/rcca, user direct input 2026-10-11 (partnership + on-spec), DoW CIO 2026-07-13, DFARS 252.204-7012, ASQ / Duke Okes 2009, Curtiss-Wright supplier guideline]
confidence: medium
---

# RCCA App — Venture Assessment

> **Why this page exists:** to decide whether the Root Cause Corrective Action app becomes a real
> business — and it has moved past "favour": as of 2026-10-11 Rick and the friend are **starting a
> business together, co-owning the requirements and the prototype, built on spec.** This page now
> answers a different question: *what does that partnership have to settle before a dollar arrives?*
> Companion to [[comparisons/career-move-vs-side-hustle-vs-maximize-current]] (Path C) and
> [[../../wiki-personal/concepts/near-term-income-plan]] (where it sits among the income options).

---

## 1. The idea and the people

A friend who works as a **defense contractor at Teledyne Brown Engineering (Huntsville)** needs a
tool to **document and resolve Root Cause Corrective Actions (RCCA)** in his job. He wrote the
requirements; Rick built the prototype.

**Structure (per Rick, 2026-10-11): a partnership, not a favour.** The two are **starting a business
together and both own the requirements and the prototype** — the friend is the domain author, Rick is
the product. The intent is to build **on spec** and sell afterwards. That settles the ownership
question *between them*; it does not touch the employer-context question, which is now a question
about the **friend's** employment agreement (§3 and §7).

**The warm network runs deeper than one friend.** Rick was at **Teledyne Brown Engineering
himself, 2006–2011**, as a software developer ([[entities/rick-segrest-resume-v2026]]) — and one of
the things he built there was *"a modular database web portal that allowed users to track system
anomalies encountered in testing … used throughout the Boeing GMD Program."* An anomaly-tracking
system, for a defense prime, delivered by the same person now prototyping an RCCA tool. That is the
pitch, and it is true.

| Field | Value |
|---|---|
| Requirements author | the friend (`msjohnson` on the document), 30 Sep 2026 |
| Rick's relationship | former TBE developer (2006–2011); **co-founder** — the friend is the domain expert and internal champion |
| Rick's domain credibility | built a TBE anomaly-tracking portal for the Boeing GMD program |
| Product thesis (from the spec) | **guided RCCA *reasoning*, not CAPA recordkeeping** |

---

## 2. What actually exists — verified on disk, 2026-10-11

Not a deck. A working, tested, running application.

| Artifact | Verified state |
|---|---|
| Requirements source | `specs/RCCA_Enterprise_Application_Requirements_v0.3.pdf` — 22-page tabloid, author `msjohnson`, 30 Sep 2026 |
| Converted baseline | 279 ID'd rows = **270 requirements** (Must 212 / Should 57 / Could 1) + 9 principles; 30 ID families; **15/15 converter gates pass**, regeneration byte-identical |
| Prototype app | Vite 8 + React 19 + TypeScript 6 + Vitest 5; **62 source files, ~9,500 lines, 114 tests, 0 type errors**; no backend; state in the browser (localStorage) |
| Build | 379 kB (113 kB gzip) |
| Running now | systemd **user** services `rcca-preview.service` (port 4180) + `rcca-tunnel.service` (cloudflared quick tunnel) → public HTTPS URL via `~/.hermes/scripts/rcca-url.sh`; phone layout verified on all 16 routes |
| Build ledger | **21 defects, 0 open**; ~135 min total across T1–T3; deepseek-v4.1-flash 100% |
| Documentation | `BUILD_LOG.md` (task ledger + review report), `docs/CONVERSION-NOTES.md` (incl. **defects found in the source document**), captioned desktop + phone screenshots |

### ✅ Closed 2026-10-11: it is now under version control

`~/code/rcca` was **not** a git repository and had never been committed — the entire artifact (the
converted 279-row baseline, the converter, the validator, the app, the tests) lived in a single
working tree with no history. **Fixed:** `git init` + a `.gitignore` for `node_modules/`, `dist/`,
`coverage/` and editor files, then an initial commit.

| | |
|---|---|
| Commit | `6731b5d` on branch `main` |
| Tracked files | **99** (zero `node_modules` — 92 MB of dependencies stay out) |
| History size | 3.9 MB |
| Remote | **none** — publishing is a separate decision, because the v0.3 document is employer-context material authored by the domain expert |

The ownership question in §3 is answered **before** anything leaves this machine; that ordering is
deliberate.

---

## 3. The method is public — which is what makes it sellable

Checked before assuming the friend's methodology was the moat:

- **DO IT²** — the ten-step model the spec walks ("FIND IT" diagnostic steps 1–5, "FIX IT" solution
  steps 6–10) — is **published**: Duke Okes, *Root Cause Analysis: The Core of Problem Solving and
  Corrective Action*, ASQ Quality Press, 2009, which ships the DO IT² RCA Guide and problem-solving
  worksheet in its appendices.
- **Curtiss-Wright's public RCCA Supplier Guidelines** lay out the same spine — containment →
  problem definition → RCA → plan development → implementation → **verification of effectiveness**
  (with Measures of Effectiveness) — and tie it explicitly to AS9100.

**So:** no methodology licence is needed, and no single vendor owns the process. That is a licence
to build. It cuts both ways — it also means *the method is not the moat*. The moat has to be the
**UX of thinking through a cause tree under evidence**, which is exactly what the prototype does and
what a QMS suite does badly.

**The live legal question has moved, and it is not between the two partners.** Co-ownership settles
who holds the work *between them*. What remains is the **friend's employment relationship with TBE**:
requirements written by a quality engineer *about his employer's process*, plus an invention-assignment
or confidentiality clause, is the classic fact pattern for an employer claim — and moonlighting rules
are the employer's, not the partnership's, to decide. **He should read his own agreement before
contributing more**, and the two of them should put the ownership split in writing while it is still
easy to do.

**And the buyer is that same employer.** The highest-value path on this page is a **paid pilot at
TBE** — so the employment question and the sales question point at one organisation and should be
resolved together, deliberately, rather than one surprising the other. Selling to your own employer
while employed by them is a conflict-of-interest question **for the friend**, and it is his to clear
(disclosure, a side-letter, or simply not selling to TBE at all and going to small AS9100 suppliers
instead — which is the larger market anyway).

### Distribution: closed source, and that is a deliberate contrast (2026-10-12)

Rick's call, recorded so a later session does not re-propose it: **RCCA is not an open-source project and will
not be given away.** It is a different venture with a different buyer from the agricultural track — and the
buyer is the reason. Defence and aerospace suppliers are the *worst* possible audience for a copyleft licence:
what they procure is a **closed, contractually accountable product** with a vendor behind it, licence terms
their own flow-downs accept, and an SBOM their software-assurance review can pass. AGPL is banned outright at
many large companies (Google's policy is explicit and long-standing), so publishing under it would forfeit the
only sale this product has.

**The ownership gate therefore changes shape rather than disappearing.** With no repository going public, the
split with his partner — and the friend's employment position — must be settled in writing **before the code
is shared with anyone outside the two of them**: an investor, a pilot customer, a subcontractor, an employee.
The employer question still comes first, because it is the one that can void the whole thing.

Contrast with the ag product, where opening the code buys distribution and trust:
[[concepts/open-source-business-model]].

---

## 4. The market

| Tier | Who | Price point |
|---|---|---|
| Enterprise QMS suites | MasterControl, ETQ Reliance, TrackWise, Qualio, Greenlight Guru, ComplianceQuest, Qualityze | **~$14K+/yr** before implementation |
| Small-supplier AS9100 tier | niche vendors (e.g. QSOD) | **~$3K/yr**, unlimited users |
| **This tool's opening** | RCCA-only, guided reasoning | **~$100–300/mo/site** — sits *under* the incumbent floor |

The incumbents sell **recordkeeping**: modules, workflows, audit trails. The prototype's own

### A second vertical, at zero extra build cost: food and feed manufacturing (found 2026-10-11)

The same product solves a *mandatory* compliance problem in a different industry. **SQF Code clause 2.5.3**
requires a documented correction / corrective action / preventive action (CAPA) programme — root cause,
verification of effectiveness, audit-ready records — and BRC-adjacent standards run the same spine. SQFI
publishes its own CAPA guidance document.

So the food/feed processing industry is RCCA's second vertical, and it is served thinly: a few small-plant
vendors exist (Qualitronyx pitches "pass your SQF/BRC audit without the Excel chaos"; SafetyChain sells SQF
management), which proves the market rather than closing it — plenty of small and mid-size plants still run
CAPA in spreadsheets. This is the **same reasoning problem the prototype already solves**, with no new build.

**And it has a warm door:** Alabama Farmers Cooperative's feed and processing operations sit inside the
network of Rick's brother-in-law (general counsel there), in a region where poultry integrators, feed mills
and processors are dense. See [[concepts/freelance-outreach-targets]] for the ag channel and its cautions.

### The same problem has four names — which is the market map

**CAPA = Corrective And Preventive Action.** It is the *same process* as RCCA, wearing the vocabulary the
food-safety and medical-device industries use. "Run CAPA in Excel" means the plant tracks those corrective
actions in a spreadsheet or a binder: no workflow, no evidence attached to each cause, no
verification-of-effectiveness step, and audit preparation turns into a scavenger hunt. That is precisely
the pain the prototype addresses — in another industry's words.

| Industry | The process is called | Mandated by | The paperwork |
|---|---|---|---|
| Aerospace & defence | **RCCA** — Root Cause Corrective Action | AS9100 / AS9110 | CAR (corrective action request), NCR (nonconformance report) |
| Food & feed manufacturing | **CAPA** — Corrective And Preventive Action | SQF Code 2.5.3, BRC | Nonconformance and corrective-action records |
| Medical devices | **CAPA** | FDA 21 CFR 820, ISO 13485 | CAPA record, NCR |
| Automotive | **8D** — Eight Disciplines | IATF 16949 | D1-D8 problem-solving report |

One product, four regulated industries, each of which **mandates** the process, each of which has small
suppliers who struggle to comply, and the reasoning engine is identical in all four: find the cause, fix
it, prove the fix stuck. **Use the buyer's word for it in the buyer's industry** — RCCA in aerospace,
CAPA in food and medical, 8D in automotive, CAR/NCR everywhere.


thesis is the gap — a tool that **helps you reason to a verified root cause** (proposed → testing →
supported → confirmed, with evidence attached, and a report that proves it) rather than a form that
files one. Small aerospace/defense suppliers are the plausible buyer: they must close RCCAs to
satisfy AS9100 and their primes, and they cannot afford an enterprise suite.

---

## 5. The compliance gate (checked 2026-10-11 — it is *more* open than expected)

Three layers, and only the third one actually bites:

1. **CMMC Phase 2 is suspended.** The Department of War CIO announced an **immediate suspension on
   13 July 2026** with a 60-day review of structure, cost and assessment model; the mandatory
   Phase 2 third-party (C3PAO Level 2 / DIBCAC Level 3) assessments — which had been due to take
   effect **10 Nov 2026** — are paused. **Level 1 and Level 2 self-assessments still stand.**
   *(Reported by DLA Piper 2026-08-03, Faegre Drinker 2026-07-17, and others; not yet re-verified
   against the DoW site itself.)*
2. **DFARS 252.204-7012 is unchanged** — NIST SP 800-171 Rev 2, **72-hour incident reporting**, and
   the **SPRS score as a condition of award**. The suspension did not touch any of it.
3. **The real gate for a hosted app — DFARS 7012 (D):** a contractor using an **external cloud
   service provider** to store, process or transmit covered defense information must require that
   the CSP meets security requirements **equivalent to the FedRAMP Moderate baseline** (per the
   DoD's Dec-2023 equivalency memo, including the no-POA&M rule).

### → The design consequence, and it should be decided now, not at hosting time

**Build for a no-CUI deployment.** RCCA records — nonconformances, causes, actions, effectiveness
measures — are **quality-process records**, not technical data. If customers do not put
export-controlled or technical data in the tool, it never enters CUI scope, and **FedRAMP is off
the critical path entirely**. If a customer insists on putting CUI in it, that is a *separately
qualified deployment* — which the spec already anticipates: **CMP-006** states that defense/CUI-
capable hosting must be treated as a separate posture and **must not be claimed merely because the
application supports STIG-related configuration**. Hold that line; it is the difference between a
$200/mo product and a compliance programme.

---

## 6. Monetization, ranked by time-to-first-dollar

| # | Path | First money | Time to first $ | Effort | Risk |
|---|---|---|---|---|---|
| 1 | **Paid pilot at the friend's org** (friend = champion + named domain reviewer) | **$10–25K**, **split with the partner → $5–12.5K to Rick** (100–200 hrs @ $100–125) | weeks, if he says yes | medium | needs the friend's employment position cleared first, and TBE is both his employer and the buyer |
| 2 | **Productized RCCA engagement** for small AS9100 suppliers — "I'll stand up your RCCA process and leave you the tool" | **$15–50K** per project | 1–3 months | high | needs a case study to sell |
| 3 | **RCCA workshop / method training** (public method + the friend's handbook as the case material) | **$2–8K** per cohort | 1–2 months | low capital | caps out; training is a job |
| 4 | **SaaS at ~$199/mo/site** | ~**$2K/mo at 20 sites** | **12–24 months** | very high | support, hosting posture, sales motion, compliance creep |

**Read the table against the household constraint:** only paths 1–3 pay inside the 90 days that
matter ([[../../wiki-personal/concepts/near-term-income-plan]]). Path 4 is the real business, but it
is the slowest thing on this page and should not be attempted until **one paying pilot exists**.

**Two corrections that "on spec" forces, and they are arithmetic, not sentiment:**

1. **Revenue is split.** A $10–25K pilot is **$5–12.5K to Rick** under a 50/50 split, which is the
   number that matters against [[../../wiki-personal/concepts/near-term-income-plan]], not the gross.
   Fix the split in writing before the first invoice, not after.
2. **On spec means months of unpaid hours before the first dollar.** That is a legitimate way to build
   an asset — and it competes directly with the freelance hours that actually retire the debt. So the
   honest framing is: **on-spec is fine for the product, but the first money must come from a paid
   pilot or a services engagement, not from finishing the app.** Cap the on-spec hours at a number
   both partners agree on, and review it against the pilot's progress rather than against how close
   v1 feels.

**Employment constraints, already checked:** the career vault's own open questions record that
Amentum's moonlighting position is *"no problem as long as it doesn't interfere or compete"* and the
non-compete is *"standard … can't compete directly"*. RCCA software is not Amentum's NASA business,
so it does not compete — but a **sale to a defense contractor** is exactly the shape of thing worth
disclosing before it happens rather than after. Rick's clearance is **dormant** and the app needs no
clearance (and no CUI, per §5).

**Rick's side is the clearer side; the friend's is the binding one.** Rick has already answered the
moonlighting and non-compete questions for himself. The partner is a *current TBE employee whose
employer is the target customer* — so the gating constraint on the whole venture is **his** agreement,
not Rick's, and it is the first thing to resolve (§8).

---

## 7. Risk register

| Risk | Why it bites | Mitigation |
|---|---|---|
| **The friend's employment agreement** | the requirements describe his employer's process; invention-assignment and moonlighting clauses are the employer's to invoke, and TBE is also the buyer | **he reads his own agreement first**; put the partnership split in writing; be ready to sell to small AS9100 suppliers instead of TBE |
| **Conflict-of-interest optics** | selling into defense while on a NASA contract | disclose; keep it clearly non-competing; no employer resources or time |
| **Single point of failure** | the friend leaves TBE → champion, domain expertise and the pilot lead all evaporate | get a second domain reference early; document the method rather than relying on him |
| **Compliance scope creep** | an RCCA tool becomes part of someone's audit evidence, so its own defects become their findings | no-CUI posture; explicit "decision-support, not a record of authority" statement |
| **On-spec, no revenue until a sale** | two people funding a product with unpaid nights; it competes with the freelance hours that retire the debt | agree and cap the on-spec hours; require the first money to be a **paid pilot/service**, never a finished product |
| **Rick's hours** | it competes with freelance hours that pay 3–10× faster | treat as an **asset-building** bet with a hard time cap, not as this quarter's income |

---

## 8. Next steps (in order — the first one is free)

1. ~~**`git init` the repo and commit**~~ ✅ **done 2026-10-11** (99 files, commit `6731b5d`, no
   remote yet).
2. **The gating questions, in writing** — the ownership one is now *answered between the partners*,
   so the three that remain are: (a) **has the friend read his own employment agreement**, and does it
   let him contribute this (invention assignment / confidentiality / moonlighting)? (b) would TBE run
   this as a **paid pilot**, who signs, and does his conflict-of-interest position allow it? (c) will
   he be the named domain reviewer? Everything else waits on (a) and (b).
3. **Decide the wedge in one sentence, and price it** — "weeks of guided root-cause work, not a
   CAPA module" at $X for Y weeks. A pilot needs a number before it needs a demo — and the number
   should be quoted **gross, with the split stated**, so both partners are pricing the same deal.
4. **Only then** consider SaaS, and only after a pilot pays.

---

## Open questions

- [x] ~~Who owns the v0.3 requirements document?~~ **Answered 2026-10-11:** the two partners
      co-own the requirements and the prototype (he authored, Rick built) — the remaining exposure is
      **his employer's** claim, not a dispute between them. See the new questions below.
- [ ] **Has the friend's own employment agreement been read?** (invention assignment, confidentiality,
      moonlighting) — the binding constraint on the whole venture, and the partner's to resolve.
- [ ] **What is the ownership split in writing?** Equity, IP, who can leave with what, and how pilot
      revenue is divided (the income plan quotes $5–12.5K to Rick on a $10–25K pilot at 50/50).
- [ ] **How many on-spec hours, capped, before a paid pilot exists?** Two people's unpaid evenings are
      the real cost of "on spec" — and they compete with Rick's fastest-paying lever.
- [ ] Would the friend's employer actually **buy** this, or does he want it as an internal tool he
      never has to pay for? *(These lead to very different projects.)*
- [ ] Is the friend willing to be named publicly as domain expert, or does his employer's policy
      stop him?
- [ ] Do small AS9100 suppliers in North Alabama buy tools this way (direct, GSA, prime flow-down)?
- [ ] Does a "no-CUI" deployment posture hold up when a customer's quality org wants to attach a
      nonconformance report to a technical drawing? *(This is the assumption the whole cheap-hosting
      argument rests on.)*
- [ ] What do the 279 requirements cost to finish as a product — i.e. how far is the prototype from
      a v1 a stranger could buy? *(Not estimated yet.)*

## Sources

- `~/code/rcca/` — `README.md`, `BUILD_LOG.md`, `specs/RCCA_Enterprise_Application_Requirements_v0.3.md` (inspected 2026-10-11)
- [[entities/rick-segrest-resume-v2026]] — TBE 2006–2011; the GMD anomaly-tracking portal
- DoW/DoD CIO CMMC Phase 2 suspension, **13 July 2026** (60-day review; Phase 2 had been due 10 Nov 2026) — reported via DLA Piper (2026-08-03), Faegre Drinker (2026-07-17), Fortinetics (2026-07-14)
- **DFARS 252.204-7012** text, incl. paragraph (D) on external cloud service providers and FedRAMP Moderate equivalence — acquisition.gov; DoD FedRAMP-equivalency memo (Dec 2023)
- Duke Okes, *Root Cause Analysis: The Core of Problem Solving and Corrective Action*, ASQ Quality Press, 2009 — DO IT² model + Appendix B guides
- Curtiss-Wright, *RCCA Supplier Guidelines* (rev 2) — public supplier-facing RCCA process, AS9100 linkage
- [[comparisons/career-move-vs-side-hustle-vs-maximize-current]] — Path C mechanics, moonlighting/non-compete answers
- [[queries/react-ai-job-market-salary-2026]] — the $100–175/hr rate band this page prices against

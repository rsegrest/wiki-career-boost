---
title: RCCA App — Venture Assessment (Teledyne Brown friend's idea)
created: 2026-10-11
updated: 2026-10-11
type: concept
tags: [venture, app, defense, quality, rcca, income, side-hustle, product]
sources: [local prototype ~/code/rcca, DoW CIO 2026-07-13, DFARS 252.204-7012, ASQ / Duke Okes 2009, Curtiss-Wright supplier guideline]
confidence: medium
---

# RCCA App — Venture Assessment

> **Why this page exists:** to decide whether the Root Cause Corrective Action app becomes a
> product/business or stays a favor for a friend — and to name the next three moves either way.
> Companion to [[comparisons/career-move-vs-side-hustle-vs-maximize-current]] (Path C) and
> [[../../wiki-personal/concepts/near-term-income-plan]] (where it sits among the income options).

---

## 1. The idea and the people

A friend who works as a **defense contractor at Teledyne Brown Engineering (Huntsville)** needs a
tool to **document and resolve Root Cause Corrective Actions (RCCA)** in his job. He wrote the
requirements; Rick built the prototype.

**The warm network runs deeper than one friend.** Rick was at **Teledyne Brown Engineering
himself, 2006–2011**, as a software developer ([[entities/rick-segrest-resume-v2026]]) — and one of
the things he built there was *"a modular database web portal that allowed users to track system
anomalies encountered in testing … used throughout the Boeing GMD Program."* An anomaly-tracking
system, for a defense prime, delivered by the same person now prototyping an RCCA tool. That is the
pitch, and it is true.

| Field | Value |
|---|---|
| Requirements author | the friend (`msjohnson` on the document), 30 Sep 2026 |
| Rick's relationship | former TBE developer (2006–2011); friend is the domain expert and internal champion |
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

### ⚠️ The one urgent gap: it is not in git

`~/code/rcca` is **not a git repository** and has never been committed. The entire artifact — the
converted 279-row baseline, the converter, the validator, the app, the tests — lives in a single
working tree with no history and no remote. One bad `rm`, one disk event, and it is gone. This is a
**five-minute fix and it is the highest-value five minutes available on the project**. Add
`.gitignore` for `node_modules/` first, then commit locally; publishing is a separate decision.

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

**Still a live legal question:** the v0.3 *document* was written by the friend **inside an employer
context**. Document ownership, and any employer process material inside it, needs a straight answer
in writing before this is sold to anyone. Ask first, build second.

---

## 4. The market

| Tier | Who | Price point |
|---|---|---|
| Enterprise QMS suites | MasterControl, ETQ Reliance, TrackWise, Qualio, Greenlight Guru, ComplianceQuest, Qualityze | **~$14K+/yr** before implementation |
| Small-supplier AS9100 tier | niche vendors (e.g. QSOD) | **~$3K/yr**, unlimited users |
| **This tool's opening** | RCCA-only, guided reasoning | **~$100–300/mo/site** — sits *under* the incumbent floor |

The incumbents sell **recordkeeping**: modules, workflows, audit trails. The prototype's own
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
| 1 | **Paid pilot at the friend's org** (friend = champion + named domain reviewer) | **$10–25K** (100–200 hrs @ $100–125) | weeks, if he says yes | medium | needs the written IP answer; **disclose to Amentum** |
| 2 | **Productized RCCA engagement** for small AS9100 suppliers — "I'll stand up your RCCA process and leave you the tool" | **$15–50K** per project | 1–3 months | high | needs a case study to sell |
| 3 | **RCCA workshop / method training** (public method + the friend's handbook as the case material) | **$2–8K** per cohort | 1–2 months | low capital | caps out; training is a job |
| 4 | **SaaS at ~$199/mo/site** | ~**$2K/mo at 20 sites** | **12–24 months** | very high | support, hosting posture, sales motion, compliance creep |

**Read the table against the household constraint:** only paths 1–3 pay inside the 90 days that
matter ([[../../wiki-personal/concepts/near-term-income-plan]]). Path 4 is the real business, but it
is the slowest thing on this page and should not be attempted until **one paying pilot exists**.

**Employment constraints, already checked:** the career vault's own open questions record that
Amentum's moonlighting position is *"no problem as long as it doesn't interfere or compete"* and the
non-compete is *"standard … can't compete directly"*. RCCA software is not Amentum's NASA business,
so it does not compete — but a **sale to a defense contractor** is exactly the shape of thing worth
disclosing before it happens rather than after. Rick's clearance is **dormant** and the app needs no
clearance (and no CUI, per §5).

---

## 7. Risk register

| Risk | Why it bites | Mitigation |
|---|---|---|
| **The v0.3 document's ownership** | written by the friend in an employer context; selling around it invites a claim | written permission / ownership answer **before** any sale |
| **Conflict-of-interest optics** | selling into defense while on a NASA contract | disclose; keep it clearly non-competing; no employer resources or time |
| **Single point of failure** | the friend leaves TBE → champion, domain expertise and the pilot lead all evaporate | get a second domain reference early; document the method rather than relying on him |
| **Compliance scope creep** | an RCCA tool becomes part of someone's audit evidence, so its own defects become their findings | no-CUI posture; explicit "decision-support, not a record of authority" statement |
| **Rick's hours** | it competes with freelance hours that pay 3–10× faster | treat as an **asset-building** bet with a hard time cap, not as this quarter's income |

---

## 8. Next steps (in order — the first one is free)

1. **`git init` the repo and commit.** 5 minutes. `.gitignore` `node_modules/` and `dist/` first. The
   only copy of 135 minutes of gated work is currently unprotected.
2. **Three questions in writing to the friend** — (a) who owns v0.3 and may it be used commercially?
   (b) would TBE run this as a **paid pilot**, and who signs? (c) will he be the named domain
   reviewer? Everything else waits on these.
3. **Decide the wedge in one sentence, and price it** — "weeks of guided root-cause work, not a
   CAPA module" at $X for Y weeks. A pilot needs a number before it needs a demo.
4. **Only then** consider SaaS, and only after a pilot pays.

---

## Open questions

- [ ] Who owns the v0.3 requirements document, and is commercial use permitted?
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

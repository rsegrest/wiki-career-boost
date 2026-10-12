---
title: Open-Source Business Model — what to open, what to sell, and why not a nonprofit
created: 2026-10-12
updated: 2026-10-12
type: concept
tags: [open-source, licensing, business-model, agtech, strategy, legal, impact]
sources: [user direct input 2026-10-12, farmos.org/hosting + farmier.com (checked 2026-10-12), IRS Form 1023-EZ instructions (rev. 2025), Foley "Establishing a New Section 501(c)(3) Organization" (2026), donewithember state-fee table read from state sites Sept 2026, Ars Technica + PetaPixel 2026-10 on AI-built Adobe clones, Software Freedom Conservancy and Open Source Collective fiscal-host documentation, anthropic.com/company and anthropic.com/news/the-long-term-benefit-trust, openai.com/our-structure]
confidence: medium
---

# Open-Source Business Model

> **Why this page exists:** Rick asked how to start a software company that has a positive impact and still
> sustains the work — given that AI has collapsed the cost of recreating software, and that the obvious shape
> (open the code, sell implementation and hosting, accept donations) might force him into a nonprofit. It does
> not. This page records the reasoning, the verified costs, and the options deliberately ruled out.

## The decision, as it stands on 2026-10-12

| Question | Recommendation | Status |
|---|---|---|
| **Legal form** | For-profit. Single-member LLC now; C-corp only if a partner or investors arrive. Add a Delaware **PBC** clause for the mission | Recommended |
| **A nonprofit** | **No** — the cost is ownership, permanently. See below | Recommended |
| **Donations** | Sponsorships invoiced as a company; or a **fiscal host** if donors need a deduction. Never an entity of his own | Recommended |
| **Application licence** | **AGPL-3.0**, with a CLA from day one | Recommended, **deferred** — "sounds good, but I don't know enough to commit" |
| **Record format / schema / docs** | Apache-2.0, so the *file* becomes a standard others build on | Recommended |
| **Kept proprietary** | Hosting control plane, integration credentials and sync, certified audit-signed report generation, client-specific modules | Recommended |

**The licence decision is safe to defer, deliberately.** While Rick is the only copyright holder he can
relicense his own code at will — MIT today, AGPL next year. The deadline is the **first public push** or the
**first outside contribution**, whichever comes first, and not a day before.

## Two decisions that get fused, and shouldn't

**Open source and tax status are independent.** Almost every open-source business is an ordinary for-profit
selling something adjacent to free code — Red Hat sells support; Ghost, Plausible and Sentry sell hosting;
Frappe sells Frappe Cloud around the GPL-covered ERPNext; Metabase sells an enterprise tier. **Mozilla is the
exception, not the rule**, and it is the heavy version: a 501(c)(3) owning a taxable corporation, with two
organisations and a board.

**Donations and tax status *are* linked.** A for-profit may accept donations and sponsorships — they are simply
taxable income — but it cannot offer the donor a deduction. That is the whole difference, and it is why the
fiscal-host route below exists.

## The closest precedent is in his own market

| Model | What it is | What it teaches |
|---|---|---|
| **farmOS + Farmier** | farmOS is free software for farm planning and record-keeping — self-host, modify, extend. Farmier sells "farmOS as a service": hosting, automatic updates, backups, SSL | **This is the plan, already running in agriculture.** Farmier was started by *farmOS's own creator* and its subscriptions fund farmOS's development |
| Ghost | Open-source publishing, hosted Ghost(Pro), run by its own foundation | Foundation-owned is possible, but it is a second organisation |
| Plausible, Sentry, Metabase | Open core, or AGPL plus paid hosting | Recurring revenue, small teams, no foundation required |
| ERPNext / Frappe | GPL application, money from Frappe Cloud and services | The nearest large analogue: a full business app, open, monetised through cloud and implementation |
| Red Hat | Subscriptions and support around free software | Services revenue is a legitimate, long-lived model — but it consumes the founder's hours |

Copy farmOS and Farmier. Do not copy Mozilla.

## AGPL in plain terms

*Free to use, free to modify, free to sell — but if you run a modified version as a service for other people,
you must publish those modifications.* The §13 network clause is the only thing that distinguishes it from the
plain GPL.

| Question | Answer |
|---|---|
| Can he charge money? | **Yes.** Selling hosting for AGPL software is the intended use, not a loophole |
| Can a competitor take it and host it? | **Yes, but they must publish their modifications.** AGPL protects the *code commons*, not his market share — the moat is service, compliance know-how and brand |
| Can client work stay private? | **Only if it is separate, not a modification of the core.** This is the one that bites the custom-development revenue line — see below |
| Can he sell a commercial licence later? | **Yes, if a CLA exists** — which is also how a customer with an AGPL ban gets served |

**What AGPL does not require:** publishing the *hosting infrastructure* (deployment scripts, monitoring,
backups — only the modified *program*), or giving away any data. And it imposes **nothing on customers**: a
farmer using the hosted app has no obligations at all; the duties fall on whoever runs or modifies the software.

**The custom-development wrinkle, stated plainly.** If he modifies the AGPL core for a client and hosts it, that
client's users must be offered the source — which can conflict with a client who wants their customisation
private. Two honest resolutions: tell clients up front that changes to the core are published (for most buyers
this is a *selling point* — no lock-in for them either), or keep client-specific work as a **separate service
talking over an API**, not a folder of patches. Plugins that link against or derive from AGPL code are
derivative works and must be AGPL; separation by process boundary is the mechanism, not a directory.

## The one irreversible mistake

**Accepting an outside contribution without a CLA.** The licence choice is reversible while he owns 100% of the
copyright; the moment a stranger's patch lands, that freedom is gone and no later relicensing or dual-licensing
is possible without chasing every contributor. So the thing to get right is not the licence — it is the
contributor agreement, and deciding that a CLA will exist costs nothing today.

## The IP premise, verified rather than assumed

The premise is real: in October 2026 an engineer shipped **AI-built open-source alternatives to Adobe's
Creative Cloud** (Photoshop, Illustrator, Premiere, Lightroom and more). Ars Technica's verdict is the useful
half — *"ambitious, free, and nowhere near finished."*

Two consequences. Software copyright never protected **function**, only expression, so cloning features was
always lawful; what collapsed is the **cost of writing the code**. Which means the sharper conclusion is not
"IP is collapsing" but **the code was never the moat**. What resists cloning is the record format, knowing what
an inspector actually accepts, the integrations, uptime, and being the person who answers the phone.

His read on his own customers is right too: almost no farmer will self-host. The self-host option is not a
competitor, it is **credibility** — and it caps the price, which is acceptable, because the farmer who would run
a Linux server was never going to pay.

## What a nonprofit would actually cost — and why it is ruled out

| Item | Verified figure |
|---|---|
| IRS Form 1023-EZ user fee | **$275** (normally ≤ $50k/yr gross receipts, ≤ $250k assets) |
| IRS full Form 1023 | **$600** (required if more than $50k/yr is expected) |
| First-year government fees, total | **$283–$500** with 1023-EZ; **$608–$825** with the full form |
| Annual | 990 series returns; state annual reports (~$10–$20+ in many states) |
| The real burden | **Multi-state charitable solicitation registration** if soliciting nationally — practitioners recommend hiring a vendor — plus state tax-exemption filings and audited financials above thresholds |

The fees are not the reason to refuse it. **The reason is that a nonprofit has no owners: no equity, no sale, no
investment, assets permanently dedicated.** For someone whose whole plan is to build an asset that sustains his
family, that is the most expensive option on the table. *Donations for an emerging-economy deployment do not
require it either.*

## The middle path: fiscal sponsorship

A **fiscal host** is a nonprofit that holds money on a project's behalf — accounting, tax, compliance and
payouts included — with no entity of his own and full ownership of his project. Software Freedom Conservancy
and NumFOCUS are the usual homes for software projects; Open Source Collective is another. **Check the host's
own tax status before promising a donor a deduction** — they are not all 501(c)(3)s.

## Funding the impact side

Treat emerging-market deployment as a **revenue line item** (a committed percentage of revenue) or a
fiscally-hosted donor fund, and **partner rather than build a field operation**: CGIAR, FAO, GIZ, Digital Green
and foundation agriculture programmes already have the field presence. Note the traditional USAID route was
largely dismantled in 2025 — verify the current funding landscape before planning around any agency. A
for-profit can receive grants from many funders, though some restrict them to nonprofits.

## Ruled out, with the reason (so it is not re-proposed)

| Idea | Why not |
|---|---|
| Form a 501(c)(3) now | $283–$825 in year one is trivial, but it forfeits all ownership permanently and adds 990s, state registrations and a board. No benefit at this stage |
| Mozilla-style foundation owning a taxable subsidiary | Correct for a company earning hundreds of millions from one partner; two organisations, a board and IRS scrutiny for a one-person venture |
| Permissive licence (MIT/Apache) for the application | Gives away the only thing that keeps a hosted competitor honest; fine for the *format*, wrong for the app |
| Donations as the primary income | Does not clear the household gap, does not scale with hours worked, and makes the mission hostage to donor mood |
| Self-hosting customers as a threat | They were never buyers. They are the reason the "no lock-in" promise is credible |

## Gates before anything publishes

1. **The CLA must exist** before any public push.
2. **RCCA's ownership must be settled in writing** with his partner before that repo goes public — those
   requirements came from someone else, and the v0.3 document carries employer-context material.
3. A customer with an AGPL ban is a **dual-licensing** conversation, not a redesign.

## Related

- [[concepts/rcca-app-venture]] — the venture whose code this decision governs
- [[concepts/demand-test-playbook]] — test demand before building; the same discipline applies to publishing code
- [[concepts/side-income-map]] — where this thread sits in the money map
- [[concepts/freelance-portfolio-strategy]] — the "I open-sourced X, I can build custom Y" pattern
- [[concepts/ag-market-intelligence]] — why "your records are yours" lands in this market
- [[concepts/john-d-stokes-brand]] — the product brand this would sit under
- [[../../wiki-personal/concepts/near-term-income-plan]] — the household constraint that sets the sequencing

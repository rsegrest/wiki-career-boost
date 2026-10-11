---
title: Demand-Test Playbook — splash page, interactive demo, and where to start
created: 2026-10-11
updated: 2026-10-11
type: concept
tags: [validation, product, startup, smoke-test, pricing, agriculture, strategy]
sources: [user direct input 2026-10-11, concepts/ag-market-intelligence.md, 40 CFR 170.311 (retention, checked 2026-10-11), waitlist conversion benchmarks (getwaitly / waitlister / lemonpage, 2026), tractionag.com pricing, nxtacre.com, agnomy.com, farm-ledger.com (all checked 2026-10-11)]
confidence: medium
---

# Demand-Test Playbook

> **Why this page exists:** Rick proposed the classic YC-era move — a splash page on its own domain with a
> mock-up, a marketing description and an email capture, to test whether a product is worth building before
> building it — with the modern upgrade of an **interactive demo of one real feature**. This page validates
> the approach, records what to measure, ranks the modules, and answers "where do I start".

## 1. The approach is right — and in this case the door does not have to be fake

The 2020s version of the test ("put up a mock-up, collect emails") works. But there is a better version
available now, and it is specific to this business: **the promise can be true on day one.**

- The landing page says *"send me one season's records and I'll send back the audit view."*
- That is deliverable **by hand, today**, with AI assistance, in hours — not a mock-up of a promise.
- So the same page tests demand **and** earns money **and** produces the specification, because every manual
  job shows which steps repeat and therefore what the product is.

That is a **concierge MVP with revenue attached**, and it beats a waitlist on every axis that matters here:
it fits the debt timeline (cash now, not in 12-18 months), it generates real leads, and it cannot be accused
of vapourware in a market that is already vendor-sceptical.

## 2. What to actually measure (emails are the weakest signal)

| Signal | Why it is better than an email address |
|---|---|
| **"Send me my records" clicks** | Behaviour, not intent. The strongest available signal short of payment |
| **Records actually sent** | The real conversion. Ten real uploads beat a thousand emails |
| **A qualifying question on the form** | "What do you keep records in? How many acres or head? Who does your spraying?" turns a list into leads and tells you the build order |
| **Paid first step** | The $750 assessment or a token pilot fee. Money is the only unambiguous yes |
| Raw email addresses | Weakest — free to give, no commitment, and they decay |

**Thresholds (directional; benchmarks are self-reported):** median waitlist conversion runs **~11%**, with
industry splits for cold-paid vs warm traffic. So with ~200 *qualified* visitors: **>10% is a real signal,
5-10% is ambiguous, <5% says the framing is wrong** (not necessarily the idea). **Zero visitors is not a
test at all** — and traffic source matters more than page quality. For this audience, warm beats cold: ag
communities, extension services, ag retailers and co-ops, LinkedIn. Cold paid traffic will burn money fast
against a farmer who is already tired of being pitched.

## 3. The suite question: one records layer, many output modules

Everything the research surfaced is the same shape — *records that already exist, plus a document somebody
is asking for*. So the suite is not a suite of apps; it is **one records store with per-job output modules**:

| Module | The output it produces | Trigger | Competitive check (checked 2026-10-11) |
|---|---|---|---|
| **Spray / application records** | The state/federal compliance record | **Legal: 40 CFR 170.311 requires 2-year retention** | **Weak spot.** The market leader "has all the data you need to be compliant" but is criticised for audit formats |
| **Audit binder (GAP, 3rd-party)** | Assembled records + corrective actions | Annual audit | Nobody owns this as a product |
| **Herd / treatment records** | Treatment and withdrawal logs | Food-safety and drug rules | cattleMAX etc. priced for registered herds — small commercial outfits excluded |
| **Mileage by state** | Fuel-tax filing | Quarterly/annual filing | Narrow, money-bearing, uncontested |
| **Equipment maintenance** | Service history, cost per machine | None (weak) | Crowded and low-urgency |
| **Landlord / custom-work billing** | Sharecrop and custom-work invoices | Monthly billing | **CONTESTED — see warning below** |
| **Farm accounting** | Schedule F package | Tax year | **CONTESTED and partly free** (Farm-Ledger free tier, nxtAcre, QuickBooks) |

**⚠️ The warning that changes the order.** My first instinct was to start with landlord/custom-work billing
because the invoice is money in the customer's pocket. **That niche is already taken:** Traction Ag does
"automatically create invoices from land agreements for sharecrop and custom work" (Pro tier only), Agnomy
does ag invoicing and payments with a 1% fee, and nxtAcre bundles invoicing with imports and multi-user
roles. Accounting is likewise contested and partly free. **Do not start there.**

## 4. Where to start: spray and application records → the compliance view

Ranked on four things that matter more than market size:

1. **A legal trigger rather than a preference.** 40 CFR 170.311 requires the application and hazard
   information be retained for **two years**; states often require more. A rule with a retention period is a
   deadline somebody can miss, which is what makes people buy.
2. **The incumbent demonstrably fails at exactly this.** Capture is solved; *output* is not — "unless you
   print off every application for every field you will not pass an audit."
3. **The current workaround is Excel and handwriting.** One farmer built his own workbook for it and gives it
   away free — the classic signal that the product is being invented by users.
4. **The deliverable is a document, so it can be demoed and delivered by hand today.** Upload a spray log,
   get the compliance view. That is the interactive demo *and* the manual service, with no gap between them.

**The one-line positioning:** *"You already have the spray records. This turns them into the report the
inspector asks for."*

### Names (descriptive beats clever for this audience)

Farmers search for the job, not the brand — so the H1 says the job and the domain can be short and literal.
Candidates for the first module: **SprayProof**, **SprayLog**, **ApplicationRecord**, **AuditReady**,
**FieldProof**. Umbrella names for the records layer: **RecordLayer**, **QuietRecords**, **FarmPaper**,
**TheBinder**. Keep whatever wins the *job* language in the headline either way.

## 5. The page and the demo, concretely

- **Domain:** one own domain (~$10-15/yr), static page on Vercel (already in use, free tier).
- **Page:** the job in the H1, three sentences of what happens, the offer ("send one season's records, get the
  audit view"), a form with **one qualifying question**, and an honest "in development — early access" line.
- **The demo:** one narrow transform, on *their* file. Upload Excel/CSV (and later a phone photo of a
  handwritten log) → return the compliance view as a PDF plus the extracted table. Honest limits stated.
- **Instrument it:** click-through on the offer, records actually submitted, and the qualifying answers.
- **Then:** do the first few by hand. Whatever you do manually three times is the product's first feature.

## 6. What this does to the plan

It adds an eleventh thread to [[concepts/side-income-map]] — a **product track tested with money attached** —
without displacing the near-term freelance work: the splash page and the free audit-view offer are the same
asset as the services page's agriculture variant, and the manual fulfilment is billable service work.
The service funds the product; the product is what the service keeps repeating.

## Open questions

- [ ] Which domain, and does the first module get its own or share an umbrella?
- [ ] Is the demo enough with Excel/CSV, or does it need photo capture of handwritten logs to land?
- [ ] Where does the first 200 qualified visitors come from — extension services, ag retailers, co-op
      networks, or the ag forums (read-only until standing is earned)?
- [ ] What token price makes the first paid step easy without being free? ($50 audit view? $250?)

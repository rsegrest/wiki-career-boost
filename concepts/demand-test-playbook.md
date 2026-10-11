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

---

## 7. What was built (2026-10-11)

**`~/code/2026/sprayproof`** — a new project with its own git repo, **local only** (no remote, nothing deployed).

- **Stack:** FastAPI + one static page, no build step. The domain core (`app/records.py`, `app/tiers.py`,
  `app/ingest.py`) is TDD'd — **14 tests passing** — and contains no framework code.
- **The pricing model, implemented exactly as decided:** free means importing records *and* seeing the whole
  compliance view on screen; **the exported document is the paid artifact**, tiered by **applications per
  year** (placeholders: $79 up to 250, $149 unlimited). The gate lives in one function (`app/tiers.py`) so the
  model cannot leak into the UI by accident.
- **Ingestion is permissive on purpose:** header synonyms ("Chem" -> product, "EPA Reg. No." -> EPA number,
  "Applied by" -> applicator), any common delimiter, unknown columns ignored, empty rows dropped, and nothing
  raises. A partially mapped row still teaches the user something, with the missing elements highlighted —
  because the customer will not retype data for anyone.

**Verified end-to-end, not just unit-tested:**
- `/api/view` on a three-row sample: 3 records, 2 complete, 1 incomplete, 96 acres, correct date range,
  `missing_fields_by_record={'3': ['product','epa_reg']}`.
- `/api/export` on free -> **HTTP 402** with the paywall reason; on $79 -> **HTTP 200** and a 955-byte document
  with the applications table and the incomplete-records section.
- The page itself: six sample applications -> 4 complete / 2 incomplete / 151 acres, four cells highlighted,
  two gaps listed, export locked and the paywall shown; selecting **$79/yr** enabled the export and cleared
  the paywall. Tiers render Free / $79 / $149.

**If this thread continues:** pick the name and domain (the placeholder appears in four places), deploy the
page plus the API, wire the form to collect **records** rather than emails, and add **photo capture of a
handwritten log** — that last one is what the research says farmers actually need and what no competitor
offers.

### Design direction (settled 2026-10-11)

The first build was dark with neon accents — a developer's aesthetic and the wrong signal for an agriculture
product. Replaced with a **printed-almanac** treatment, in Rick's words: wheat-coloured background, grassy
green and sky-blue accents, traditional and conservative layout, serif type, cues from the Farmers' Almanac.

- **Palette:** wheat paper `#f7f1e1`, panel `#fffdf6`, warm ink `#2f2a1e`, grass `#3f6f2a`, sky `#3d7ba1`,
  brick `#9c4227` for anything needing attention. No dark mode, no gradients, no glow.
- **Type:** **Bitter** (slab serif) for the masthead and headings, **Source Serif 4** for body text,
  small-caps letterspaced labels — with Georgia/Times fallbacks so it reads correctly even without webfonts.
- **Layout:** centred masthead between double rules, Roman-numeral section heads, boxed panels, a ruled ledger
  table (zebra rows, `†` beside each cell needing attention), figure boxes for the counts, a "seal" badge.
- **A print stylesheet, deliberately:** the input area, tier chooser and footer are hidden when printing and the
  ledger prints clean — because **printing the record is the product**. Verified: the print media query is
  present and four elements carry `no-print`.
- **Two visual languages, on purpose:** the product's own site speaks almanac; the agriculture landing page on
  ricksegrest.com stays in that site's existing language, because it is a portfolio page in a personal brand,
  not the product.

## 8. Naming (checked 2026-10-11)

**The problem:** `sprayproof.com` is taken. Almost every plain two-word descriptor is gone. Eighteen
candidates were checked against the Verisign registry for `.com`:

| Candidate | Status |
|---|---|
| sprayproof · sprayledger · sprayrecord · sprayrecords · spraylog · applicationrecords · fieldledger · fieldrecords · rowrecords · recordrow · cropledger · fieldbook · recordbinder · farmpaper · quietrecords · recordlayer | **taken** |
| spraybook · cropbook · rowbook · tankbook · ledgerbook · sprayjournal · cropjournal · fieldjournal · growerrecords · spraypaper · cropnotes · spraynotes · farmrecords · growerbook · ledgerrow · applicatorrecords (batch 2: all) | **taken** |
| **growerledger.com** | ✅ available |
| **furrowrecords.com** | ✅ available |
| **sprayregister.com** | ✅ available |
| **applicationledger.com** | ✅ available |
| **applicatorrecords.com** | ✅ available |

Alternative TLDs came back available for several strong names (`sprayproof.farm`, `sprayproof.ag`,
`growerledger.farm`, `sprayledger.farm`, `sprayledger.ag`) — but those checks are **less authoritative** than
the `.com` ones and must be confirmed at a registrar.

### Criteria that matter for this buyer

1. **Sayable on the phone** to a co-op or extension buyer, first try, no spelling out.
2. **No SaaS tells** — no `-ly`, `-io`, `-ify`, no dropped vowels, no hyphen or digit.
3. **Sounds like an object on a desk** — a ledger, a register, a book — not a platform.
4. **Generalises across the suite.** The product is one records layer with per-job outputs (spray,
   maintenance, herd, mileage). Naming it after spray boxes it in; naming it after the *record book* does not.
5. **A `.com` still earns its keep here** — this buyer types the address off a business card or a truck door.

### Recommendation

- **If naming the layer (recommended): `GrowerLedger.com`** — generalises to every module, farm-authentic
  wording, available. The module then reads as "GrowerLedger — Spray Records", and the page hero keeps
  naming the *job* rather than the brand (farmers search the job).
- **If naming the first product tightly: `SprayRegister.com`** — "register" is the word the regulation and the
  inspector actually use, so the name carries the compliance promise.
- `ApplicatorRecords.com` / `ApplicationLedger.com` are accurate but long: better as secondary domains that
  redirect than as the brand.
- **Not recommended:** splitting the brand from the domain (`Sprayproof` at `sprayproof.farm`). Two names for
  one small product is a cost with no upside for a conservative buyer.

**Confirm at a registrar before buying** — registry `WHOIS` says "available" but reserved, premium and
pending-delete states exist, and the `.farm`/`.ag` results above used looser matching than the `.com` ones.

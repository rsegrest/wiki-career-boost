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

### The Stokes option (2026-10-11)

Rick's own idea, and it beats the generic list on the criterion that matters most: **the phone test.** "Stokes"
is one syllable and spelled exactly as it sounds, where "Segrest" needs spelling twice. It is also his
mother's maiden name — his grandfather **John D. Stokes was a farmer** — which is a *credibility asset* in a
market that distrusts vendors: multi-generational family framing is respected in agriculture, and "named for
my grandfather, who farmed" answers "who are you?" in one line.

**Availability (Verisign registry, checked 2026-10-11):** `stokesagtech.com` (his pick), `stokesag.com`,
`stokesagriculture.com`, `stokesagservices.com`, `stokesagtechgroup.com`, `stokesfarmtech.com`,
`stokesagtools.com`, `jdstokesag.com` — all **available**; only `stokesfarm.com` is taken. That is a far
better field than the five-of-thirty-four result for generic descriptors.

**The caution, verified at the registry (TSDR, 2026-10-11) — and it is sharper than I first thought:**

- **"STOKES" is a LIVE, registered US trademark held by Stokes Seeds, Limited** (Thorold, Ontario):
  **Reg. 2,962,111** (filed Aug 2003, registered Jun 2005, **standard-character claim — the word itself in
  any font/style**) and **Reg. 3,040,436** (registered Jan 2006, a stylised/underlined-letter version). Both
  show **LIVE/REGISTRATION/Issued and Active**, both **renewed** (status dates Mar 2025 and Sep 2025), and
  both claim **acquired distinctiveness in whole** — i.e. the owner had to *prove* the mark is distinctive,
  which makes it a strong one. They have **counsel of record** (Barclay Damon LLP, Boston).
- **The scope that matters:** the goods/services are **"vegetable seeds and flower seeds", International
  Class 031 only.** Software is Class 9/42. So the registration does **not** cover what Rick would sell — the
  goods gap is wide.
- **But the industries are the same, and the customers overlap.** Stokes Seeds sells vegetable seed to
  commercial growers with four US locations including **LaBelle, Florida** and distribution up the Southeast.
  "Same field, different goods, same buyers" is exactly the shape of a confusion argument, and a mark this
  well maintained is one a lawyer would take seriously. Enforcement appetite against a one-person records app
  is very likely nil — but this is now a **judgment call with facts attached**, not a blank slate.
- Also in the same ear-space: **Stokes Agricultural Services Ltd** (UK, live company — so that *name* is
  taken even though the domain is free) and **Stocks Ag** (UK, one letter away).

**Recommended structure given all of that — and it reverses my earlier advice on one word:**

| Layer | Name | Why |
|---|---|---|
| Legal / umbrella | **Stokes AgTech** (`stokesagtech.com` ✅ available) | **"AgTech" is the distinguishing word.** It keeps the brand from reading as a seed company or as "Stokes Agricultural Services" — which is precisely the differentiation that matters now. My earlier instinct to drop it was about the *farmer's ear*; the trademark facts cut the other way. |
| Product | **Spray Register** (then Maintenance Records, Herd Records, Mileage Log) | Plainness belongs on the product name, where the farmer is deciding whether to trust it. "Register" is also the regulator's own word. |
| Story line | *"Named for John D. Stokes, who farmed."* | True, warm, and it answers "who are you?" in a market that asks. Keep it in the About/footer, not the logo. |

**A more conservative alternative if the surname in the brand feels too close:** **J.D. Stokes Ag**
(`jdstokesag.com` ✅ available) — the full personal name is a different source identifier from the bare
surname, and it tells the story harder.

**Buying:** own `stokesagtech.com` and, if it feels right, `jdstokesag.com` defensively with one redirecting.
Do not buy the six-variant set — that is $60/year for nothing. Confirm at a registrar (registry WHOIS is not a
purchase guarantee), and treat this page as research, not legal advice: an attorney's hour is the only real
answer, and that hour is not affordable this quarter.

**The one word I would drop: "AgTech."** It is the industry's own venture-capital vocabulary — farmers say
"the co-op", "the farm", "the seed guy", never "agtech" — and for a buyer who is tired of vendors it quietly
says *startup that may not exist next year*. Fine as a legal holding name; the wrong thing on a truck door.

**Recommendation:** umbrella **`StokesAg.com`** (short, sayable, region-appropriate, available), with modules
reading plainly underneath — **"Stokes Ag — Spray Register"**. Own `stokesag.com` *and* `stokesagtech.com`
(cheap), redirecting one. Name the module with the regulator's word rather than the invented one, and retire
"Sprayproof" now that its .com is gone.

**Routing for the umbrella (his "individual apps under the brand" idea):**
- **v1 — one domain, path per module:** `/spray` now; `/maintenance`, `/herd`, `/mileage` later. Simplest on
  Vercel, consolidates brand and search authority, and the app already serves one page at `/`.
- **Later — promote a module to a subdomain** (`spray.stokesag.com`) only once it earns its own traffic;
  exact-match module domains can simply redirect to it.
- On the app side that means a small **module registry** (route -> app) rather than a rewrite, which is the
  right time to add it: when the second module arrives, not before.

### The John Deere question (2026-10-11)

Rick's hesitation about "John D. Stokes" / "J.D. Stokes": fear of John Deere's legal team. Two precision
points and one finding that cuts his way.

**Terminology matters here:** this is **trademark**, not copyright. Trademark asks whether two marks, taken
*as wholes*, are likely to be confused for the same source of goods — not whether one copied the other.

**What Deere actually owns (checked 2026-10-11):**
- **"JD" — Reg. 1,062,200**, owned by Deere & Company, a typeset word mark filed 7 Jan 1975, registered 1977,
  **status: DEAD / expired as of 5 Jan 2008.** That registration has lapsed.
- **A new "JD" application was filed by Deere on 31 Aug 2026** — pending, and the aggregator that surfaced it
  gates the goods/services behind a subscription, so the classes are **unverified**. The takeaway is that they
  are actively filing for the initials again, not that a live registration covers software.

**What Deere actually litigates:** the **green-and-yellow trade dress.** In 2017 a Kentucky federal court
held that FIMCO's use of green and yellow on **sprayers and wheeled agricultural equipment** infringed and
diluted Deere's marks, finding the colour combination "famous" since the late 1960s. Note the adjacency: the
loser made **sprayers**.

**Reading it as a mark:** "J.D. Stokes" and "JOHN DEERE / DEERE / JD" share only a common given-name initial,
which is not itself protectable; the dominant, distinctive element of Rick's name is the surname **Stokes**,
which has no relation to Deere. Different dominant element plus different goods (records software, not
equipment) makes confusion unlikely, and a *dilution* claim over a records app named for someone's
grandfather is a stretch. Deere's enforcement energy goes at equipment makers, counterfeit parts, and use of
the deer logo or the green-yellow dress — not at a one-person software product. Realistic worst case is a
letter, not a lawsuit.

**But three cheap rules if he uses the name:**

1. **Never render it as "JD."** Always spelled out — "J.D. Stokes" — and no block-letter monogram. The
   initials alone are the element Deere claims.
2. **No green-and-yellow signature.** This one touches *our own palette*: brand green `#3f6f2a` paired with
   mustard `#c1912a` sits in the neighbourhood of Deere green/yellow. Recommendation if a Stokes/J.D. name is
   used: make **wheat + brick + sky** the identity, keep green for rules and text, and drop mustard from the
   masthead. (For software the trade-dress risk is much lower than it was for a sprayer manufacturer — but the
   fix costs nothing.)
3. **Avoid Deere product names for modules** — not "Operations Center", "GreenStar", "AutoTrac", "StarFire".

**The structure this now points to.** Three separate collisions have accumulated around the surname — Stokes
Seeds holds a live Class-31 STOKES mark in the same industry as the buyers; "Stokes Agricultural Services Ltd"
takes that company name; Deere claims the JD initials and polices green-and-yellow. So:

| Layer | Name |
|---|---|
| **Brand / wordmark** | **Stokes AgTech** — distinctive composite, no initials, no colour claim |
| **Story (About + footer)** | *"Named for John D. Stokes, who farmed."* |
| **Products** | Spray Register · Maintenance Records · Herd Records · Mileage Log |

Using the personal name as a **story** rather than a **logo** preserves the family meaning, drops both risks
to near zero, and requires no colour gymnastics. If he wants it more visible, "the J.D. Stokes line of record
books" works as a product-family label — spelled out, no monogram.

*(A clearance search for "J.D. Stokes" as an existing business returned nothing, but the search backend was
flaky on that call — treat it as inconclusive, not clear.)*

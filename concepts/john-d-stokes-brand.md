---
title: John D. Stokes — Agricultural Records (brand)
created: 2026-10-11
updated: 2026-10-11
type: concept
tags: [brand, design, naming, identity, logo, agriculture, product]
sources: [user direct input 2026-10-11, TSDR registry checks 2026-10-11, Verisign whois 2026-10-11, concepts/demand-test-playbook.md]
confidence: high
---

# John D. Stokes — Agricultural Records

> **Why this page exists:** the single source of truth for the brand — the name and its story, the palette and
> what each colour *means*, the type, the logo direction, and the rules that keep it out of trouble. Builds on
> [[concepts/demand-test-playbook]] §8, which holds the naming research and the legal checks.

## The name

**John D. Stokes — Agricultural Records**, first module **Spray Register**.

Named for Rick's grandfather, **John D. Stokes, a farmer**, whose farm outside **Andalusia, Alabama** is where
he spent childhood summers. The full name was chosen over the surname alone, and over the initials, for three
reasons that all point the same way:

1. **It passes the phone test** — one syllable, spelled as it sounds, unlike "Segrest".
2. **It avoids the initials ("JD"), which is the element John Deere actually claims** — so this is *lower* risk
   than "J.D. Stokes", not higher.
3. **A full personal name is a more distinctive identifier than a bare surname**, and the use is *truthful* —
   it is his grandfather's actual name. Best possible footing if ever questioned.

`johndstokes.com` is available (registry-checked), and no software or agriculture business uses the name.

## The palette — the Stokes farm palette

| Role | Colour | Hex | Meaning and placement |
|---|---|---|---|
| **Anchor** | Denim blue | `#2f4a6b` (light `#3f6489`) | "He usually wore overalls." Masthead band (with a cotton-twill weave), headings, primary button, ledger header |
| **Ground** | Boiled-peanut tan | `#ece0c8`, panels `#fbf6ea` | The paper. Warm and printed, not office-white |
| **Attention** | Watermelon red | `#b8393d`, tint `#f8e5e4` | **Semantic only** — cells needing attention, the inspector's flags, errors |
| **Tally** | Sugarcane yellow | `#d3b055`, tint `#faf2da` | The ledger's totals row — the one "gold" moment |
| **Complete** | Butterbean green | `#557033`, tint `#eef3e2` | **Semantic only** — the "complete" figure, the middle plan tier |

Every colour is a crop or a garment from that farm. **Red and green always mean something and are never
decoration** — which also guarantees that green and yellow never pair as a *signature*, the combination Deere
successfully litigated in 2017 (FIMCO, green-and-yellow sprayers). The Deere trade-dress risk is therefore
structurally avoided, not merely avoided by discipline.

**Contrast verified in code, not by eye:** every body-text pair is ≥4.5:1. Two failed the first pass and were
darkened automatically — muted labels `#857c66`→`#6f6655` (3.84→5.25) and green text `#6b8b47`→`#557033`
(3.43→4.95). Body on paper 11.0:1; ecru on denim 8.05:1.

## Type

**Bitter** (slab serif) for the masthead, headings and buttons; **Source Serif 4** for body text;
small-caps letterspaced labels for descriptors. Georgia/Times fallbacks so it reads correctly without
webfonts. A serif identity is the point: it reads as a printed record, not a dashboard.

## Logo direction

**The rule that matters most: never ask an image model to render the company name.** Letterforms come out
mangled. Generate the **mark only**, then set the wordmark in Bitter beside it. A lockup is mark + name + a
sugarcane rule + the descriptor in small caps.

**On "communicating software":** circuit boards, node graphs, gears and robots read as *technology* to a
founder and as *something that will break* to a farmer. The tech signal belongs in the typography, the
descriptor line, and above all in how fast the thing works. Each mark below therefore says **records** or
**verified** first — a promise this product can keep.

Five marks are drawn and rendered at real sizes (96 / 48 / 24 / 16 px plus one-colour) on a local design page:
`/static/design/logo-options.html` in the app, file `static/design/logo-options.html`.

| Mark | Concept | Reads as | Weakness |
|---|---|---|---|
| **A** | Ruled page, one row flagged with a watermelon check | *a record book, with something to look at* | page-outline marks are the most common "document app" shape there is |
| **B** | Field rows rising like a chart (furrows that are bars) | *agriculture and data at once* | least literal of the five |
| **C** | A check mark in a denim square | *done and verified* | says "complete", not "records" |
| **D** | Page with a folded corner and a flagged line | *a document, digitised* | the folded corner is a 2010s app-icon cliché |
| **E** | JS monogram in denim | *a firm* | least informative; easiest to protect |

**Recommended for the masthead: B or C.** B carries the farm and the data; C is unbeatable small and prints
like a stamp. Both are one-colour safe.

### The descriptor carries the category — in type, not in artwork

Rick's requirement: seeing the logo should show what the company *is* ("Ag Tech"), while the mark itself stays
non-tech-themed. That is a **lockup** job, not a mark job — and it is the right split. Four variants are drawn
on the design page:

1. **Horizontal** — mark · `John D. Stokes` · sugarcane hairline · `AG TECH`. For the masthead and letterhead.
2. **Stacked** — mark above `John D. Stokes` above a sugarcane rule above `AG TECH`. For a stamp, a seal, a sign.
3. **Company style** — one line, `John D. Stokes` with `AG TECH` as a letterspaced suffix. Reads as a firm name;
   right for a signature block, an invoice footer, an email sign-off.
4. **Descriptor beneath the name** — `Ag Tech · Agricultural Records`: category *and* function. Worth the width
   on a landing page, too long for a business card.

**The degradation rule, fixed:** the descriptor is **dropped before it becomes unreadable**, never squeezed
until it is. Full lockup at 48px and up → tightened (name + small descriptor) at 24-48px → name only at
16-24px → **mark alone** for the favicon and app icon. The design page shows all four steps side by side so the
hand-off is unambiguous.

## Production path

A generated raster mark goes mushy when scaled. So: generate candidates with an image model, pick at **16px
first** (if it does not read there it does not work), then **redraw the winner as a hand-coded inline SVG** —
crisp at every size, locked to the palette, with a one-colour version for print, a stamp or a fax header, plus
a favicon. That is a small job and it is the difference between a logo and a picture of one.

---

## Locked palette (2026-10-11) — from the brand sheet

The identity sheet Rick commissioned (ChatGPT, filed in the project at `brand/`) is now the source of record.
Its swatches are labelled by name and *meaning*, not by hex, so these values were **sampled from the artwork**:

| Role | Colour | Value | Where it came from / how it is used |
|---|---|---|---|
| **Anchor** | Denim Blue | **`#0a2136`** | The crest field — deepest navy on the sheet. Masthead band, headings. |
| └ secondary | Denim Blue (light) | `#1c4a70` | Links, hover, the lighter navy of the wordmark (`#132c3a` sampled from the lettering) |
| **Ground** | Cream | **`#f9f7f0`** | Text on navy (15.3:1), panels |
| └ paper | Warm cream | `#f6f1e6` | The page itself |
| **Ground / ornament** | Peanut Tan | **`#988c72`** | Rules, borders, ornament — never body text (2.95:1, so it fails for text and is used only as surface and rule) |
| **The single green** | Cane Green | **`#405830`** | The one green of the set: "complete" state, the wordmark's *AgTech*, rule accents (7.0:1 as text) |
| **Attention** | Watermelon Red | **`#b84040`** | Cells needing attention, the inspector's flags, errors (4.85:1) |
| **Trim / tally** | Hay Gold | **`#e4b472`** | The crest's trim and stitch (8.6:1 on navy), and the ledger's totals row as a tint `#faf0dd` |

**Every body-text pair clears 4.5:1** — lowest is watermelon at 4.85, then greens at 7.0, links at 8.9, body
text at 13.9, cream on navy at 15.3.

**Blueberry is retired from the palette.** Rick's own note: his grandfather grew blueberries in the garden for
the family, and it is a significant memory — which is precisely why it belongs in the *writing* rather than in
a swatch. The recollection already lives in the memoir chapter about summers at Granddaddy's farm outside
Andalusia; a colour chip in a style guide is a poor place to keep it. *(If a fifth accent is ever needed, it
can come back as a small non-brand tint — but not now, and not as brand.)*

**The reversed logo on navy is the primary treatment** (Rick's preference), and the app's masthead already is a
deep-navy band, so the crest slots straight in with no redesign. The positive version on cream remains for
print, where a wall of navy would be expensive ink.

## Wordmark type

The sheet's wordmark is closest to **Bookmania** (Mark Simonson Studio) — a commercial family with 20 styles,
available as a self-hosted **web licence** from the studio or through **Adobe Fonts**, which includes it with a
Creative Cloud plan. For a product that has not earned a dollar yet, the free routes are:

| Font | Licence | Note |
|---|---|---|
| **Rye** | Free (OFL, Google Fonts) | Rick's suggestion. Wood-type western — spurs and slab serifs, the barn-sign/feed-store flavour the crest already speaks. Best marriage with the crest; **one weight, no italic**, and decorative rather than quiet at small sizes. |
| **Vollkorn** | Free (OFL, Google Fonts) | The closest free match to Bookmania (**82%** per font-alternatives), and it does everything: wordmark, descriptor, tagline, table headings, real italics. |
| **Bitter** | Free (already in the app) | Clean slab serif, least characterful, and what the current lockups and tables were built around. |

**Recommended split:** **Rye for the wordmark, Vollkorn (or Source Serif) for everything else** — character where
it is wanted, quietness where legibility matters. If Bookmania is licensed later, Vollkorn is a straight swap
and almost nothing else changes. All four candidates are rendered head-to-head in the lockup at masthead size
*and* at the small size on the design page (`/static/design/logo-options.html`), because a display face has to
survive the small lockup, not just the big one.

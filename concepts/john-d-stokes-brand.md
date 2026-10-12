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

---

## Logo files and the reversal (2026-10-11)

Rick produced the logo as **SVG** and separated the composite (PSDs for the palette, the secondary icons and
the dark-background logo, plus GIF previews) — all filed in the project under `brand/`. His SVG is not just the
crest: it is the **full lockup** — shield, `JOHN D. STOKES`, `AgTech`, and the tagline **"AGRICULTURAL SOFTWARE
& TECHNOLOGY"** *(verified from the SVG's own text node; a vision read of the raster said "Innovation" and was
wrong)* — sitting on an opaque cream panel, which is why it read as a cream tile when dropped on navy.

**Built four variants from his artwork:**

| File | What | Use |
|---|---|---|
| `johndstokes_logo-light.svg` | his original — cream panel, navy ink, green *AgTech*, navy shield with cream/green/gold internals | print, letterhead, invoices |
| `johndstokes_logo-on-navy.svg` | reversed — navy panel, cream lettering, and the shield becomes a **cream badge** with navy/green/deep-gold internals | the primary dark treatment; the masthead |
| `mark.svg` / `mark-light.svg` | crest only, no lettering, no panel (reversed / positive) | the masthead band, app icons / print |
| `static/favicon.svg` | navy tile + shield silhouette + stitch | the browser tab |

**Two lessons worth keeping:**

1. **Inverting a badge kills its gold trim unless the gold moves with it.** The first pass flipped the shield to
   cream but left the stitch at `#e2b561` — gold on cream is **1.78:1** and effectively disappears. The fix is
   context-aware: the crest's golds deepen to **`#9a7328`** (4.03:1 on cream), while the rules flanking *AgTech*,
   which sit on navy, stay bright at `#e2b561` (7.7:1). Same family, two values, chosen by background.
2. **A navy badge on a navy panel survives only on its outline** — the first alternative relied on a 1.1px cream
   outline and would fail at small sizes, so the cream-badge version won.

**Wired into the app:** the reversed crest sits in the navy masthead above the live-type wordmark, the
descriptor now reads the brand's own line (*Agricultural Software & Technology*), a `favicon.svg` carries the
shield and stitch at tab size — the full crest is too dense at 16px, so only the two elements that survive are
in it — and the print stylesheet swaps to the light crest. Verified in the browser: the artwork loads, serves
200 as valid SVG, the light variant is hidden on screen and shown in print, and the app still works.

---

## Separated assets and the composed lockup (2026-10-11)

Rick separated the artwork into production pieces, Letter-sized (612×792): **`logotype.svg`** (the wordmark as
outlines, 58 paths) and **`overall-pocket-logo.svg`** (the crest, 29 paths). Both are **class-coloured** — the
palette lives in a `<style>` block (`cls-1`…`cls-8`), not in inline fills — which is the right way to ship a
logo: a variant is a stylesheet edit, not a shape edit.

**What was built from them** (all in `brand/`, mirrored into `static/brand/`):

| File | What |
|---|---|
| `wordmark-light/dark.svg`, `mark-tight-light/dark.svg` | each piece tightened to its ink bounds (measured from the rasterised alpha channel, not guessed from path data) and recoloured for its ground |
| `lockup-light.svg`, `lockup-on-navy.svg` | the composed lockup: crest above wordmark, proportions taken from Rick's original single-file logo |
| `static/favicon.svg` | navy tile + the shield silhouette + the stitch — the full crest is too dense at 16 px |

**Two traps worth recording:**

1. **Two SVG files with `cls-1`…`cls-4` will silently overwrite each other's palette when composed.** Both of
   Rick's files use the same class names, so dropping them into one document made his wordmark's *bright* gold
   rule apply to the *crest* as well — resurrecting the exact gold-on-cream stitch defect (1.78:1) that had
   already been fixed. The fix is to namespace the classes per source (`mk-cls-*`, `wd-cls-*`) and rewrite both
   the selectors and the `class` attributes. **Verified numerically afterwards**: in the composed lockup the
   crest's golds measure `#907020` (deep) while the wordmark's rules measure `#d0b050` (bright) — two values,
   each on the ground it was chosen for.
2. **Letter-sized artboards carry 6-decimal coordinates.** Rounding path data to two decimals cut the files by
   roughly half with no visible change, and the artwork now declares intrinsic width/height so browsers and
   link previews size it correctly.

**In the app:** the masthead now shows the real lockup — crest, wordmark, *AgTech*, gold rules and the tagline,
all from the artwork — with a visually-hidden `<h1>` carrying the words for search engines and screen readers,
and the print stylesheet swapping to the light lockup. The crest alone stays available for app icons.

---

## Type: the wordmark is outlines, so the font question changes (2026-10-11)

Rick confirmed the wordmark was **not generated from a specific font** — Bookmania and Rye were *similar*, not
sources. That settles the licensing question in the best possible way: **a logo shipped as outlines needs no
font licence at all**, and it can never be re-rendered wrongly by a system that lacks the face. The outlines in
`logotype.svg` are the definitive wordmark.

What the font question actually reduces to is the **supporting type** — the text set *around* the mark, which
still needs a face for headings, descriptors, tables, email signatures and invoice footers. Decision:

- **Vollkorn** (free, Google Fonts) — supporting display face: headings, buttons, table figures, descriptors. It
  is the closest free relative of the bookish, high-contrast, swashy lettering in the mark, so the page and the
  logo read as one family without a licence.
- **Source Serif 4** (free) — body text.
- **Rye is dropped.** It was only ever a candidate for *imitating* the wordmark; with the wordmark fixed as
  outlines, Rye has no job, and as a western wood-type it would clash rather than harmonise.
- **Bookmania remains optional**, and only if Rick ever wants the exact wordmark as *live text* (a typed
  signature, a one-colour fax, editable collateral). Until then, outlines cost nothing.

**Design review of the app after the change** (screenshot read against the brief) caught two real defects:

1. **The drop cap was broken** — the initial letter was enlarged but its float box was only one line tall, so the
   second line still started at the left margin. Fixed with an em-based size and a float box measured to span
   two body lines (52.7 px glyph against a 27 px line).
2. **The masthead was too tall.** The lockup is now 252 px (was 330) with the band's padding reduced, bringing
   the content up ~60 px.

Also tightened the space under the section rules. Verified: the lockup loads, Vollkorn is live on headings and
buttons while body text stays Source Serif, and the app still returns 6 applications / 2 flagged.

---

## Reviewing your own work with a model's eyes — and knowing when to disbelieve it (2026-10-11)

A screenshot of the app was read back against the design brief. It produced three findings; **one was real and
two were wrong**, which is the useful lesson.

**Wrong #1 — the drop cap "isn't wrapping".** Reported twice, so rather than take it on faith the paragraph was
measured: the x-position of the first word on every rendered line. Line 1 starts at **197** (the paragraph's own
left edge, with the `P` *being* the drop cap), lines 2 and 3 indent to **261** and **231** to clear it, and lines
4 and 5 return **flush at 197**. A correct two-line wrap. The reviewer had mistaken the paragraph's own left
margin for an indent and described a "hanging indent" that does not exist.

**Wrong #2 — "AgTech green is a contrast failure."** It measures **5.13:1** on the navy: it passes AA, and it is
simply the *least* contrasty element, which is a different thing from failing.

**Right — the file input was raw browser chrome.** A "Choose File / No file chosen" native control sat next to a
designed button. It now reads as a pair: a Vollkorn **"Open a spreadsheet…"** button, an "or", and a filename
readout. Verified end-to-end by feeding a real CSV through the control (3 rows → 3 applications, 0 flagged).

**The rule:** a vision model is worth consulting for *composition and hierarchy*, where it is genuinely useful,
and not for *measurements* — spacing, contrast ratios, line wrapping — where it will state a number-shaped
opinion with total confidence. Measure the DOM, or don't claim it.

---

## CORRECTION — what "swap the background and logotype colours" actually means (2026-10-11)

Rick's correction, and it was a real error on my part: **the crest is also an overalls pocket.** Its field is
denim blue on purpose, so turning that field cream destroys the association. And the crest's **leaf is cream** —
which my inversion turned navy, i.e. a blue leaf, which is not a colour a leaf can be.

**Read the instruction literally. It names two things:**

1. the **background** — the cream panel becomes navy;
2. the **logotype** — the navy lettering becomes cream.

**Nothing else.** The crest keeps every colour it has: denim pocket field, cream leaf, green and tan field rows,
gold stitch. Flipping the crest was never asked for, and it was my mapping that did it — I inverted navy↔cream
*across the whole composition* instead of applying the swap to the two named elements.

### The reference, measured

The composite Rick likes (`source-art/logo-dark-bg.gif`) was sampled on a 14×10 median-colour grid rather than
described:

| Region | Measured | Reading |
|---|---|---|
| Shield field | `#051b32`, `#072137`, `#051e32` | **navy denim — essentially the same value as its background** |
| Leaf and rows | `#5c7843` → `#93a961` | a mid-to-light green, lighter than the greens in the SVG |
| Field rows, trim | `#a97c4b`, `#c99e5b`, `#b3945b` | tan / gold |
| Lettering | `#dbd7c7`, `#f0e7d0` | cream |
| Background | `#082138`, `#0d263a`, `#072137` … many near-identical navies | **a woven denim texture**, not a flat fill |

**The consequence is the design rule worth keeping: the pocket does not read by contrasting its field against
the background — it cannot, they are the same navy. It reads on its stitched border, its rivets and its interior
motifs, over a woven ground.** So do not try to "fix" that merge with a lighter pocket; the weave and the stitch
are doing the work. The app's masthead already carries a `repeating-linear-gradient(45deg, rgba(255,255,255,.05))`
weave, which is exactly that ground.

### Lesson for any logo work from a written brief

**A swap names its targets.** When an instruction says to exchange two things, exchange those two things and
leave every other colour alone. An image-wide inversion is not the same operation, and on a mark that carries
meaning in its colours — a denim pocket, a cream leaf — it destroys the meaning while still looking
"reversed" and plausible. When the elements are already separated into files, the swap should be applied per
element, never to the composition as a whole.

---

## Pocket on the left, and a solid rule around the stitching (2026-10-11)

Two changes Rick asked for, and both turned on geometry worth recording.

### How the solid outline is built

The stitching is **not a dashed stroke** — `cls-8` is two filled paths (d = 9,551 and 2,369) made of
individually drawn dashes, traced along the pocket's seam. Measured, the pocket's own edge (`cls-1`, the path
enclosing the stitch contour) is **446 × 409**, and the dashes sit **~13 units inside it**. So a solid line
around the stitching is simply the pocket's edge path, duplicated, `fill:none`, stroked in the chosen tan/gold
(`stroke-width 3.2`) — placed last so nothing can cover it. It lands about 13 units outside the dashes, with no
offset maths and no hand-tracing. **Stitching that is drawn as dashes can always be outlined by stroking the
contour the dashes follow.**

Two traps, both caught before shipping:

1. **An outward-offset element is clipped by a tight viewBox.** The crest had been tightened to its ink bounds,
   so the version whose line sat *outside* the edge had only 1–2 px visible at the artboard boundary. Any variant
   that adds ink outside the existing bounds needs the viewBox padded first (now 6 units on every side).
2. **Namespacing classes twice kills the stylesheet.** Composing the crest and the wordmark namespaces each
   file's `cls-N` classes so their palettes cannot collide — but applied twice it produces `wd-mk-cls-1`, which
   matches no rule, so the fills fall back to the SVG default: **the wordmark rendered black on navy**, i.e.
   invisible. Namespace exactly once, at extraction, with the prefix chosen there. Verify by colour census
   (cream 14,172 px + green 5,009 px, zero black), not by eye.

### The horizontal lockup

The pocket goes left of the logotype, and it is centred on the **name + AgTech block**, not on the whole
wordmark: measured, the wordmark's ink splits at viewBox rows `2–208` and `215–229`, so the descriptor is its own
small block below. Centring the pocket on everything drags it down and leaves the mark sitting low; centring it
on the main block lets the descriptor hang beneath, which is how a horizontal lockup normally reads.

Result: the masthead is now **187 px** tall instead of 266 — the horizontal lockup solved the height problem as a
side effect. Print uses the horizontal light lockup with the outline deepened to `#9a7328` so it carries on
cream. Files: `lockup-horizontal-{gold,tan,peanut}.svg`, `lockup-horizontal-light.svg`,
`crest-outline-{gold,tan,peanut,light}.svg`.

---

## Locked: pocket left, peanut tan rule (2026-10-11)

Rick's choice for the masthead: **horizontal lockup, pocket to the left, peanut tan `#988c72` outline.** Now in
`lockup-horizontal-peanut.svg` (the app masthead) with a print companion in the same colour
(`lockup-horizontal-light.svg`, on cream). The gold and `#c99e5b` variants stay on the design page for other
applications.

Measured: the rule holds **4.93:1** on the navy band and **3.10:1** on cream — over the 3:1 bar for a graphic,
consistent with the palette rule that peanut tan is for rules and borders and never for text.

### A line weight is a production decision, not a detail

The first version drew the rule at **3.2 units** on a 446-unit pocket — 0.7% of the crest's width, which is
**1.4 px** at the 430 px the masthead actually renders. Sampled, its pixels came back as antialiased blends
(`#867e6a`, `#2b3a44`, `#4d5655`) rather than the tan: a grey smudge, not a line. At **5.0 units** it becomes a
crisp ~2 px rule (4–5 device px on a retina display) with solid `#988c72` pixels present.

**The lesson: judge a stroke at the size it will be rendered, never in the source file's own units.** A rule
that looks correct in the SVG's coordinate space can be invisible in the product. Render at product size, sample
the pixels, and check the colour is actually there.

### The variant build is now a script

`brand/build-variants.py` regenerates every crest and lockup from the source artwork: `OUTLINE_WIDTH`,
`PAD`, `CREST_RATIO`, `GAP_RATIO` and the `OUTLINES` colour table at the top, everything else derived. It
carries the two traps in its own comments — namespace `cls-N` exactly once (twice yields selectors that match
nothing and the fills fall back to black), and pad the viewBox for any element that extends past the ink
(`PAD = 6`).

---

## The brass rivets get a recessed centre (2026-10-11)

Rick's suggestion: a smaller darker dot inside each brass rivet reads as a rivet rather than a dot. Correct —
a flat disc of gold is a dot; a snap fastener shows a ring of brass with a darker recessed centre.

Built as **`cls-9`**, a new class in the crest's own stylesheet: `fill:#a97c4b` (the darker brass measured off the
composite), a circle at **40% of the rivet radius**, concentric with each `cls-6` rivet and drawn after it. Two
dots, r = 6.13 against a rivet radius of 15.3. Verified on rendered pixels rather than assumed: rivet centres
read **`#a97c4b`** inside rings of **`#d2a54d`**.

At the 430 px the masthead renders, a rivet is ~13 px across and the dot ~5 px — so it reads at masthead size and
above, which is what Rick asked for; he has explicitly parked the favicon, where a line or dot of this size is
sub-pixel anyway. It lives in `build-variants.py`, so every variant gets it.

**One process lesson: a string replacement that does not match fails silently.** The first attempt to add the
dots targeted a double-quoted line that was in fact single-quoted, so the edit did nothing — the stylesheet
gained a `cls-9` rule that no element used, and the build kept reporting success. The tell was a count
(circles emitted: 0, expected 2). Assert the anchor exists before replacing, and verify the artefact contains
what you meant to add — a build that says "done" is not evidence.

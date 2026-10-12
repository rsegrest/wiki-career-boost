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

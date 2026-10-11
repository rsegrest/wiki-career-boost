---
title: Services Page — copy for ricksegrest.com
created: 2026-10-11
updated: 2026-10-11
type: concept
tags: [marketing, services, website, freelance, sales, ai]
sources: [user direct input 2026-10-11, concepts/freelance-outreach-targets.md, writing/voice-profile.md (personal vault)]
confidence: high
---

# Services Page — copy for ricksegrest.com

> **Why this page exists:** the outreach plan needs a place to *send* people. This is the sales asset:
> a business page that shows **applications and outcomes**, not technologies, written so a non-technical
> owner or manager recognises their own week in it. Companion to
> [[concepts/freelance-outreach-targets]].

## The rule for this page

**Show what it does and why it is worth having; never name the machinery.** No model names, no
"RAG/embeddings/agentic/LLM/pipeline" — those words cost credibility with this reader. Every item is
written as **a job role's bad week, then that week fixed**, with the value stated in hours or dollars and
labelled as an estimate. Reuse the personal vault's voice rules: no hype adjectives, no AI-vocabulary
words, plain sentences.

## THE COPY (ready to publish)

### Hero

**Small AI tools for the paperwork your business already has.**

I build focused tools around the documents and forms your team already works with — contracts, invoices,
intake forms, maintenance logs, compliance records. Nothing new to learn, and nothing has to leave your
network.

*Fixed scope. Fixed fee. Working software in two weeks.*

### Six things this looks like

**1. The contract pile**
*Before:* contracts live as PDFs in folders. Nobody knows what auto-renews, what the obligations are, or
when the next deadline lands — until it is late.
*After:* every contract is read once. Dates, obligations and renewal terms land in one simple table you
can ask questions of — "what terminates in the next 90 days?" — and every answer points back to the page
it came from.
*For:* a general counsel, a purchasing manager, an office manager.

**2. The invoice pile**
*Before:* someone matches invoices to purchase orders and packing slips by hand. Duplicates slip through,
and small overcharges go unnoticed because finding them costs more than they are worth.
*After:* invoices are matched automatically. The ones that disagree are flagged with the reason, and
duplicates are caught before payment.
*For:* a controller, a bookkeeper, an accounts-payable clerk.

**3. The forms nobody wants to type**
*Before:* paper intake forms, faxed logs, handwritten service sheets. Once filed they are effectively gone
— nobody searches them.
*After:* every form becomes a searchable record. Ask "when was pump 3 last serviced, and what did it say?"
and get the answer with the original page attached.
*For:* operations managers, clinic and shop front desks, maintenance leads.

**4. The emails that repeat all day**
*Before:* fifty near-identical replies a day — quotes, scheduling, status requests, directions. It never
gets done because it keeps arriving.
*After:* drafts written in your own voice, waiting for you to approve or edit. You stay in control of
every message that leaves.
*For:* sales, customer service — anyone with an inbox.

**5. The audit binder**
*Before:* two weeks of scrambling before every audit, every year — records pulled from four places, hoping
nothing is missing.
*After:* the records assemble themselves, and the corrective actions you took stay linked to the problems
they fixed, so you can prove the fix stuck rather than just that you wrote it down.
*For:* quality managers, compliance officers, plant managers.

**6. The thirty-year veteran's head**
*Before:* the person who knows how everything works retires, and the knowledge leaves with them. New staff
interrupt the remaining veterans all day, every day.
*After:* an assistant that has read your procedures, work orders and past fixes answers new staff in plain
language — and says "I don't know" when it doesn't.
*For:* any business with long-tenured staff.

### Why this is safer than it sounds

- **It can run on your network.** These tools can be built to run entirely inside your own network, so the
  documents never leave it. Where a cloud service is involved, that is a decision you make deliberately,
  not a default you inherit.
- **You approve what goes out.** Nothing is sent, filed, ordered or paid without a person clicking the
  button. Drafts stay drafts.
- **Your systems stay.** Nothing here replaces your ERP, your accounting package or your shared drive. It
  reads from them and fits alongside them.
- **You can walk away.** No lock-in, and no proprietary format holding your records hostage.

### How engagements work

1. **One-day assessment — $750.** I read your documents and watch the workflow for a day, then tell you
   where the hours actually go and which fixes are worth doing. You get the written plan whether or not we
   work together again.
2. **Two-week build — $3,500.** One fixed-scope tool, working in your environment, on your real documents.
3. **Ongoing — only if it earns it.** If it saves what we said it would, we discuss the next one. If it
   does not, we stop.

### Who I work with

Professional services, insurance, logistics, manufacturing, agriculture — any business whose work runs on
documents. **Commercial networks only:** no government, ITAR-controlled or export-controlled data.

### About

Twenty-plus years building software for engineering teams, much of it for NASA's engineering
organisations, where being wrong is expensive and "probably right" is not good enough. Now I build the
same kind of careful tooling for the paperwork that runs small and mid-size businesses.

### Next step

A 30-minute conversation. Tell me what your team spends its time on; I will tell you what I would try
first — and if the honest answer is "nothing here is worth it", I will say that too.

## Build notes (where it goes)

- Site: `~/code/2026/portfolio-gallery` — repo **rsegrest/ricksegrest.com**, branch `master`, Vite + React +
  TypeScript, deployed on Vercel.
- Add `src/pages/ServicesPage.tsx`, register the route alongside the existing pages
  (`HomePage`, `AboutPage`, `ProjectPage`, `ResumePage`, `BlogListPage`, `BlogPostPage`), and add a
  **Services** link to `src/components/NavBar.tsx`.
- **Phase 2 (the part that actually impresses):** a small interactive demo — drop in a sample contract and
  watch the dates and obligations come out. The site already serves static demos from `public/demos/`
  (`vector-display`), so there is a pattern to follow.

## Open questions

- [ ] Does the page lead with the assessment price ($750) or leave pricing to the conversation?
- [ ] Add a one-line case study once the first pilot ships? *(Nothing to show yet — do not invent one.)*
- [ ] Should the six scenarios be reordered by industry for the ag/co-op conversation specifically?

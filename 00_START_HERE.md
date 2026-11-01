# Tepenian Language — start here

*Formerly named TepenianHawaiian (renamed 2026-11-01, D-24 Repo renamed Tepenian Language). Decisions logged before the rename keep their original wording.*

**What this repo is.** The research, synthesis and record of **Modern Hawaiian** as it is spoken in the Tepenian universe: a complete language that takes shape over the ~500 years between the Great War (2083) and the Falkland Treaty (2564), starting as a pidgin of English, Japanese and Tagalog on the islands of Hawaii, and becoming the international robot language and then the national language of the Tepenian Federation. It is synthesized as **its own complete language**, not studied or analyzed for slang. (Slang built on top of it is the job of the sibling repo, `slang-synthesis`; see `INTERFACES.md`.)

**What it is eventually for.** A series of eBooks: a **grammar reference**, a **full dictionary**, and **a couple of history books**. See `ebooks/`.

**Status:** starting structure only (created 2026-10-13). No language content exists yet. Nothing here is canon until it is recorded as accepted in `DECISIONS.md` and, where the Inner Tepenia GDD needs it, worked into the GDD by explicit decision.

## Read in this order

1. `CLAUDE.md` — standing rules for working in this repo.
2. `CANON.md` — what the developer has already established, with dates.
3. `ROADMAP.md` — the phases, and where the work stands.
4. `DECISIONS.md` and `OPEN_QUESTIONS.md` — what is settled, what is not.
5. `synthesis_method/` — how a language is derived here (read before writing any word or rule).

## Map

| Folder / file | What it holds |
|---|---|
| `CANON.md` | The established facts, each with a date and its origin. |
| `DECISIONS.md` | Numbered decision log (proposed, accepted, superseded). |
| `OPEN_QUESTIONS.md` | Questions awaiting the developer or research. |
| `INTERFACES.md` | How this repo connects to the GDD, `slang-synthesis`, and the eBooks. |
| `SOURCE_ACQUISITION_TODO.md` | Reference material still needed. |
| `ASSUMPTIONS.md` | Inputs chosen by the developer because the future cannot be derived (for example, Hawaii's demographics). |
| `public_domain_translations/` | Planned later: the developer's list of public-domain books to translate (`README.md`) and the plan for doing it (`PLAN.md`). |
| `RESEARCH_QUEUE.md` | Topics to research one at a time, with where to look and where each result goes. |
| `source_reference/` | Local, untracked library of grammars, dictionaries and studies. |
| `contributing_languages/` | One folder per source language: what it brings to Modern Hawaiian and at which level. |
| `real_world_analogs/` | Real pidgins, creoles and contact languages used as models (Hawaiʻi Creole English first). |
| `synthesis_method/` | The derivation pipeline, the layering table, and provenance rules. |
| `history/` | The language's own history, stage by stage, anchored to GDD dates. |
| `language/` | The language itself: phonology, orthography, morphology, syntax, lexicon, semantics, registers, dialects, sound change. |
| `ebooks/` | The planned books and how they compile from `language/` and `history/`. |
| `methodology-observations/` | A running record of what the method itself teaches us. |

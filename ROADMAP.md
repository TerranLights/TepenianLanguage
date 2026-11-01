# Roadmap

**Status legend:** `not started` · `in progress` · `complete`. Update when work actually begins or finishes.

## Phase 0 — Foundation *(in progress, 2026-10-13)*
Repo structure, standing rules, canon record. **Done:** structure created. **Next:** developer review of this structure.

## Phase 1 — Source acquisition and triage *(not started)*
Gather reference material (`SOURCE_ACQUISITION_TODO.md`). Triage and extraction are done in `slang-synthesis`, not here (D-9 Extraction in slang-synthesis, absorption here); this phase records what exists, what is missing, and what is extracted. Existing English, Japanese, Korean, Spanish and other material already sits in `slang-synthesis/source_reference/languages/`, with extractions in its `datasets/`; reference it by path, do not duplicate.

## Phase 2 — Contributing-language analysis *(not started; as of 2026-10-30 the sibling repo has completed Phase 1 extraction for English, Japanese, Korean, Spanish and Tagalog; Ilocano and Cantonese are triaged only; real Hawaiian has no sources yet; this phase absorbs the extractions)*
For each language in `contributing_languages/`: phonology, morphology, syntax, lexicon strata, what contact would keep and what it would drop. Order (D-19 Build order: English and Japanese first): **step 1,** how English and Japanese, the two primary sources, interact with each other; **step 2,** the layers of Tagalog, Ilocano, Spanish (Mexican) and Korean on top of that (order among them not yet decided). Output per language into its own folder.

## Phase 3 — Contact-language modeling *(not started)*
Study real pidgins and creoles (`real_world_analogs/`): how pidgins form, stabilize and nativize; typical outcomes for grammar, sound system and lexicon. Hawaiʻi Creole English first.

## Phase 4 — Layering table *(not started)*
Decide, with the developer, which source language governs which levels and domains (`synthesis_method/02_Layering_Table.md`) and which language supplies the grammatical frame.

## Phase 5 — Stage-by-stage derivation *(not started)*
Derive the language through its stages: contact pidgin, stabilized pidgin, creole, regularized standard (Falkland era, Hawaiian), then the Second Interwar's widening into Tepenian and Classical Tepenian (2812), the main primary target (D-21 Targets), then Federation-era usage. Record sound changes and grammaticalization in `language/` and the story of each stage in `history/`.

## Phase 6 — Core language build *(not started)*
Phonology, orthography, morphology, syntax, core lexicon, registers, dialects, pragmatics. Every item provenance-tagged.

## Phase 7 — Lexicon expansion and the Dome Fuji name *(not started)*
Grow the dictionary; derive the vocabulary the GDD needs (starting with the proper name of Dome Fuji, "The Temple").

## Phase 8 — History books *(not started)*
Write the language's history (and the history of Hawaii as it bears on it) from `history/`.

## Phase 9 — eBook assembly *(not started)*
Compile the grammar reference, dictionary and history books (`ebooks/`).

## Phase 10 — Handoff to slang-synthesis *(not started)*
Modern Hawaiian becomes an input language for in-universe slang work.

## Phase 11 — Public-domain translations *(not started; only after the language is functional)*
Translate public-domain books into the language (`public_domain_translations/`: the developer's book list in `README.md`, the plan in `PLAN.md`). Doubles as a stress test: every gap found goes in a gap log and is filled only by a recorded derivation. Begins once the core language build (Phase 6) is done. Target: the Falkland-era standard (D-17 Translation method and target); first book: Aesop's *Fables*.

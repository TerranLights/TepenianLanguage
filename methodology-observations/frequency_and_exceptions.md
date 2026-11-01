# Frequency vocabulary sets and motivated exceptions

**Status: `proposed` method, from the developer's statements of 2026-10-31 (decisions D-22 Frequency dictionaries seed the core vocabulary and D-23 Exceptions must have reasons).** The developer's words are marked as theirs; everything else is a proposal or an open point.

## 1. Frequency dictionaries seed the core vocabulary (D-22)
**Developer's plan.** Collect frequency dictionaries across as many languages as possible (the developer already has a fair number). They will help establish the **core-level vocabulary of Hawaiian**, which in turn establishes the core-level vocabulary of Classical Tepenian (C-13 Language timeline: Hawaiian to Tepenian). Once the words most commonly used across all languages are identified, it is much easier to decide which words to synthesize first.

**What this connects to.**
- The working assumption of a small real Hawaiian core of about 100 to 450 words (`ASSUMPTIONS.md`, "Real Hawaiian's share"), and the source weights.
- The selection factors (`selection_factors.md`) and the layering table (C-7 Layering by register and domain).
- The extraction spec's frequency column (`slang-synthesis/datasets/00_Reference_Extraction_Spec.md`), which records a "Weight/Frequency" value where a source gives one.
- One frequency dictionary is already known: a Japanese frequency dictionary in `language-stash/Japanese/` (`SOURCE_ACQUISITION_TODO.md`, 2026-10-18 survey).

**Points to settle (open, proposed for the research queue as RQ-B9).**
1. What "most commonly used across all languages" means in practice: the same concept's rank in each list, or presence in every list's top N. Lists differ in corpus (spoken or written), in what counts as a word (form or lemma), and in size, so ranks are not directly comparable.
2. Whether the languages are weighted by the source weights, by demographic share, or equally, and how this interacts with the stage the word belongs to (the Hawaiian stage versus the later stage, Q-16).
3. Whether a frequency dictionary exists for real Hawaiian; none is known here, and I will not assume one.
4. Where the dictionaries are stored. Books stay on the external drive and are referenced by path, with citations in `SOURCE_ACQUISITION_TODO.md`.

## 2. Exceptions with reasons (D-23)
**Developer's statements.** The language must look, operate and feel like a real language, so it needs **exceptions**. It cannot be like Esperanto, where there are none, because human (and robot) language is messy. But the exceptions **cannot be random**: each must have a reason it exists. For this the developer wants an extensive study of the kinds of exceptions found in real, currently existing languages; it will take months.

**Proposed shape of the study (RQ-B10).**
- Catalog the kinds of exception in the languages already extracted (the English, Japanese, Tagalog, Ilocano, Korean, Spanish and real Hawaiian extractions record irregular forms in their grammar notes) and in the general linguistics references now being collected.
- For each kind, record why it exists, with a source, not from memory (rule 4).
- Candidate reasons, **unverified leads only:** old forms surviving in very common words; vocabulary from different source layers following different patterns (the English `'s` and `of` split is the developer's example, D-18 Source layers as ways of thinking); sound changes that leave alternations behind. Whether frequency explains which words keep exceptions is a question to test, linked to D-22.
- Proposed rule for the language itself: every exception carries a **reason** field next to its provenance, so an exception without a recorded cause is not allowed in `language/` (rule 1 in practice). This is a proposal for the developer to accept or change.

## Revision history
- 2026-10-31: created from the developer's statements.

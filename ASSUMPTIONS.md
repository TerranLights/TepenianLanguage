# Assumptions

The future cannot be predicted in enough detail to derive a language from it, so some inputs have to be chosen, not derived. This file is the register of those inputs. Everything the repo derives later must say which assumptions it rests on, so that changing an assumption shows what it affects.

**Rules.** An assumption is chosen by the developer; it is not a research finding and is never presented as one. Each records what it assumes, why one is needed, how it will be informed by research, and what depends on it. All are `proposed` until the developer accepts them and the acceptance is logged in `DECISIONS.md`. Revise by adding a dated line to the assumption's history, never by overwriting.

| Name | Assumption | Status |
|---|---|---|
| Real Hawaiian's share | Real-world Hawaiian ends up a very small part of Middle Hawaiian: a core of roughly 100 to 450 actual Hawaiian words at the foundation level, with the rest of the language built on top of it. | proposed |
| Source-language weights | Rough shares of influence among the sources, as approximations only: English 30%, Japanese 30%, Tagalog 15%, Ilocano 15%, Korean 4.5%, Mexican Spanish 4.5%, other 1%; separately, a foundational core of 100 to 450 real Hawaiian words. Not laws to be obeyed. | proposed |
| Long-term divergence | Over the roughly thousand years after the Falkland-era standard, the language probably diverges into multiple accents and dialects, and possibly several languages, as Latin diverged into Spanish, French, Italian, Portuguese and Romanian; the Mars era, and perhaps a Jupiter era, are part of that picture. | proposed |
| Demographics of Hawaii | The population mix of Hawaii (who speaks what, in what proportions) at the time the pidgin forms is assumed, since it cannot be known. | proposed, details not yet chosen |

## Real Hawaiian's share

- **Stated by:** the developer, 2026-10-18 ("maybe around 150 to around 450 actual Hawaiian words that are down at the core foundation level of Middle Hawaiian. Then on top of that, the rest of the language actually gets built").
- **Revision history:** 2026-10-18, roughly 150 to 450 words. 2026-10-21, roughly 100 to 450 words (developer, stated while giving the source-language weights below). 2026-10-30, scope clarified to vocabulary only (see "Scope clarified").
- **Scope clarified (developer, 2026-10-30):** only a very core vocabulary comes from real Hawaiian. The majority of the grammar is a mixture of English and Japanese (the two primary sources), with some from Korean, Tagalog, Ilocano and Spanish. Real Hawaiian is therefore not a source of grammar; its grammar (for example the *a*/*o* possessive classes) is background only.
- **Why needed:** the repo has asked whether real Hawaiian contributes anything (see Q-4 Real Hawaiian's contribution). This sets the scale of the answer: a small core, not a major source language.
- **Still to decide:** which words, and by what criteria; what "foundation level" means in terms of the layering table (see the open question at the end of this section); how the words change over the centuries before the Falkland-era standard.
- **Vantage point:** from the Falkland era and later, today's real Hawaiian is "Ancient Hawaiian" (Mars era) or "Old" or "Medieval" Hawaiian (Federation era); see C-8 Era names.
- **Affects:** `contributing_languages/README.md` (role of real Hawaiian), `synthesis_method/02_Layering_Table.md` (place names, flora and fauna; religion and temple vocabulary, including Dome Fuji's name), the lexicon.
- **Open question for the developer:** does "foundation level" mean (a) the everyday common core of the vocabulary, as German is the common core of English, or (b) a deep underlying layer (a substrate) that other layers sit on, or (c) something else, such as names and nature words? The answer decides which row of the layering table these words go in.

## Demographics of Hawaii

- **Stated by:** the developer, 2026-10-18, as one of the assumptions that will have to be made.
- **Why needed:** the weighting factor in `methodology-observations/selection_factors.md` needs population shares, and the community that forms the pidgin lives after the Great War (2083), not in 2026.
- **Starting point:** sourced 2026 figures for Hawaii by home language, kept as a baseline and labeled as 2026. Any change from that baseline is recorded here as its own assumption, with the reasoning.
- **Sourced 2026 baseline (a research finding, not an assumption).** Hawaii State Data Book 2024 (Hawaii State Department of Business, Economic Development & Tourism), based on the U.S. Census Bureau's 2019-2023 American Community Survey 5-year estimates. Persons 5 and over; language spoken at home. Local copies in `source_reference/Hawaii_Demographics/` (git-ignored; fetched 2026-10-20 from `files.hawaii.gov/dbedt/economic/databook/2024-individual/01/`: `014324.pdf` Table 1.43 and `014424.pdf` Table 1.44).
  - Table 1.43: 1,363,614 people; 1,021,218 speak only English at home (74.9%). Its language lines group Ilocano, Samoan, Hawaiian and other Austronesian languages together (122,558).
  - Table 1.44 (DBEDT estimates from the Census microdata sample; its non-English total, 350,862, differs slightly from Table 1.43's 342,396, so the two tables are not interchangeable). Speakers of each language other than English, with their share of all non-English home speakers: Tagalog/Filipino 59,395 (16.9%); Ilocano 58,297 (16.6%); Japanese 39,249 (11.2%); Chinese (Mandarin, Cantonese and others) 35,176 (10.0%); Hawaiian 27,611 (7.9%); Spanish 27,497 (7.8%); Korean 15,024 (4.3%); other English-based Creole languages, which per its footnote includes but is not limited to Hawaii Creole English, 12,374 (3.5%); Samoan 10,564 (3.0%); Vietnamese 10,021 (2.9%); Chuukese 9,005 (2.6%); Marshallese 6,417 (1.8%); Portuguese 1,712 (0.5%).
  - Caveats: home-language self-reports are not the same as ethnicity or ancestry, and survey samples carry sampling error. These are 2019-2023 figures, not a model of the community that forms the pidgin.
- **Not yet chosen:** the baseline year and source, how the mix changes between 2026 and the pidgin's formation, and what, if anything, the Great War does to it.
- **Affects:** every weighted choice about which source language supplies a feature.

## Source-language weights

- **Stated by:** the developer, 2026-10-21, as "strictly approximation-only; *NOT* 'laws' to be obeyed. Only rough estimates."
- **The figures:** English 30%; Japanese 30%; Tagalog 15%; Ilocano 15%; Korean 4.5%; (Mexican) Spanish 4.5%; other 1% (total 100%). Real Hawaiian is separate: a foundational core vocabulary of 100 to 450 words (see "Real Hawaiian's share" above), not part of the percentages.
- **Why needed:** the repo needs a rough guide to how much each source contributes when sources disagree, to be combined with the factors in `methodology-observations/selection_factors.md` (usability, demographic weight, cultural influence).
- **How to use it:** as a sanity check on the overall balance of the result, never as a rule that forces a word or rule to come from a given language. A derivation records its reasons; the weights only say whether the overall mix looks plausible.
- **Open points (to settle with the developer):**
  1. *What the percentage measures.* Overall influence, or vocabulary share, or grammar, or sound system? These can differ a lot (for example a language might supply many words and little grammar). Until settled, the weights mean "overall rough influence."
  2. *Departure from the sourced baseline.* Home-language shares among non-English speakers in 2019-2023 were Tagalog 16.9%, Ilocano 16.6%, Japanese 11.2%, Spanish 7.8%, Korean 4.3% (see the demographics baseline below), and 74.9% of residents speak only English at home. The weights give Japanese much more than its present share and English much less. The reason should be recorded (for example cultural influence, or the pidgin's formation after the Great War), since this is a deliberate departure from raw demographics.
  3. *What "other" means.* It cannot include Portuguese (D-10 Portuguese excluded as a source) or Chinese (D-11 Chinese excluded as a source). Candidates, if any, are still to be named (for example Okinawan, Samoan, Chuukese, Marshallese).
  4. *Role labels.* The roster's role words (core, supplementary) have not been reassigned to match these weights. Ilocano is marked core in the roster as of 2026-10-21 pending confirmation.
- **Affects:** `contributing_languages/README.md` (roles), the layering table, and every weighted choice in the lexicon and grammar.

## Long-term divergence

- **Stated by:** the developer, 2026-10-26, while answering questions about the public-domain translations. Framing: the Falkland-era standard (about 2564) is a base from which later forms are extrapolated; after about a thousand more years the language "will probably diverge into multiple accents and dialects and possibly even multiple languages, the way that Latin diverged into Spanish, French, Italian, Portuguese, and Romanian."
- **Why needed:** it sets how far this repo's modeling reaches (see Q-10 Mars-era scope) and what "Modern Hawaiian" and "Middle Hawaiian" refer to in the later eras.
- **Not canon:** the repo's canon covers the Federation era and the Mars era (C-8 Era names). A Jupiter era does not appear in the canon. The Inner Tepenia GDD holds the world's timeline; nothing flows back to it without an explicit decision.
- **Open points for the developer:**
  1. *Era naming if there is a Jupiter era.* The canon's naming rule is by vantage point (Modern, Middle, Ancient). Does it need extending, and if so how?
  2. *Does a daughter language count?* If a later form is a separate language, does this repo give it its own name, or call every stage a form of Modern Hawaiian from its own vantage?
  3. *Scope.* How much of the later divergence does this repo model, versus only the Falkland-era standard and the Federation era?
  4. *Starting point (added 2026-10-31).* With Tepenian and Classical Tepenian now canon (C-13, C-14), is the base for the later divergence Classical Tepenian (2812) and not the Falkland-era standard?
- **Research lead (unverified):** historical accounts of how Latin diverged into the Romance languages, as an analog for long-term divergence; to be checked against real sources and recorded under `real_world_analogs/` if used.
- **Affects:** `synthesis_method/01_Pipeline.md` (stages 6 to 8), the dialects folder, and the long-term reach of `history/`.

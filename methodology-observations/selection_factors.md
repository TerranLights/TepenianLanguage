# What decides which source language wins a feature

**Status: proposed.** Stated by the developer on 2026-10-18; not yet logged as a decision in `DECISIONS.md`.

## The principle

When the contributing languages disagree about a sound, word or rule, "which one is most common among them" is not enough. At least three other factors decide what a mixed community settles on.

1. **Usability (a workable middle ground).** Speakers with different native systems need something all of them can use. Where the sources handle a feature differently, the result may be a middle form that matches none of them exactly. Example from the developer: the sources treat articles (the, a) very differently, so the language would find some intermediate arrangement. Icelandic, which is not a source, is only an illustration of what such an arrangement can look like, not a derivation.
2. **Demographic weight.** A language's share of the population affects how much it contributes. Developer's example: Spanish speakers are about 10% of Hawaii. That figure is the developer's estimate and still needs a source.
3. **Cultural influence.** A group that is technically a minority can still shape the language when the majority finds its forms useful and takes them into their own habits. Numbers alone do not predict this.

## What each factor needs as evidence

- Usability: a recorded comparison of how each source language handles the feature, then a stated reason the middle form is easier for the mixed community. Record the reasoning, not just the result.
- Weight: a sourced population breakdown, with the date it describes. The pidgin forms after the Great War (2083), so 2026 figures are a starting proxy, not the weights of the community that actually speaks it. Open question for the developer: which date's population should the weights model?
- Cultural influence: a stated reason the majority would adopt the form (a function it fills, a gap it covers), ideally with a real-world parallel recorded in `real_world_analogs/`.

## Auxiliary reinforcement (Chinese), added 2026-10-21

Per D-13 Chinese as an auxiliary reinforcement mechanism: for any feature under question for the language, check how Cantonese and Mandarin handle it. If they operate similarly, the feature's strength (its likelihood of being in the language) goes up; if they operate in conflict, it goes down. Chinese never supplies a form of its own and is not counted in the source-language weights. It only adjusts candidates that come from the real sources (English, Japanese, Tagalog, Ilocano, Korean, Spanish, and the Hawaiian core).

This follows what real contact showed: Siegel (2000) argues that the Cantonese substrate in Hawaii Creole English reinforced and expanded patterns already present in the pidgins, and did not introduce them on its own.

**Rules settled 2026-10-21 (D-14 Rules for Chinese reinforcement):**
1. *Size of the effect.* It depends on how fundamental the feature is to the language. The more fundamental the functionality, the more a reinforcement or a conflict counts.
2. *When Cantonese and Mandarin disagree with each other.* The result is only a partial increase, not a full one. (Reading to confirm: one of them operates similarly and the other does not; if both are in conflict, the strength goes down as in the basic rule.)
3. *What counts as "operating similarly."* All three: the same surface form, the same function, and the same mechanism. More fundamentally, the same sort of function and/or mechanism; a matching surface form alone counts for less than a matching function or mechanism.
4. *Other reinforcers.* None. This applies to Chinese only.

**Still open:**
- How to judge "how fundamental" a feature is (for example whether core grammar such as word order and tense/aspect counts as most fundamental and peripheral vocabulary as least) and how the judgment is recorded, so two derivations treat the same kind of feature the same way.
- How to record the result (a note on each derivation giving the strength change and the reason). No numeric scale has been chosen, and none should be invented.

## Draft ranking: how fundamental a feature is (proposal, 2026-10-21)

**Status: accepted as a working draft (D-15 Fundamentality bands as a working draft, 2026-10-21); adjust wherever the need arises.** Written by Claude to answer the first open point above; the developer corrects it. It is a design judgment, not a research finding, and is not yet checked against the literature (see RQ-B7). Under D-14, the more fundamental the feature, the larger the reinforcement or conflict effect from Chinese. No numbers are attached; only the order and the bands.

| Band | Feature types | Examples from this repo's candidates |
|---|---|---|
| **1. Foundation (largest effect)** | Basic word order and clause structure; how predicates are built (copula or none, adjectives as verbs, how existence, possession and location are expressed); the strategy for tense, aspect and mood; negation; how questions are formed. | Siegel's patterns: one word for "have" and "there is"; a separate word for location; no copula; adjectives behaving like verbs; weak tense and aspect marking. |
| **2. Structural categories (large)** | The sound system and syllable shapes; number marking; articles and specificity; classifiers and counting; pronouns; prepositions or particles that mark roles. | The ideas file's "no singular/plural", "definite article but no indefinite", "genderless nouns". Siegel's *one* and *the* for specificity. |
| **3. Word-building (moderate)** | Affixes, reduplication, compounding; derivation. | The person-from-a-place suffix; honorific suffixes. |
| **4. Function words and discourse particles (smaller)** | Small grammatical words, conjunctions, fillers and discourse markers. | No candidates yet; examples would be filler words and sentence-final particles. |
| **5. Vocabulary (smallest)** | Basic everyday words first, then common words, then specialized and cultural words (names, foods). | The real Hawaiian core words; food and place words. |
| **6. Pragmatics and idiom (smallest)** | Politeness conventions, address terms, idioms. | San/Sama and Kun/Chan address terms. |

**Notes on the draft.**
- Sounds could arguably go in band 1, since the sound system limits what every word can be. Placed in band 2 for now.
- Address terms (San, Sama, Kun, Chan) are partly grammar (a closed set of forms) and partly pragmatics; placed in band 6 provisionally.
- Features can sit between bands; the rule is that two derivations treat the same kind of feature in the same band.

## Research leads (unverified; to check against real sources, not to cite from memory)

Contact-linguistics literature on accommodation and leveling between speakers of different languages, on how the proportions of speakers affect a mixed language, and on covert prestige and borrowing from low-status or minority groups. Candidate sources are the pidgin and creole genesis works still listed as not acquired in `SOURCE_ACQUISITION_TODO.md`.

## How this fits the pipeline

It informs the contact pidgin and stabilization stages in `synthesis_method/01_Pipeline.md` (which words and structures "win"). The pipeline's nativization stage currently lists plural marking among the grammar that expands; the developer's idea of a language with no singular/plural distinction (`to-be-integrated/ideas_for_further_investigation.md`) would need that line revisited. The pipeline is still a draft.

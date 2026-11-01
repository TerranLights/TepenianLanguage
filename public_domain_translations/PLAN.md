# Public-domain translations: plan

The developer's own book list is `README.md` in this folder. This file holds the plan around it: why, when, how, what is settled and what is still open. Written by Claude on 2026-10-26 from the developer's note and answers; rebuilt on 2026-10-26 after a README edit overwrote the first version. Anything marked PROPOSED is for the developer to decide.

## Purpose and timing
Once the Tepenian language is formulated, structured and functional as a learnable language, public-domain books will be translated into it (D-16 Public-domain translations planned). This comes **after** the core language build (Phase 6 in `ROADMAP.md`, where it is Phase 11). Nothing is translated yet, and nothing should be started before the core language exists.

**Vantage point.** The same language is "Modern Hawaiian" from the Federation era and "Middle Hawaiian" from the Mars era (canon item C-8 Era names). Every translation says which stage of the language it targets. The target is the Falkland-era standard, about 2564 (D-17 Translation method and target).

## Why this is more than a hobby project
1. **It is a stress test.** Every passage a translator cannot render exposes a gap in the lexicon or grammar. Nothing may be invented to fill it (rule 1, derive, do not invent): each gap goes in a gap log, and each new word needs a recorded derivation before it enters `language/`.
2. **It checks coverage.** Different books exercise different registers and domains, which maps onto the layering table (`synthesis_method/02_Layering_Table.md`).
3. **It proves learnability.** Many books at many levels give a real learner a reading path at any skill level.
4. **It fits the setting.** The canon says the International Archive, a vast library of human information, is a major data source for the robots (C-1 Hawaii's importance to the robots). Robots translating human works into their own language is plausible in-universe (a suggestion, not canon).

## Settled (developer, 2026-10-26; D-17 Translation method and target)
1. **Source text:** translate each book from its own original language, because that is how real-world book translations are usually done.
2. **Target stage (revised 2026-10-31 by D-21 Targets: the main target is now Classical Tepenian at 2812; translating into Hawaiian, the Falkland-era standard, remains possible; the original answer follows):** the Falkland-era standard (about 2564), as a base for later extrapolation into the Modern Hawaiian of the Mars era, and perhaps the Jupiter era (see "Long-term divergence" in `ASSUMPTIONS.md`).
3. **Reader:** an in-universe reader, with many books at many registers and levels of complexity so a real learner of any skill level has something at the right level to practice reading comprehension.
4. **Output form:** a combination of stand-alone books and parallel text, with stand-alone books predominant.
5. **First book:** Aesop's *Fables*, because the language is very simple and accessible and the collection is large.

## What the developer's list needs, given original-language translation
Original languages as I understand them (to be confirmed per book against a catalog):

| Original language | Books on the developer's list |
|---|---|
| Ancient Greek | *Meditations* (Marcus Aurelius); *The Republic* (Plato) |
| Russian | the Dostoevsky books |
| Classical Chinese | *The Art of War* (Sun Tzu); translating it does not conflict with D-11 Chinese excluded as a source |
| Italian | *The Divine Comedy* (Dante) |
| English | *Heart of Darkness*, *Dracula*, *Frankenstein*, Douglass's *Narrative*, the Wells books, the Poe books, *Paradise Lost*, *The Wealth of Nations*, *Flatland*, the Hemingway books |
| Greek and Latin (several collections) | Aesop's *Fables* (not on the list as written; see "Still open") |

**Public-domain caveats (verify per book and per country; RQ-C6).**
- Most of Hemingway's work is later than 1930 and may not be in the public domain yet, so "all available books" may be only his early works.
- For books translated from another language, the original may be free while a given English edition is not. Because the plan is to translate from the original, the edition of the original matters; its editor's apparatus may be protected even if the text is not.
- The poems (*Paradise Lost*, *The Divine Comedy*) are long and hard tests of verse, likely late projects.

## Reference translations (check readings), added 2026-10-26
Because each book is translated from its original language (D-17), a published translation can serve as a **reference for checking understanding of the original**, not as the base text.
- ***The Art of War*:** the developer suggests Thomas Cleary's English translation as a basis of reference. Library and retailer listings show several editions (a 1983 hardcover listed under another publisher, and Shambhala editions listed under 1998, 2003, 2005 and 2019); **the developer owns a copy published in 1991** (2026-10-26), an edition my search did not list, so its publisher, title page and any commentary are still to be recorded from the book itself. It is a physically small pocket edition; whether it carries the complete translation, or any commentary, is to be checked against a fuller edition. That owned copy is the edition to use.
- **Copyright caution (to verify):** a modern translation is the translator's own protected work, so it is almost certainly not in the public domain. It may be read and used privately to check a reading. The Tepenian-language text must come from the Chinese original, not from Cleary's English wording, and none of Cleary's text is copied into this repo beyond short quotation with citation (repo rule 2).
- **Where it fits:** this is one answer to open point 2 below (how to check readings of original-language texts). Other books will need their own reference translations, chosen per book.

## Selection criteria (PROPOSED)
- The specific edition of the source text must be verifiably in the public domain.
- A spread of registers and domains: reflection, narrative, formal and legal prose, technical and logical exposition, poetry.
- A graded range of length and difficulty, starting with the simplest.
- Preference for texts the developer cares about, since this is a long project.

## Candidates added by Claude, not on the developer's list (PROPOSED; all unverified)
| Title | Why it might suit | Register tested |
|---|---|---|
| Aesop, *Fables* | **First book (developer's choice).** Very short self-contained stories; simple language; a large collection | simple narrative, moral |
| Epictetus, *Enchiridion* | Short numbered sayings; pairs with *Meditations* | aphorism, reflection |
| Euclid, *Elements* (an opening book) | Definitions and proofs; a strong test of logical and technical vocabulary | technical, mathematical |
| Machiavelli, *The Prince* | Argument and strategy in prose | political, argumentative |
| Čapek, *R.U.R.* | The play that gave the world the word "robot"; original is Czech; check which translation, if any, is free | drama, dialogue |
| A short formal founding document | A compact test of legal and formal register | formal, legal |
| A small selection of Shakespeare's sonnets | A hard test of poetry and compression; likely a late project | poetry |
| Carroll, *Alice's Adventures in Wonderland* | Wordplay is a severe stress test; likely a late project | wordplay, dialogue |

## Per-book record (PROPOSED template)
Title; author; original language; the edition of the original that will be used and its editor; year; why it is in the public domain (which country's law, and how this was verified); where the source text was obtained; length; registers and domains it covers; target stage of the language; translation file path; link to the gap log; status.

## Still open (also in `OPEN_QUESTIONS.md` as Q-12 Translation method and target)
1. **Aesop's original.** The fables survive in many ancient collections in Greek and Latin and there may be no single original text. Which collection or collections count as "the original" has to be chosen and verified against a scholarly source, not from memory.
2. **Working from original languages.** Translating from Greek, Latin, Russian, Italian, Classical Chinese and so on needs a reliable public-domain edition of each, reference dictionaries, and a way to check the reading, such as comparing a public-domain English edition. Tools and checks are to be decided with the developer.
3. **Making an in-universe book usable for real learners.** Are the graded levels shown in-universe (for example as in-world reader levels)? Do the books carry glosses or notes, or do learners rely on the grammar reference and dictionary in `ebooks/`?
4. **Which books are parallel text.** The default is stand-alone.
5. **The next books after Aesop.**
6. **README housekeeping (developer's file):** Aesop is not on the list; the Douglass title is missing its closing quotation mark; Poe's first name is usually spelled "Allan".

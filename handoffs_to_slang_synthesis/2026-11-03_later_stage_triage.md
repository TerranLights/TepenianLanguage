# Handoff to `slang-synthesis`: triage the later-stage languages

**Written 2026-11-03 by the Tepenian Language session, for the `slang-synthesis` session.** The developer asked for this work to be done in `slang-synthesis`, not in `TepenianLanguage`. Nothing in this file has been done yet.

## The task

Do a **full triage, one language at a time**, for each language below. **Do not extract anything yet.** The data extraction waits until the developer says so. Triage only: inventory, text-layer check, identification, exclusions, duplicates, priority tiers, and a catalog.

Write each result in the usual place and format: `datasets/<Language>/00_Book_Triage_Catalog.md`, plus `.triage_raw.tsv` where that is your habit. Follow the structure of the most recent catalogs, `datasets/German/00_Book_Triage_Catalog.md` (2026-11-01) and `datasets/Cantonese/00_Book_Triage_Catalog.md` (2026-10-26): headline numbers, exclusions (wrong metalanguage or audience), non-content assets, packed archives, bulk usage-corpus material, a category overview, and priority tiers. Identify each book from its title page or metadata; do not guess titles from filenames alone.

## Why these languages (context, not instructions)

These are the "later-stage" languages of the Tepenian language project: the ones that influence the base language (Hawaiian) as it becomes Tepenian over the Second Interwar Period (2564 to 2812). The developer's ideas for what each might bring are `proposed`, not decided, and they are only context for you:

| Language | Domain the developer associates with it | Presence in the Federation (from the GDD) |
|---|---|---|
| Scandinavian languages (Swedish, Norwegian, Danish) | technical studies | Troll (Norway); Utstein |
| Indonesian (with Malay) | agriculture | Relung Panen |
| Portuguese | none yet | Brazil's presence in Tepenia along and around the Palmer Peninsula (developer, 2026-11-03; D-10) |
| Mongolian | none yet | Ariun Nuur |
| Kazakh | none yet | Mawson, Temirötkel |
| West Slavic (mainly Polish) | none yet | the Intermarium bloc, centered on Poland |

So the useful finds, beyond grammars, are: general and technical vocabulary, colloquial and slang material, anything in the domains above, and word lists or frequency lists. Flag any frequency list or frequency dictionary you meet in a stash. The developer is collecting those in a separate folder (`/home/kuroskalacs/Documents/Doll-Fi/media/y-files/frequency_dictionaries/`), and a list found inside a stash belongs there, so report it and do not move it.

## Scope

**In scope (file counts as measured on 2026-11-03; none triaged yet):**

| Language | Where the books are | Files (measured) |
|---|---|---|
| Swedish | External drive `/media/kuroskalacs/Home-Theater/w-lang/Swedish/` (3.1 GB): 126 files (72 PDF, 23 DJVU, 29 audio or video). Also `source_reference/languages/Swedish/` (620 MB): 20 files (16 PDF) | 146 |
| Norwegian | External drive `w-lang/Norwegian/` (3.0 GB): 109 files (92 PDF, 9 DJVU, 1 audio or video) | 109 |
| Danish | External drive `w-lang/Danish/` (855 MB): 39 files (30 PDF, 7 DJVU, 1 audio or video). Also `source_reference/languages/Danish/` (151 MB): 14 PDFs | 53 |
| Malay-Indonesian | External drive `w-lang/Malay-Indonesian/` (1.8 GB): 60 files (53 PDF, 4 DJVU). Covers Malay as well as Indonesian | 60 |
| Mongolian | External drive `w-lang/Mongolian/` (1.2 GB): 44 files (41 PDF, 2 DJVU). Also `source_reference/languages/Mongolian/` (4.5 GB): 203 files (193 PDF). Also three loose files in `source_reference/languages/`: *An Elementary Mongolian Grammar* (Daniel Elliott), *The Secret History of the Mongols*, and *Ocean of Milk, Ocean of Blood* (Matthew King) | about 250 |
| Kazakh | External drive `w-lang/Kazakh/` (454 MB): 40 files (23 PDF, 16 DJVU). Also `source_reference/languages/Kazakh Language Learning Pack/` (541 MB): 33 files, and `source_reference/languages/Colloquial Kazakh/` (186 MB): 3 files | 76 |
| Portuguese | External drive `/media/kuroskalacs/Home-Theater/w-lang/Portuguese/` (3.6 GB): 167 files (123 PDF, 28 DJVU, no audio or archives), in two subfolders, `Brazilian Portuguese/` and `European Portuguese/`. Nothing in `source_reference/languages/`. Keep the Brazilian and European material distinct in the catalog: Brazil is the reason Portuguese is on the list | 167 |
| Polish (West Slavic) | External drive `w-lang/Polish and Ukrainian/` (12 GB): 1,015 files (234 PDF, 246 DJVU, 238 audio or video). Also `/home/kuroskalacs/Documents/Doll-Fi/media/y-files/language-stash/Polish/` (16 MB): *Colloquial Polish* (Mazur) and *Polish: A Comprehensive Grammar* (Sadowska) | 1,017 |

**Out of scope for this pass:**
- **Italian and Australian slang.** The developer will find additional resources for them later.
- **Russian and German.** Both are already triaged (Russian 2026-09-12 and extracted; German 2026-11-01). Do not redo them. Russian and German extraction decisions are separate.
- **Czech.** There is no Czech book stash, only a frequency dictionary that is already in the frequency folder.
- **Ukrainian.** The Polish folder is shared with Ukrainian and Ukrainian is not on the list. Triage the Polish material, but list the Ukrainian files in one short table (counts and sizes) so the developer can decide later. Treat other Slavic material found in that folder the same way, and note whether a Czech or Slovak title turns up (West Slavic).

**Two things I did not check and you should:**
- `source_reference/languages/lang transfer bay/` (5.4 GB) and `source_reference/languages/xx--stash/` (1.4 GB) are unsorted. They may hold more books for the languages above. A filename and folder-name search is enough. List anything found, and fold it into the right catalog.
- The folder sizes above come from `du` in 1 MiB steps. The file counts come from `find`. Confirm both when you harvest.

## Conventions that apply

- **Source books stay where they are.** Do not copy, move or track PDFs, and do not write into the external drive or into the source folders. Work on renders and extracted text in a scratch location.
- **The external drive is mounted at `/media/kuroskalacs/Home-Theater/`.** Confirm that it is mounted before starting. The developer's home SSD is about 94% full, and so is the external drive, so keep scratch output small and delete it when you finish.
- **Identify before you rate.** For files with a text layer, read the first pages from the text layer. For image-only files, render the title or copyright page and read it. Say in the catalog how each title was confirmed, as the Cantonese catalog does.
- **Check duplicates** by full filename and by md5 (the same book appears in two formats or in two folders, as in the Cantonese and Korean catalogs).
- **Check the metalanguage.** This project's extraction is English-medium. Exclude Swedish-to-German, Norwegian-to-Russian and similar glossaries and courses, as the German catalog does, and check each file in a multi-glossary folder on its own. A Swedish-medium grammar of Swedish (as opposed to an English-medium one) needs an explicit decision. Do not silently drop or keep it. Put such books in their own section so the developer can rule.
- **Audio and video** are not extraction targets. Count them and list the companion relationship (audio that goes with a named course book), nothing more.
- **Flag the slang and colloquial titles** as the flagship category when they exist, because that is what this project most wants from a stash.
- **Do not state facts from memory about books or languages.** Everything in a catalog should come from the file in front of you.
- **Pacing.** The developer has asked for one language at a time. Finish and verify one catalog before starting the next. The developer has also raised token-burn concerns on large jobs, so keep rendering to what identification needs (title pages, not whole books). Polish is the large one: 1,015 files. Do it last, after Portuguese, and consider triaging it in batches by sub-folder, with a running count, so that an interruption leaves usable work.
- **Commit** only when the developer asks.

## When you finish

Tell the developer, per language: file counts, real candidates, text-layer versus vision-read counts, exclusions, flagship titles, and anything you want a ruling on. The `TepenianLanguage` session will then update its roster (`contributing_languages/README.md`), `SOURCE_ACQUISITION_TODO.md` and the disk-space figures from the catalogs.

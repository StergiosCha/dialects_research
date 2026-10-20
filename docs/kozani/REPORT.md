# Kozani inventory: session report

Date: 20 October 2026. Branch: claude/kozani-inventory-review-o5ks95. Files: docs/kozani/00-scope.md to 13-open-questions.md, one commit per file.

## What was done

All fourteen files exist: the scope (00), ten researched sections (01 to 10, 155 table rows in total, ten to seventeen rows each), three synthesis sections (11 disagreements, 12 top ten, 13 open questions) and this report. Sections 1 to 10 were researched by one agent each in parallel, sections 11 to 13 were written from the filled tables. Every file passed the style check: no em or en dashes, no semicolons, six columns in every table, one "Not found" line per researched section.

## The blocker: no page could be opened

The cloud environment's network policy denied outbound connections to every host except github.com, raw.githubusercontent.com and pypi.org (the proxy answered 403 on CONNECT, WebFetch got DNS failures). Web search worked, but its per-session budget of about 200 calls was shared by the ten agents and ran out part way through each section (between 6 and 48 searches per agent). The consequence:

- Every row that does not cite a GitHub repository rests on search-engine records and catalogue snippets, and is marked [unverified: page not opened]. The convention in HANDOVER.md ("a search snippet is not a source") is therefore not met for about 140 of the 155 rows. Nothing was invented, and each row still gives the URL the search returned so a follow-up can open it.
- Sections 6 (orthography) and 9 (tools) are the exception: their GitHub rows (the UD_Greek-Lesbian treebank, GRDD_plus, DI_detector, eellak, apertium-ell, IPA_Greek and others) were opened and counted, and are verified.
- Section 10 (people) is the weakest: a first pass produced only a checklist of leads. A second agent was launched to redo it from search records, and if it finishes its result replaces the file in a later commit. Treat the committed version as a list of who to contact, not as findings.

Remedy: in the environment settings (cloud environment menu in the session's title bar, then Edit, Network access) choose a broader access level or add the Greek institutional domains under Allowed domains (uowm.gr, academyofathens.gr, ekt.gr, upatras.gr, auth.gr, uoc.gr, kozlib.gr, greek-language.gr, mdpi.com, benjamins.com, archive.org, wikipedia.org, oeaw.ac.at, ertnews.gr, kozan.gr and the other local media). Then re-run the ten section briefs against the existing files with the instruction to open every cited URL and replace the [unverified] markers. Steps: https://code.claude.com/docs/en/cloud-environments#network-access.

## What was found

The Kozani literature is as thin as HANDOVER.md expected, but not empty.

- **Grammar (01).** One full grammar, Ντίνας 2005 (two print volumes, about 240 and 592 pages, copyrighted). Three acoustic papers on Kozani speakers give the quantitative vowel rules (Topintzi and Baltazani 2012, Lengeris, Kainada and Topintzi 2016, Lengeris et al. 2015). One open-access syntax paper from 2019 fieldwork in Kozani and Grevena states the accusative indirect object rule (Anagnostopoulou, Mertyris and Sevdali 2022). Sister-idiom grammars exist for Σιάτιστα (Τσοπανάκης 1953, Μαργαρίτη-Ρόγκα 1985), Βελβεντό (Μπουντώνας 1892, public domain) and Αιανή (Χριστοδούλου 2012).
- **Lexicon (02).** Κοζανιτολόγιο (Χριστοδούλου 2017, about 6,600 lemmas, volumes 2 and 3 announced as free files) and the Ντίνας glossary. No open machine-readable Kozani lexicon. The ΚΕΝΔΙ-ΙΛΝΕ archive holds manuscript glossaries for Kozani (1959), Σιάτιστα, Βόιο, Βελβεντό and Ερατύρα.
- **Texts (03).** The carnival (φανοί) songs are the only sizeable corpus: a web list (kozanitikiapokria.gr), a 2010 compiled volume (Λάκκας), a reported 180-song collection (Φτάκα-Τσικριτζή). Dialect prose from 1964 to 2022 is all in copyright (Παπασιώπης, Κουζιάκη Παπαγγέλη 2008, Πιτένης 2022). ΙΛΝΕ manuscripts from 1892 and 1933. GRDD's Northern portion is reported (unverified) to come from Kozani and Grevena.
- **Audio (04).** Nothing openly licensed. ΕΡΤ archive documentaries, ΕΡΤ Κοζάνης carnival reports, local TV, YouTube uploads, two CDs (one municipal and non-commercial). Institutional sound archives (ΚΕΝΔΙ, Λαογραφία, Μερλιέ) hold no confirmed Kozani item. No Northern Greek ASR or TTS.
- **Teaching (05).** Nothing teaches Kozanitika: one 2018 school newspaper feature, a 2024 ημερίδα with a 2025 proceedings volume, Ντίνας's teacher-education course on γλωσσική ποικιλία, national curriculum units on varieties in general.
- **Orthography (06).** No explicit convention. The UD_Greek-Lesbian treebank (CC BY-SA 4.0, opened and counted) gives the de facto Northern practice: apostrophe for deleted /i/ and /u/, phonetic ι and ου for raised vowels, plain τσ and τζ, SMG lemma underneath, 3sg mediopassive written -ιτι not -ιτ'.
- **Variation (07).** Θαβώρης 1994 (the Μακεδονικά article HANDOVER.md attributed to Ντίνας) classes the nomos as Northern. Kozani is full Northern, Καστοριά semi-Northern. Pappas 2017 is the one sociolinguistic study of the vowel rules as variables, locality unknown. Σέρβια, Βόιο and Εορδαία are undocumented.
- **Pedagogy (08).** Concentrated in the Πανεπιστήμιο Δυτικής Μακεδονίας circle: Ντίνας and Ζαρκογιάννη 2009, the Μαρωνίτη, Στάμου, Γρίβα and Ντίνας 2016 intervention, a ΠΔΜ thesis designing Gymnasium exercises on Kozani forms. No Northern spelling-error or acquisition study.
- **Tools (09).** Kozani is not a class anywhere. No SMG to Northern converter exists. The open SMG stack (eellak morphological dictionary CC BY-SA 3.0, modern-greek-inflexion MIT, apertium-ell GPL-3.0, IPA_Greek MIT) is the base to build on. The ILSP greek-dialects-asr recipe is rerunnable on Kozani recordings.
- **People (10).** First contacts in order: Κ. Ντίνας, the rights holder of the Ινστιτούτο Βιβλίου και Ανάγνωσης Κοζάνης, the Κοβεντάρειος library, then the Σύνδεσμος Γραμμάτων και Τεχνών (Λαογραφικό Μουσείο, Κοζανιτολόγιο), ΟΑΠΝ Δήμου Κοζάνης (carnival), ΚΕΝΔΙ.

## Implementable items

Flagged **Implementable** in the tables (rules codable from facts, or data loadable under licence):

- Ντίνας 2005 (grammar and glossary, rules codable, data needs permission).
- Lengeris, Kainada and Topintzi 2016 and Topintzi and Baltazani 2012 (vowel rule conditioning and rates).
- Anagnostopoulou, Mertyris and Sevdali 2022 (accusative indirect object, clitic doubling).
- Θαβώρης 1994 (nomos-wide rule statement).
- Μαργαρίτη-Ρόγκα 1985 (rule-based phonology of Σιάτιστα as a model).
- Μπουντώνας 1892 (public-domain paradigms, Βελβεντό).
- UD_Greek-Lesbian treebank and README (display convention, two-layer data model, CC BY-SA 4.0).
- ΚΕΝΔΙ IPA page and ΙΛΝΕ transcription system (pronunciation layer, pending symbol tables).
- eellak morphological dictionary, modern-greek-inflexion, apertium-ell, IPA_Greek (open SMG base for generating Kozani forms).
- GRDD+ fine-tuning scripts (CC BY-NC-SA 4.0, non-commercial).
- Κοζανιτολόγιο and the Ντίνας glossary (with permission), the ΙΛΝΕ TEI entries (licence to confirm), Wiktionary pipeline (CC BY-SA, near-zero Kozani content).
- The ΠΔΜ thesis on teaching the Kozani idiom and the 2016 intervention (exercise types and evaluation items, with permission), the 20-word comprehension test (town to confirm).
- Common Voice Greek (CC0, SMG baseline only).

## Open or public-domain items

- Public domain: Μπουντώνας 1892 (Ανέμη scan, death year 1941 to confirm). Possibly the 1892 ΙΛΝΕ Kozani collection, collector's death year unknown.
- Open licence: UD_Greek-Lesbian (CC BY-SA 4.0), eellak morphological dictionary (CC BY-SA 3.0), modern-greek-inflexion (MIT), apertium-ell (GPL-3.0), IPA_Greek (MIT), kypriaka skill (MIT), greek-dialect-classifier (MIT), UniMorph ell (CC BY-SA 3.0), spaCy el and UD GDT (CC BY-NC-SA 3.0), Stanza (Apache 2.0), Greek BERT (MIT), Piper and espeak-ng (MIT, GPL-3.0), Common Voice Greek (CC0), Wiktionary (CC BY-SA), UD_Greek-Cypriot (CC BY-SA 4.0), Anagnostopoulou et al. 2022 and Condoravdi and Kiparsky 2026 (MDPI Languages, CC BY expected, unconfirmed), ΙΕΠ curriculum text (state regulatory text).
- Open PDF but copyrighted (facts usable, text not): Θαβώρης 1994 and 1998, Τσοπανάκης 1953, Ανδριώτης 1933, Κατσάνης 1985, Lengeris et al. 2016, Topintzi and Baltazani 2012 (course copy), Trudgill 2003 (university copy), Χριστοδούλου 2012, Ντάγκας 2012, Μπατζιακοπούλου 2015, Κυρανούδης thesis, the ΠΔΜ theses, the 2018 school feature.

## Top ten (section 12, in rank order)

1. Ντίνας 2005 (Ask).
2. Lengeris, Kainada and Topintzi 2016 with Topintzi and Baltazani 2012 (facts free).
3. Anagnostopoulou, Mertyris and Sevdali 2022 (Open, CC BY expected).
4. Κοζανιτολόγιο 2017 (Ask, free electronic volumes announced).
5. The carnival song corpus via ΟΑΠΝ Δήμου Κοζάνης (Ask).
6. The open SMG stack: eellak, modern-greek-inflexion, apertium-ell (Open, usable today).
7. UD_Greek-Lesbian treebank (Open, usable today).
8. Μπουντώνας 1892 (PD).
9. ΚΕΝΔΙ-ΙΛΝΕ archive (Ask, archive visit).
10. The ΠΔΜ teaching thesis and the 2016 intervention (Ask).

## Corrections to HANDOVER.md

- The article "Τα γλωσσικά ιδιώματα του νομού Κοζάνης ως βόρεια και οι κυριότερες ιδιορρυθμίες τους" is indexed under Α. Ι. Θαβώρης (Μακεδονικά 29, 1994), not Κ. Ντίνας.
- The Κοβεντάρειος library's domain is kozlib.gr (catalogue.kozlib.gr, opac.kozlib.gr, atom.kozlib.gr), not kdbk.gr.
- Κοζανιτολόγιο (Χριστοδούλου 2017) should be added to the pointers as the largest Kozani lexicon.

## Next steps

1. Fix the environment's network access and re-run the ten section briefs in verification mode (open every URL, replace the markers, drop rows that do not exist).
2. Replace section 10 with the re-run result if it arrives, otherwise redo it with network access.
3. Place the files into the Claude Docs document for Kozani as HANDOVER.md section 5 describes.
4. Ask the author the three questions at the end of section 13 before the Pontic and Cretan sessions, since the same network setting will block them too.

# Cretan inventory: report

Oct 20, 2026 · session report for the Cretan Greek tutor inventory, files docs/cretan/00-scope.md to 13-open-questions.md

## Status

All fourteen files are written and committed: scope, ten research sections (1 grammar, 2 lexicon, 3 corpora, 4 audio, 5 teaching, 6 orthography, 7 variation, 8 pedagogy, 9 tools, 10 people) and three synthesis sections (11 disagreements, 12 top ten, 13 open questions). Every file passes the style check: no em or en dashes, no semicolons, six columns in every table row, one "Not found" line per section.

Two constraints shaped this session and must be read before the tables.

1. The cloud environment's network policy allowed web search but refused every page fetch outside github.com. No page outside GitHub was opened. Every row that rests on search results carries the marker [unverified: search only], and its URL is the one the search returned. Rows confirmed on a GitHub page carry no marker. The verification pass the conventions require (open every link, confirm sizes, licences, death years, contact pages) has not been done and is the first task for a session with ordinary network access.
2. The web search budget is shared across parallel agents and capped per turn. Sections 7, 8 and 10 were rerun after their first versions ran out of budget, and sections 6 and 9 were resumed. Sections 5, 6 and 7 still list in their "Not found" lines some items that were not searched, as distinct from items searched and not found.

The author was not available, so the scope section assumes nothing in hand beyond GRDD and GRDD+, and lists the Τμήμα Φιλολογίας holdings as an open question.

## What was found

Grammar. No reference grammar of contemporary spoken Cretan written with modern methods exists. The rules must be assembled from Πάγκαλος's 1955 grammar outline (the only full paradigm set), Χαιρετάκης's 2020 Patras thesis on inflection and derivation, Κοντοσόπουλος's east vs west feature lists, and the University of Crete phonetics papers on palatalisation, affrication and the retroflex /l/. No study of clitic placement, negation or word order in contemporary spoken Cretan was found, and no linguistic study of Σφακιά.

Lexicon. The large dictionaries (Πάγκαλος, Ξανθινάκης, Πιτυκάκης, Ιδομενέως, Τσιριγωτάκης, Ξενάκη-Ροβίθη) are print and copyrighted, with no entry counts found for the three main ones. The only open machine-readable lexical data are 273 Wiktionary headwords (CC BY-SA), the UD_Greek-Cretan treebank (1,009 lemmas, CC BY-SA 4.0) and the dilemma lemmatizer (MIT). Κονδυλάκης's 4,000-word list is public domain but exists only in print.

Texts. The loadable public-domain text is the Renaissance corpus on Βικιθήκη (Ερωτόκριτος, Ερωφίλη) and the Anemi scans of Κριάρης 1920 and Βλαστός 1893. The largest contemporary sources (mantinades.gr with about 21,000 couplets, Ιδομενέως with 12,000) need permission.

Audio. The ILSP Cretan speech corpus (about 2 hours of transcribed eastern Cretan radio narrative, CC BY 4.0, extended to about 4 hours in 2026) and the xls-r-greek-cretan model are the only reusable Cretan speech and speech technology. Institutional sound archives (ΚΕΝΔΙ, ΚΕΕΛ, Μουσείο Κρητικής Εθνολογίας, Βικελαία) are untranscribed and on request. No Cretan text to speech exists.

Teaching and pedagogy. No course, textbook or app for learning Cretan exists. The only Cretan curriculum is Μαρίνα Τζακώστα's elective in Ρέθυμνο (from 2019). The pedagogy literature is small and centred on her group: attitude surveys show oral Cretan welcomed and written Cretan corrected, and one documented intervention (Καψάσκη 2018) builds a lesson sequence on mantinades. No competence test, prestige ranking or study of foreign learners was found.

Orthography. No complete Cretan spelling convention exists. Counts over the GRDD files give the de facto practice: historical Standard Greek spelling, κι, τσ, τζ digraphs, no diacritics, apostrophes for elision, and είντα as the majority form (2,744 against ίντα 201 and ήντα 29). The interrogative is publicly disputed in the Ηράκλειο press. ΚΕΝΔΙ's IPA table is the one explicit convention, for transcription only. The rule_dialnorm repository holds the only explicit Cretan to Standard Greek spelling rules found.

Variation. The east vs west and Σφακιά layers can rest on Κοντοσόπουλος's 1988 atlas (163 settlements, IPA) and a chain of regional lexica. Manolessou and Pantelidis warn that palatalisation is not island-wide. Urban speech, perceptual dialectology and the Christian diaspora are unstudied. The Muslim diaspora has one linguistic study (Cunda) and vitality reports for Al Hamidiyah.

Tools. Cretan tooling is GRDD-derived (classifiers with Cretan F1 0.92, the DI_detector app, LoRA adapters, Dialect_Trans, Greek_Rhyme, all in the author's account and non-commercial), ILSP's speech work, and the two open syntactic resources above. The spaCy Greek models are CC BY-NC-SA 3.0, not MIT.

People. Expertise sits in Ρέθυμνο (Κάππα and the Εργαστήριο Γλωσσολογίας, Τζακώστα, TALOS AI4SSH) and Athens (ΚΕΝΔΙ with Μανωλέσσου and Χαιρετάκης, ΚΕΕΛ, ΙΕΛ, Χαραλαμπάκης at the Academy). Rights sit in Ηράκλειο (ΠΕΚ, Βικελαία, ΕΚΙΜ).

## Implementable items

Items that load directly as data or state rules explicit enough to code. Licence or status in parentheses.

- ILSP Cretan speech corpus, its 2026 extension and xls-r-greek-cretan (CC BY 4.0 on the base card, others unverified).
- UD_Greek-Cretan treebank (CC BY-SA 4.0) and the dilemma lemmatizer and parser (MIT).
- Wiktionary Cretan categories (CC BY-SA 4.0).
- Ερωτόκριτος and Ερωφίλη on Βικιθήκη, Κριάρης 1920 and Βλαστός 1893 on Anemi (PD), Λιουδάκη 1933 once scanned (PD).
- Πάγκαλος 1955 vol. 1 paradigms and Χαιρετάκης 2020 inflection classes (facts free).
- Lengeris and Kappa 2016, Lengeris et al. 2014, Kappa 2001 and 2016, Tzakosta 2016, Granqvist 1997 (facts free): palatalisation, affrication, retroflex /l/, vowel assimilation environments.
- Newton 1972 (facts free): palatalisation as ordered rules.
- Κοντοσόπουλος's 1988 atlas, 1969 thesis and handbook (facts free): per-village regional values.
- The regional lexica as layer labels (Ξανθινάκης west, Πιτυκάκης Μεραμπέλλο, Κασσωτάκης Λασίθι with grammar chapters, Γαρεφαλάκης Σητεία, Ξενάκη-Ροβίθη Ηράκλειο, Περιστεράκης and Γερωνυμάκης Σφακιά), and the Σφακιά and Μυλοπόταμος retroflex /l/ rule (facts free).
- Manolessou and Beis 2006 (facts free): genitive indirect object.
- Condoravdi and Kiparsky 2001 (facts free): clitic trigger list, Cretan data unconfirmed.
- ΚΕΝΔΙ's IPA transcription table (open to adopt).
- Καψάσκη 2018 mantinada lesson protocol, Παπαγιαννάκη 2021 teacher questionnaire, Yiakoumetti 2006 bidialectal protocol (facts free).
- GreekBERT (MIT) and Hunspell el_GR (MPL, GPL, LGPL) as baselines for a Cretan error detector and spell checker.
- The author's GRDD classifiers, DI_detector, adapters and Dialect_Trans (own work, non-commercial terms).

## Open or public-domain items

- Public domain: Ερωτόκριτος, Ερωφίλη (Βικιθήκη), Κριάρης 1920, Βλαστός 1893 (Anemi scans), Λιουδάκη 1933 (PD since 2018), Ξανθουδίδης 1915 Ερωτόκριτος (editor died 1928, an Anemi PDF reported in section 6, not in section 3), Κονδυλάκης's word list (print only), Χατζιδάκις's Cretan studies (died 1941), Ο Πατούχας if Κονδυλάκης's 1920 death year holds.
- Openly licensed: ILSP Cretan speech corpus (CC BY 4.0), UD_Greek-Cretan (CC BY-SA 4.0), Wiktionary (CC BY-SA 4.0), dilemma (MIT), GreekBERT (MIT), Hunspell el_GR, Whisper (MIT), eSpeak NG (GPL-3.0), Common Voice Greek (CC0, no Cretan tag), the Λειβαδιωτάκης and Τζακώστα 2024 article (CC BY-NC-SA 4.0), the Ayiomamitou and Yiakoumetti 2017 article (CC BY), Wikipedia articles (CC BY-SA 4.0, pointer only), Αρχείο Αμαργιανάκη items (CC, version unverified).
- Free to read, not licensed for reuse: Κασσωτάκης's Λασίθι dictionary PDF, the MGDLT and ICGL papers, Κρητικά Χρονικά 1947 to 1960, the Κριαράς online epitome, the Τζακώστα papers on ResearchGate.

## Top ten

Full table with reasons and first actions in section 12.

1. ILSP Cretan speech corpus with the 2026 extension and the xls-r-greek-cretan model.
2. UD_Greek-Cretan with the dilemma lemmatizer and parser.
3. Πάγκαλος vol. 1 with Χαιρετάκης 2020.
4. Κοντοσόπουλος's 1988 atlas and his east vs west feature list.
5. The University of Crete phonetics papers with the ΚΕΝΔΙ IPA table.
6. The public-domain text: Ερωτόκριτος, Ερωφίλη, Κριάρης, Βλαστός, Λιουδάκη.
7. The GRDD spelling counts with the rule_dialnorm map.
8. The author's GRDD tool set.
9. Ξανθινάκης and Πιτυκάκης, with Κοντοσόπουλος's reverse dictionary as the first licence request.
10. Τζακώστα's Cretan pedagogy: syllabus, mantinada protocol, ΨηΜοΠΙ recordings.

## Points for the author

- The GRDD licence is stated inconsistently. The GitHub README says CC BY-NC-SA 4.0 for annotations, metadata and code, while the Zenodo record and the TALOS Open-Data copy say CC BY-NC-ND 4.0.
- The GRDD+ repository's Krikri training script contains a hard-coded Hugging Face token in two places. It should be revoked and removed from the history. The token value is not reproduced in any file of this inventory.
- The tutor's licence model decides how much of the inventory is usable. Most of the strongest items are non-commercial or need permission (section 13).
- The orthography decision cannot be avoided: είντα (corpus majority) against ίντα (etymological, argued in the Ηράκλειο press and used by Βικιλεξικό) against ήντα (literary tradition). Section 11 sets out the evidence.
- What the Τμήμα Φιλολογίας in Ρέθυμνο holds is unknown to this inventory and is the first question to put to Ιωάννα Κάππα.

## Verification tasks for a session with page access

1. Open every link in sections 1 to 10 and remove the [unverified: search only] marker where the page confirms the row.
2. Confirm entry counts for Ξανθινάκης, Πάγκαλος and Πιτυκάκης, and the living status of Ξανθινάκης.
3. Confirm Anemi scan status for Πάγκαλος vol. 1, Λιουδάκη 1933 and Ξανθουδίδης 1915.
4. Confirm death years for Κονδυλάκης, Καζαντζάκης, Πάγκαλος, Παπαγρηγοράκης and Ιδομενέως.
5. Read the licences of the ILSP corpus, its extension and the ASR models, and the terms of the Κριαράς online epitome, the Πύλη and mantinades.gr.
6. Settle the bibliographic conflicts listed in section 11 (atlas year, Πάγκαλος vol. 1 year, Ιδομενέως editions and publisher).
7. Re-run the items marked "not searched" in the "Not found" lines of sections 5, 6 and 7.

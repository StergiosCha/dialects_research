# Cretan inventory: report

Oct 20, 2026 · session report for the Cretan Greek tutor inventory (docs/cretan/00-scope.md to 13-open-questions.md)

## Status of the files

Final, researched by web search and committed: 00-scope, 01-grammar (18 rows), 02-lexicon (18 rows), 03-corpora (20 rows), 04-audio (16 rows), 05-teaching (16 rows).

Interim, committed as drafts and being rewritten: 06-orthography (its three GitHub-verified rows with spelling counts from the GRDD files are final, the search-based rows are being added), 07-variation, 08-pedagogy and 10-people (their first versions were written without search budget and rest on memory, marked as such in every row, full reruns are in progress), 09-tools (its GitHub-verified rows are final, the web-search rows are being added).

Not yet written: 11-disagreements, 12-top-ten, 13-open-questions. They are written from the filled tables and follow once sections 6 to 10 are final. This report will be updated at that point. The top ten below is provisional and rests on sections 1 to 5 plus the verified rows of 6 and 9.

Two constraints shaped this session and must be read before the tables. First, the cloud environment's network policy allowed web search but refused every page fetch outside github.com, so no page outside GitHub was opened. Every row that rests on search results carries the marker [unverified: search only] and its URL is the one the search returned. Rows confirmed on a GitHub page carry no marker. The verification pass the conventions require (open every link, confirm sizes, licences, death years, contacts) is the first task for a session with ordinary network access. Second, the web search budget is shared across the parallel agents and capped per turn, so four of the ten section agents ran out of searches before or soon after starting, which is why sections 6 to 10 are being redone in a second wave.

## What was found

Grammar. No reference grammar of contemporary spoken Cretan written with modern methods exists. The tutor's rules have to be assembled from Πάγκαλος's 1955 grammar outline (the only full paradigm set, Academy of Athens reissue from 1991), Κοντοσόπουλος's east vs west feature lists and his 1988 Γλωσσικός Άτλας της Κρήτης, Χαιρετάκης's 2020 Patras thesis on Cretan inflection and derivation (inflection classes per period), and the University of Crete phonetics papers (Lengeris and Kappa 2016 on palatalization and affrication of velars with stress and position conditioning, Lengeris, Kappa, Paracheraki and Sipitanos 2014 on the retroflex /l/ before back vowels in weak positions, Kappa and Tzakosta on vowel assimilation and epenthesis). Syntax is covered only by cross-dialectal studies: Condoravdi and Kiparsky's clitic trigger typology and Manolessou and Beis 2006 placing Crete on the genitive side of the indirect-object isogloss. No study of clitic placement in contemporary spoken Cretan, of Cretan negation or of the Σφακιά variety as such was found.

Lexicon. The large dictionaries are all print and copyrighted with no digital edition: Πάγκαλος (six glossary volumes, village attributions), Ξανθινάκης (west, Πανεπιστημιακές Εκδόσεις Κρήτης, 2023 printing), Πιτυκάκης (east, 1983), Ιδομενέως (11,300 entries), Τσιριγωτάκης (13,000 with derivatives), Ξενάκη-Ροβίθη (Ηράκλειο prefecture, 2019), Κασσωτάκης (Λασίθι plateau, 7,500 entries, free PDF on the author's site, no licence). No source gave an entry count for Ξανθινάκης, Πάγκαλος or Πιτυκάκης. The only open machine-readable lexical data are small: 273 Cretan-tagged Wiktionary headwords (CC BY-SA), the UD_Greek-Cretan treebank (1,009 lemmas with morphological features, CC BY-SA 4.0) and Κονδυλάκης's public-domain Κρητικόν λεξιλόγιον of about 4,000 words, which exists only in print. Κοντοσόπουλος's Αντίστροφο λεξικό (180 pp, Standard Greek to Cretan) is the cheapest item to license for production exercises.

Texts. The public-domain loadable text is the Renaissance corpus: Ερωτόκριτος and Ερωφίλη on Βικιθήκη, plus Anemi scans of Κριάρης 1920 (songs and mantinades) and Βλαστός 1893 (wedding mantinades), all authors dead before 1956. Λιουδάκη's 1933 mantinades are public domain since 2018 but no scan was confirmed. Modern critical editions (Αλεξίου, Κακλαμάνης, Bakker and van Gemert) are copyrighted apparatus. The largest contemporary dialect sources are mantinades.gr (about 21,000 user-contributed couplets) and Ιδομενέως's 12,000 printed mantinades, both needing permission. Κρητικά Χρονικά volumes 1947 to 1960 are digitised but open access is not a reuse licence. The GRDD Cretan part was built from web text, plays and Σφακιανάκης's Cretan translations of ancient drama (permission-only), so those should not be recollected.

Audio. One directly loadable resource exists: the ILSP Cretan speech corpus on Hugging Face, about 2 hours of transcribed eastern Cretan radio narrative (CC BY 4.0, mostly one speaker), extended in 2026 with western material to about 4 hours, with released ASR checkpoints (28.27 percent word error rate after fine-tuning). Everything else is untranscribed institutional sound (ΚΕΝΔΙ, ΚΕΕΛ, Μουσείο Κρητικής Εθνολογίας with about 1,453 tapes, the Harvard Notopoulos tapes) or broadcast and oral-history material under paid or permission-only terms (ΕΡΤ, Istorima). No Cretan text to speech exists.

Teaching. No course, textbook, app or lesson set for learning Cretan exists. The one Cretan-specific curriculum is Μαρίνα Τζακώστα's elective at the Παιδαγωγικό Τμήμα Προσχολικής Εκπαίδευσης in Ρέθυμνο (from 2019), whose syllabus is not online. The national curriculum requires dialect teaching since 2011 but gives Cretan no unit, so the tutor fills a gap rather than duplicating school material.

Orthography (verified part). No published complete spelling convention for Cretan was found. Counts over the GRDD Cretan file show the de facto convention of the texts already in hand: historical Standard Greek orthography, κι, τσ, τζ digraphs with no caron or diaeresis anywhere, apostrophes for elision (22,428 in 5.07 million characters), είντα 2,744 against ίντα 201 and ήντα 29, τσι 5,158, τση 3,783, τζη 1,035, εδά 1,704 against εδαέ 0, εκάμα 144 against ήκαμα 62. The GRDD+ additions drift toward Standard Greek spelling (μάτια 1,423 against μάθια 391). The hyphenated sandhi forms (τον-ε, αν-ε) are confined to the Σφακιανάκης translations.

Tools (verified part). Everything that treats Cretan as a class or a target is GRDD-derived and in the author's own GitHub account: the GRDD classifiers (LinearSVC Cretan F1 0.92, BiLSTM 0.88), the five-class DI_detector Flask app, the GRDD+ LoRA scripts and the krikri_dialectal adapters (the only released Greek dialect generation weights, research use only), the VarDial perplexity study (Cretan perplexity anomalously high, attributed to the rhymed folk genre of the subcorpus), the Dialect_Trans collection site (first Cretan to Standard Greek parallel data) and the Greek_Rhyme generator (rhyme verifier reusable, no mantinada corpus). Open Standard Greek baselines with confirmed licences: GreekBERT (MIT), Hunspell el_GR, Whisper (MIT), eSpeak NG and Piper Greek voices. The spaCy Greek models are CC BY-NC-SA 3.0, not MIT.

## Implementable items

Items whose source either loads directly as data or states rules explicit enough to code. Licence in parentheses.

- ILSP Cretan speech corpus and 2026 extension, with xls-r-greek-cretan and whisper-medium-cretan (CC BY 4.0 on the base corpus card, extension licence unverified): aligned speech for pronunciation feedback.
- UD_Greek-Cretan treebank (CC BY-SA 4.0): 270 sentences, 4,351 tokens, manual lemmas and features, sandhi voicing annotated, eastern layer, single speaker.
- Wiktionary Cretan categories (CC BY-SA 4.0) and the open-greek dilemma lemmatizer (MIT): lexicon seed and lookup.
- Ερωτόκριτος and Ερωφίλη on Βικιθήκη (PD, transcription edition to check), Κριάρης 1920 and Βλαστός 1893 on Anemi (PD, polytonic OCR needed): reading and mantinada text.
- Πάγκαλος 1955 vol. 1 (facts free, text Ask): verb endings, augment, pronoun and article paradigms.
- Χαιρετάκης 2020 (facts free): inflection classes for a lexicon with inflection tags.
- Lengeris and Kappa 2016, Lengeris et al. 2014, Kappa 2001 and 2016, Tzakosta 2016 (facts free): palatalization, affrication, retroflex /l/, vowel assimilation environments for the western layer.
- Newton 1972 (facts free): palatalization as ordered rules.
- Κοντοσόπουλος 2001 and 1988 (facts free): east vs west feature list and isoglosses for the regional switch.
- Manolessou and Beis 2006 (facts free): genitive indirect object for Cretan.
- Condoravdi and Kiparsky 2001 (facts free): clitic trigger list, Cretan-specific data unconfirmed.
- Χαραλαμπάκης's pronunciation-rendering section in Ξανθινάκης (facts free): a ready spelling layer, content unverified.
- GRDD classifiers, DI_detector, krikri_dialectal adapters, Dialect_Trans (CC BY-NC-SA 4.0 or research only, the author's own): detector and generation baseline, commercial use needs the author's decision.
- GreekBERT (MIT), Hunspell el_GR (MPL, GPL, LGPL): encoder for a Cretan error detector, affix engine for a Cretan spell checker.

## Open or public-domain items

- PD text: Ερωτόκριτος, Ερωφίλη (Βικιθήκη), Κριάρης 1920, Βλαστός 1893 (Anemi scans), Λιουδάκη 1933 (PD since 2018, scan unconfirmed), Ξανθουδίδης's 1915 Ερωτόκριτος text (editor died 1928, scan not found), Χατζιδάκις's Cretan studies (died 1941), Κονδυλάκης's Κρητικόν λεξιλόγιον (word list PD, 1990 edition's apparatus Ask, print only), Ο Πατούχας (PD if the 1920 death year holds, not returned by search).
- Open licensed: ILSP Cretan speech corpus (CC BY 4.0), UD_Greek-Cretan (CC BY-SA 4.0), Wiktionary (CC BY-SA 4.0), dilemma (MIT), GreekBERT (MIT), Hunspell el_GR, Wikipedia Cretan Greek articles (CC BY-SA 4.0, pointer only), Αρχείο Αμαργιανάκη Cretan music items (licence field "cc", version unverified), Common Voice Greek (CC0, no Cretan tag).
- Free to read, not licensed: Κασσωτάκης's Λασίθι dictionary PDF, Κοντοσόπουλος's Αριάδνη article, the MGDLT and ICGL papers, Κρητικά Χρονικά 1947 to 1960, the Κριαράς online epitome.

## Provisional top ten

1. ILSP Cretan speech corpus with its ASR models. The only transcribed Cretan speech, open, with a working recogniser for pronunciation feedback. Ask ILSP about the extension licence and the 23 undigitised Radio Mires tapes.
2. UD_Greek-Cretan. The only open morphologically annotated Cretan, a ready test set and paradigm seed for the eastern layer.
3. Πάγκαλος vol. 1 with Χαιρετάκης 2020. Together the paradigm tables and the inflection class system the morphology module needs. Facts are free, confirm whether Anemi serves the scan.
4. The University of Crete phonetics cluster (Lengeris, Kappa, Tzakosta). Codable pronunciation rules with stated environments for the western layer, and the people to ask for recordings.
5. Ξανθινάκης (west) and Πιτυκάκης (east) as the licensing targets for a real lexicon, with Κοντοσόπουλος's Αντίστροφο λεξικό as the small Standard Greek to Cretan list to license first.
6. The public-domain Renaissance and folk corpus (Ερωτόκριτος, Ερωφίλη, Κριάρης, Βλαστός). Loadable reading text and mantinada models at no cost beyond OCR cleanup.
7. Wiktionary plus dilemma. The open lexicon seed and a Cretan-aware lemmatizer for exercise checking.
8. The GRDD-derived tool set in the author's account (detector, adapters, Dialect_Trans). Already in hand, the main decision is its licence for a commercial app and a Cretan evaluation of the adapters.
9. Κοντοσόπουλος's east vs west feature lists and atlas. The evidence base for labelling forms regionally, since GRDD and GRDD+ carry no regional labels.
10. mantinades.gr and Ιδομενέως for contemporary verse, and Τζακώστα's course syllabus for the lesson sequence, all as permission requests.

## Points for the author

- The GRDD licence is stated inconsistently: the GitHub README says CC BY-NC-SA 4.0 for annotations, metadata and code, the Zenodo record and the TALOS copy say CC BY-NC-ND 4.0. Pick one and align the hosts.
- The GRDD+ repository's training script for Krikri contains a hard-coded Hugging Face token in two places. Revoke it and remove it from the history.
- The orthography decision the tutor cannot avoid: είντα (majority in GRDD) against ίντα (etymological, argued in the Ηράκλειο press). The GRDD counts in section 6 are the only quantitative basis found.
- What the Τμήμα Φιλολογίας in Ρέθυμνο holds (dialect archive, recordings, theses) is unknown to this inventory and is the first question to put to the department.

## Verification tasks for a session with network access

Open every link in sections 1 to 10 and confirm: entry counts for Ξανθινάκης, Πάγκαλος and Πιτυκάκης, Anemi scan status for Πάγκαλος vol. 1, Λιουδάκη 1933 and Ξανθουδίδης 1915, the death years of Κονδυλάκης, Καζαντζάκης, Πάγκαλος and Ιδομενέως, the Κριαράς and Πύλη terms of use, Βικιθήκη pages for Θυσία του Αβραάμ, Βοσκοπούλα, Απόκοπος, Κατζούρμπος, Πανώρια, Στάθης and Φορτουνάτος, the licence of the ILSP extended corpus, Common Voice's accent table, the Τζακώστα syllabus, and whether Condoravdi and Kiparsky 2001 contain Cretan data. Then re-run the items each section's "Not found" line marks as not searched.

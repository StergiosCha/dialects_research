# Cypriot Greek inventory: session report

Session of 20 October 2026. Input: the research report `inputs/cypriot_survey_sections_03-10` (PDF and text) and the exported sections 0 to 2. Output: `docs/cypriot/03-corpora.md` to `13-open-questions.md`, one file per section, committed one by one, plus this report.

## What was done

Sections 3 to 10 were converted from the PDF text dump into the six-column convention (Reference, Contents, Access, Reuse, Judgement, Contact), with the 114 hyperlinks recovered from the PDF's link annotations (the text dump had lost them), the citation badges stripped, the style rules applied (no dashes, no semicolons, ranges as "15 to 45", Greek titles in Greek), and copyright reasoned from death years. Every row was cross-checked by web search in Greek and English, items the draft missed were added, and sections 11 to 13 were written from the filled tables. Each file passed a checker for column count, dashes, semicolons, hyphen ranges, link syntax and the presence of exactly one heading and one "Not found" line.

Row counts after the session, with the draft's counts in parentheses:

| Section | Rows | Implementable | PD or Open | Rows verified on an opened page |
| --- | --- | --- | --- | --- |
| 3 Text corpora and texts | 19 (14) | 6 | 10 | 1 (hb20007 corpus, files counted) |
| 4 Audio and speech | 17 (11) | 3 | 6 | 1 (pocket-tts-greek listing in the kyutai README) |
| 5 Teaching materials and curricula | 18 (10) | 1 | 1 | 0 |
| 6 Orthography | 16 (9) | 9 | 5 | 2 (CG_Dictionary README, hb20007 README) |
| 7 Variation | 21 (12) | 3 | 5 | 0 |
| 8 Pedagogy and acquisition | 22 (12) | 2 | 4 | 0 |
| 9 Existing tools | 19 (11) | 4 | 11 | 5 (hb20007, CG_Dictionary, DialectBench, nlp_editor, Dimakis et al. repositories) |
| 10 People and institutions | 24 (15) | n/a | n/a | 1 (Common Voice locale list) |

## The limitation of this session, and what the next pass must do

The brief's main task for sections 3 to 10 was to open every page the earlier tool could not open. This cloud environment's network policy denied every host except package managers and raw.githubusercontent.com: WebFetch failed with DNS errors and curl received HTTP 403 from the proxy for anemi.lib.uoc.gr, el.wikisource.org, kypros.org, library.severis.org, ibcc.dighum.kcl.ac.uk, ucy.ac.cy, moec.gov.cy, pi.ac.cy, huggingface.co, aclanthology.org, frontiersin.org, lex-cy.com, archive.org, wikipedia.org and every other site tested. Web search worked, so each row was checked against search results, which caught the errors listed below, but a search result is not an opened page under the conventions. Therefore every row of sections 3 to 10 still carries `[unverified: page not opened]` except the rows built from files opened on GitHub (listed in the table above). The markers are honest, and the links in every Reference cell are the pages the next pass has to open.

To finish the verification, run one more session with network access set to full, or with these hosts allowed: anemi.lib.uoc.gr, el.wikisource.org, el.wikipedia.org, en.wikipedia.org, el.wiktionary.org, kypros.org, library.severis.org, ibcc.dighum.kcl.ac.uk, www.ucy.ac.cy, gnosis.library.ucy.ac.cy, lekythos.library.ucy.ac.cy, library.ucy.ac.cy, www.moec.gov.cy, www.pi.ac.cy, mefesi.pi.ac.cy, kea.schools.ac.cy, sch.cy, gov.cy, huggingface.co, datacollective.mozillafoundation.org, mozilladatacollective.com, aclanthology.org, arxiv.org, www.frontiersin.org, pasithee.library.upatras.gr, euralex.org, benjamins.com, jbe-platform.com, tandfonline.com, academic.oup.com, sciencedirect.com, wiley.com, researchgate.net, academia.edu, ktisis.cut.ac.cy, pure.unic.ac.cy, eprints.rclis.org, eskep.ekt.gr, ich.unesco.org, moufflon.com.cy, iris.unive.it, edizionicafoscari.unive.it, multicast.aspra.uni-bamberg.de, fd-repo.uni-bamberg.de, ouc.ac.cy, universiteitleiden.nl, ru.nl, icrea.cat, westminster.ac.uk, berks.psu.edu, parathyro.politis.com.cy, news.rik.cy, apps.apple.com, play.google.com, cyprusays.com. That pass should open each link, confirm or correct the cell, and delete the marker. The list of facts that change a decision is in section 13.

## Corrections made to the draft (from search evidence, each still to be confirmed on the page)

- The ACL W09-0501 paper on extreme-case formulations is by Maria Christodoulidou (Frederick University), not Themistocleous.
- Themistocleous 2019: best accuracy 81 percent with formants, not 69 percent for a random forest.
- Common Voice el-CY exists as standalone datasheets (v1.0, 15 September 2025, 1,284 clips, 11 hours, v3.0, 22 March 2026, 1,221 clips, 10.37 hours), not only inside the shared-task bundle, but it has no locale on the main Common Voice platform (verified in the locale list on GitHub).
- The DialRes 2026 ASR paper has six authors (Stamou, Armostis, Klimi, Paraskevopoulos, Katsouros, Anastasopoulos), LREC 2026, pages 308 to 314.
- ΚΕΕ cassettes: 7,046 in the catalogue record of Ανδρέου and Ζέρβας 2003, the draft's 7,045 is the UCY page figure.
- Λιασίδης *Άπαντα*: τόμ. Α΄ 1997 (378 pp), τόμ. Β΄ 1998 (428 pp), Βικιπαίδεια dates the edition 2003.
- Λιπέρτης on Ανέμη: volumes 1923, 1930 and 1934 appear to be digitised, the 1937 volume was not found. The draft's page counts were not confirmed.
- The Γιαγκουλλής *Corpus* continues to τόμ. Ζ΄ (2023), the *Παραμύθια της Κύπρου* series runs to τόμ. 5.
- Τσιπλάκου's *Γλωσσική ποικιλία και κριτικός εγγραμματισμός* is a 2007 chapter in Ματσαγγούρας (ed.), Γρηγόρης, 466 to 511, mirrored by the ΠΙ. Τσιπλάκου and Χατζηιωάννου is dated 2010 (Μελέτες για την Ελληνική Γλώσσα 30).
- The Οδηγός Διαχείρισης Κοινωνικοπολιτισμικής Ετερότητας is 2018, edited by Τσιπλάκου with Αρμοστή, Ιωαννίδου is one of the writing group.
- Cyprusays: launched October 2025 by Effie and Costas Athanassiou in Sydney, App Store seller Karava Tech Pty Ltd.
- "The linguistic ecology of Cyprus" is Vida-Männl, Buschfeld and Grohmann 2025 (HSLD 9), the Frontiers 2022 perceptual study is Fotiou and Grohmann, Tsiplakou 2014 is in SILV 16 (163 to 178), Kappler and Tsiplakou is 2018 (MLR 25).
- Armostis 2020 at kormakitis.net is his Cypriot Arabic paper with Karyolemou, not an orthography paper. His 2022 orthography paper's title and venue were found (Ioannina 2019 workshop, vlahoi.net).
- Papapavlou and Pavlou 2005 is University Studio Press, not Cambridge Scholars (their 2007 volume is). Ioannidou 2009 is in Language and Education, not Linguistics and Education.
- Grohmann, Pavlou, Fotiou and Leivada is 2024, Edizioni Ca' Foscari, open access.
- The Chatzikyriakidis et al. 2026 VarDial paper's title is *Perplexity as a Metric for Dialectal Distance: A Computational Study of Greek Varieties*, and the GRDD+ paper (arXiv 2511.03772) is Chatzikyriakidis, Papadakis, Papaioannou and Psaltaki, LREC 2026.
- The hb20007 repository has a LICENSE.md (MIT) and 748 sentences (429 CG, 319 SMG), not the "about 7,000 CG sentences" of the GRDD paper, and the draft's "CC BY-SA 4.0" for the thesis is not stated anywhere in the repository.
- Multi-CAST Cypriot Greek is hosted at Bamberg, not on Zenodo as section 2 states.
- Affiliations (section 10): Armostis is Assistant Professor at Πανεπιστήμιο Κύπρου, Department of English Studies, so section 1's "European University Cyprus" should be corrected. Hadjioannou is Associate Professor at Penn State Berks and does not appear in the July 2025 promotion list the draft cited. Themistocleous is Associate Professor at the University of Oslo (2022 to present). Yiakoumetti is Senior Lecturer at Oxford Brookes. Eftychiou (Lombardo) is adjunct faculty at the University of Nicosia. Pavlou's current post and Μητσιάκη's institution were not found.

Items added that the draft lacked: Σάθας 1877 (the Ασσίζες), Multi-CAST Cypriot Greek, the τσιαττιστά anthology of Γιαγκουλλής 2011, the TV series row, pocket-tts-greek (two Cypriot voices), the ΡΙΚ pricing policy and Ψηφιακός Ηρόδοτος, Fakotakis 2004, the podcast Πε μας τα λλίον, Πισσούριος 2019 *Μαθθαίννω Κυπριακά* (the only CG textbook), the 2010 and 2016 curricula, the Georgiou and Karatsareas 2026 UK schools study, Αρμοστής et al. 2016 on synizesis, Αρμοστής 2017 on the apostrophe, Papadima et al. (ΤΕΠΑΚ), Themistocleous 2010 on Greeklish, the xkeyboard-config code points, Papapavlou 1998, 2001 and 2009, Goutsos and Karyolemou 2004, Karatsareas 2018 and 2025, Ioannidou, Ralli, Neokleous and Andreou 2019 on Turkish Cypriot Greek, Κοντοσόπουλος, Hadjioannou, Tsiplakou and Kappler 2011, Ioannidou 2009 and 2012, Sophocleous and Wilks 2010, Theodorou et al. 2017, Grohmann and Kambanaros 2016, Pavlou and Christodoulou 2001, Tsiplakou, Ioannidou and Hadjioannou 2018, Cylingo, nlp_editor (GPL v3), Dimakis et al. 2025, Orthos, PetrosStav F5-TTS-Greek, and nine people or institutions in section 10.

## Implementable items

Sections 3 to 9 mark 28 rows Implementable. The ones that matter most:

- Texts: Μιχαηλίδης on Βικιθήκη and Λιπέρτης on Ανέμη (PD), the hb20007 corpus (MIT, verified), Multi-CAST Cypriot Greek (CC BY 4.0, glossed), Common Voice el-CY transcripts (CC0, no re-hosting).
- Speech: Common Voice el-CY audio, parakeet-tdt-0.6b-v3-greek (ASR, 26 percent WER on Cypriot speakers), pocket-tts-greek (TTS with two Cypriot voices). Licences on the cards still to be opened.
- Orthography: the Συντυχιές convention (Armosti et al. 2014, the two EURALEX 2012 papers, Αρμοστής et al. 2012 on postalveolars, 2016 on synizesis, 2017 on the apostrophe), the xkeyboard-config code points, the parallel spellings of *Η 9η Ιουλίου* and the Λιπέρτης title variants as normaliser tests.
- Grammar and variation: Kappler and Tsiplakou 2018 (koine feature list), Grohmann, Papadopoulou and Themistocleous 2017 (clitic variation rates), Grohmann, Pavlou, Fotiou and Leivada 2024 (placement patterns), Theodorou et al. 2017 (24 CG sentences), the ΠΙ Οδηγός 2018 (contrastive rules for teachers).
- Tools: hb20007 classifier (MIT), nlp_editor IPA converter (GPL v3, early), DialectBench scaffold (Apache 2.0).

## Open or public-domain items

42 rows in sections 3 to 9 are PD or Open. Public domain: Μιχαηλίδης (from 1988), Λιπέρτης (from 2008), Σάθας 1877 (editor d. 1914), Dawkins 1932 and 1964 (from 1 January 2026). Open with a named licence: hb20007 (MIT), DialectBench (Apache 2.0), nlp_editor (GPL v3), mandododo Whisper models (MIT), Multi-CAST (CC BY 4.0), Common Voice el-CY (CC0 with a no re-hosting clause), Wiktionary (CC BY-SA 4.0), the Frontiers, ACL Anthology, Ca' Foscari and Languages papers (CC BY), parakeet and pocket-tts-greek (CC BY 4.0, unverified on the card), Krikri models (Llama 3.1 terms, unverified). LEXcy at lex-cy.com declares its data reusable with attribution but offers no download.

## Top ten (section 12)

1. Pavlou 2018 for the verbal paradigms and verb position.
2. The clitic placement rule set (Agouraki, Chatzikyriakidis, Liapis) with the variation rates.
3. Wiktionary Κυπριακά (CC BY-SA 4.0) as the lexicon seed.
4. The PD verse of Μιχαηλίδης and Λιπέρτης, plus Σάθας for the Ασσίζες.
5. The speech stack: Common Voice el-CY, parakeet ASR, pocket-tts-greek TTS.
6. The Συντυχιές orthography convention and the normalisation table.
7. LEXcy and the Συντυχιές database, by export request to Κατσογιάννου and Algolysis.
8. ΚΟΜΟΛεξ nominal paradigms, by request to Μητσιάκη.
9. The hb20007 classifier with GRDD+ as the register detector.
10. The teaching layer: ΠΙ Οδηγός 2018, Yiakoumetti 2005 to 2007, Πισσούριος 2019, Cyprusays 2025.

## Files

- `docs/cypriot/03-corpora.md`, `04-audio.md`, `05-teaching.md`, `06-orthography.md`, `07-variation.md`, `08-pedagogy.md`, `09-tools.md`, `10-people.md`: converted and cross-checked sections, one heading, lead, table and "Not found" line each.
- `docs/cypriot/11-disagreements.md`: ten linguistic disagreements with the decision for the tutor, plus the bibliographic conflicts to settle.
- `docs/cypriot/12-top-ten.md`: ranked list with licence step and first action.
- `docs/cypriot/13-open-questions.md`: decisions for the author, permission requests in priority order, facts to verify, resources that do not exist.
- The scratch files used (per-section text, the recovered link list, the checker) were not committed.

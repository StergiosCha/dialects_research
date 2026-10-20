# Handover: Greek dialect tutor, inventories of existing resources

Prepared 20 October 2026 for Claude Code cloud sessions (claude.ai/code, Desktop Code tab with Cloud selected, or `claude --cloud`), which spend the cloud session credits. Everything below is self-contained. One cloud session per variety.

OUTPUT FORMAT FOR CLOUD SESSIONS: you cannot assume access to the Claude Docs connector. Write every finished section as its own markdown file under sections/<variety>/NN-title.md (NN = two-digit section number, 00 for scope and conventions), commit after each file, and at the end write sections/<variety>/REPORT.md (what was found, the Implementable items, the open or public-domain items, the top ten). The main session will place the files into the Claude Docs documents afterwards. If the Claude Docs connector is available, you may additionally replace the pending blocks in the Cypriot document, but the files are the deliverable.

## 1. What we are building

A language-tutor app for Greek dialects, starting with Cypriot Greek, then Kozani (Western Macedonian, Northern Greek), Pontic and Cretan. The tutor needs: grammar rules and paradigms explicit enough to implement, a lexicon it may legally load, example texts and audio it may legally reuse, and a clear view of what already exists in teaching materials, orthographic conventions, regional variation, pedagogy research and NLP tools, so nothing is rebuilt that can be licensed or reused and so register decisions (koine vs regional, acrolectal vs basilectal) rest on published evidence.

The output of this work is one inventory document per variety. The documents are the input to the design of the tutor, they are not the tutor.

## 2. The Cypriot Greek document (exists, partly filled)

Claude Docs artifact: https://claude.ai/code/artifact/12ed4e4a-fc68-43b2-9f66-84848ba7c91c
Title: "Cypriot Greek tutor: inventory of existing resources". Dated 10 October 2026.

Done:
- Scope and conventions (items already in hand, columns, reuse codes, verification marker).
- Section 1, Grammatical descriptions: 26-row table (Pavlou 2018, Agouraki 2001, Terzi 1999, Condoravdi and Kiparsky 2001, Revithiadou 2006, Chatzikyriakidis 2010 and 2012, Pappas 2014, Papanicola and Armostis 2021, Grohmann et al. 2021, Neokleous 2015, Tsiplakou's clitic chapter, Liapis on έντζε, Pavlou on -ντε, Pavlou et al. on εμπού clefts, Tsiplakou 2017, Tsiplakou and Moser on the past perfect, Terkourafi 2005, Tsiplakou et al. 2006 and later on levelling, Arvaniti 2010 twice, Armostis 2011, Arvaniti 2001 and Christodoulou 2007 on geminates, Eftychiou 2009 and 2010, Themistocleous 2017, Χατζηιωάννου's grammar), each row flagged Implementable where the source states conditions codable as rules, plus a "Not found" line.
- Section 2, Lexical resources: 16-row table (Σακελλάριος 1891 PD on archive.org, Μενάρδος 1969, Κυπρή Υλικά 1979 to 1989, Χατζηιωάννου 1996, Γιαγκουλλής 2014 and 1997 and 2005, Παπαγγέλου 2001, Συμεωνίδης 2014 and 2017, ΚΟΜΟΛεξ morphological dictionary, Συντυχιές database (offline, ask Κατσογιάννου for the Access file), lex-cy.com (open with attribution, no bulk download), Χατζηπιερής and Καπατάς 2015, Wiktionary el and en (CC BY-SA, the only open machine-readable lexicon), community web dictionaries, the Cyprus Food Museum lexicon, small web glossaries), plus a "Not found" line.

ALREADY RESEARCHED, NEEDS VERIFICATION AND CONVERSION: a separate research report, `inputs/cypriot_survey_sections_03-10.pdf` (text in `.txt`), already covers Cypriot sections 3 to 10 in the same six-column format with leads and "Not found" lines. Its weakness: many rows say "[unverified: page not opened]" or "fetch blocked" because the tool that wrote it could not open anemi.lib.uoc.gr, Wikisource, kypros.org, Severis, KCL and other sites. The Cypriot session's job for sections 3 to 10 is therefore: read the report, open every page it could not open, confirm or correct each row (sizes, licences, URLs, death years, contact pages), add items it missed, drop items that do not exist, and write each section as `docs/cypriot/NN-title.md` in the conventions below. Do not research these eight sections from scratch. Sections 0 to 2 are done and exported in `docs/cypriot/00-02_scope_grammar_lexicon_from_claude_doc.md`: read them, they feed sections 11 to 13.

Pending (eleven blocks, each already planted in the doc with its intent, fill each by replacing its pending block with a "## heading" plus lead plus table):
3. Text corpora and texts: written, spoken, social media, folk material, public-domain literature (Μιχαηλίδης d. 1917, Λιπέρτης d. 1937, Μαχαιράς via Dawkins 1932, Βουστρώνιος, Ασσίζες), copyrighted dialect poets (Λιασίδης d. 1985, Μόντης), τσιαττιστά, CG theatre, TV scripts, with copyright status reasoned from author death year plus 70.
4. Audio and speech: recordings, speech corpora, TTS and ASR, podcasts, broadcast archives (ΡΙΚ), oral-history archives (ΚΕΕ oral tradition archive).
5. Teaching materials and curricula: the 2010 Cyprus Greek-language curriculum and its dialect component, Cyprus Educational Mission UK, textbooks, apps, courses, YouTube.
6. Orthography: proposals and conventions (Συντυχιές convention, Armostis et al. orthography paper, Katsoyannou et al.), the εν/έν accent convention, Roman-script and Greeklish practice, who uses what.
7. Variation: atlases, regional studies, sociolinguistic studies, diaspora (UK, Australia).
8. Pedagogy and acquisition: bidialectal education, interventions, instruments, attitudes (Ioannidou, Tsiplakou, Papapavlou, Yiakoumetti).
9. Existing tools: NLP software, dialect identification, language models, licences (CG in Greek dialect datasets, Themistocleous's tools, any CG ASR models, GRDD-trained classifiers).
10. People and institutions with contacts.
11. Disagreements between sources on grammatical facts (write from the filled tables, e.g. Armostis vs Arvaniti on the cue to gemination, categorical vs variable clitic placement).
12. Ranked top ten items for the tutor with reasons.
13. Open questions and gaps.

Items already in hand for Cypriot (do not re-inventory): Newton 1972, Andreou 2nd ed., Arvaniti's JIPA illustration, GRDD and GRDD+, Ioannidou, Karatsareas, Tsiplakou and Lytra 2020.

## 3. Conventions used in every document

Columns, exactly six, in this order: Reference | Contents | Access | Reuse | Judgement | Contact.
- Reference: author, year, title in italics, publisher or venue, markdown link to the page actually opened.
- Contents: what is in it (entries, words, hours, format: print, PDF, website, XML, CSV).
- Access: Open PDF, Website, Print, Paywalled, Download, On request.
- Reuse: PD (public domain), Open (licence allows reuse with attribution, name the licence), Ask (copyrighted or unclear, needs the holder's permission), No (reuse excluded by terms). Add a reason in parentheses when useful.
- Judgement: one short phrase on value for the tutor. Prefix **Implementable.** when the item can be loaded directly as data or states rules explicit enough to code.
- Contact: person or institution, or [unverified].

Rule stated in the doc: facts a source describes can inform the tutor's grammar without permission. Its example sentences, tables, word lists and recordings cannot.

Verification: every fact is taken from a page that was opened (a search snippet is not a source). Anything not confirmed on a primary or institutional page is marked [unverified]. Never invent URLs, sizes, dates or licences. Search in Greek as well as English. Each section ends with one line starting "Not found:" listing what was looked for and not found.

Style, strict: no em dashes or en dashes anywhere, ranges written "15 to 45", commas, colons, parentheses or full stops instead. No semicolons in prose. Compact cells. Greek titles in Greek. No filler phrases.

## 4. Method that worked

One research agent per section, in parallel, each given: the goal (section 1 of this file), the section's scope and a list of items it must cover at minimum, the conventions (section 3), and the instruction to return only the heading, a one or two sentence lead stating the main finding, a 10 to 16 row table and the "Not found" line. The section-2 agent used about 100 tool calls and ten minutes. The three synthesis sections (disagreements, top ten, open questions) are written by the main session from the filled tables, not delegated. Place each section into the doc as it arrives (replace its pending block), so the author can watch and stop a section that goes wrong. Finish with a verification pass: no pending blocks left, every link opens, no em dashes or semicolons, every [unverified] still justified.

Agent brief template (replace the bracketed parts):

"You are researching one section of an inventory document, '[variety] tutor: inventory of existing resources', for Stergios Chatzikyriakidis (computational linguist building a [variety] language-tutor app that needs implementable grammar rules, a lexicon, reusable texts and audio). Your section: '[number]. [title]'. METHOD: use web search (extended mode for niche or Greek-language items) and open every page you take facts from, put a markdown link to the opened page in the Reference cell, mark anything not confirmed on a primary or institutional page with [unverified], never invent URLs, sizes, dates or licences, search in Greek as well as English. COVER AT LEAST: [list]. TABLE COLUMNS: [section 3 of this file]. STYLE: [section 3 of this file]. RETURN ONLY: the '## [number]. [title]' heading, a one or two sentence lead stating the main finding, the pipe table with 10 to 16 rows, then one line starting 'Not found:'."

## 5. The three new documents

Create one Claude Docs document per variety with the same skeleton as the Cypriot one: title "[Variety] tutor: inventory of existing resources", byline (as-of date chip and the author), a Scope and conventions section (items in hand, columns, reuse codes, verification marker), then thirteen sections in the same order: 1 grammatical descriptions, 2 lexical resources, 3 text corpora and texts, 4 audio and speech, 5 teaching materials and curricula, 6 orthography, 7 variation, 8 pedagogy and acquisition, 9 existing tools, 10 people and institutions, 11 disagreements, 12 ranked top ten, 13 open questions and gaps. Plant them all as pending blocks first, fill one per call.

Items already in hand for all three: GRDD and GRDD+ (they contain Cretan, Pontic and Northern Greek text). Ask the author what else he holds before starting, if he is available. If not, proceed and list the assumption in the scope section.

Variety-specific notes and starting pointers. These come from memory and must be verified before they enter a table.

Kozani (Western Macedonian, a Northern Greek variety). Expect the thinnest literature, so the "Not found" lines carry weight. Key phenomena the tutor needs: unstressed high-vowel deletion and mid-vowel raising, the resulting consonant clusters and stress patterns, accusative for indirect objects, the local lexicon with Slavic, Turkish, Aromanian and Albanian loans, carnival (Αποκριά, φανοί) song texts as a folk corpus. Pointers: Κώστας Ντίνας, Το γλωσσικό ιδίωμα της Κοζάνης (two volumes, Ινστιτούτο Βιβλίου και Ανάγνωσης Κοζάνης, 2005, to verify). The Κοβεντάρειος Δημοτική Βιβλιοθήκη Κοζάνης and its digitised collections. Local glossaries published by the Λαογραφικό Μουσείο Κοζάνης and in Ελιμειακά. Newton 1972 and Trudgill 2003 for the Northern vowel system in general. Any Kozani material in the Ιστορικό Λεξικό της Νέας Ελληνικής (Ακαδημία Αθηνών) and in the ΚΕΝΔΙ archive. Kozani speech recordings on YouTube and in local radio archives. Check whether the dialect-ID literature treats Kozani separately or only as "Northern".

Pontic. The largest literature of the three. Decide early, and state in the scope section, which Pontic the tutor teaches: the Greece-based koine of the refugees' descendants, or Romeyka of Trabzon, or both with marked differences. Pointers: Ά. Α. Παπαδόπουλος, Ιστορικόν λεξικόν της ποντικής διαλέκτου (two volumes, 1958 to 1961) and Ιστορική γραμματική της ποντικής διαλέκτου (1955). Δ. Οικονομίδης, Γραμματική της ελληνικής διαλέκτου του Πόντου (1958). Georges Drettas, Aspects pontiques (1997). Ioanna Sitaridou's Romeyka work (Cambridge, the Romeyka project and its recordings). Peter Mackridge 1987 on the Pontic of Of. Δ. Τομπαΐδης. The Επιτροπή Ποντιακών Μελετών and its journal Αρχείον Πόντου. The Pontic Wikipedia (pnt.wikipedia.org, CC BY-SA, size to check). Pontic song and theatre corpora, Pontic radio and TV, the Pontic lyra tradition's lyric texts. Pontic courses offered by associations and universities (Θεσσαλονίκη, Κομοτηνή), textbooks such as those of the Παμποντιακή Ομοσπονδία. Orthography: the competing conventions for the Pontic vowels (ä, ö, ü vs Greek digraphs) and who uses which. NLP: any Pontic entries in Greek dialect datasets, Pontic machine translation attempts, ASR.

Cretan. Pointers: Ν. Κοντοσόπουλος, Διάλεκτοι και ιδιώματα της Νέας Ελληνικής and Γλωσσογεωγραφική μελέτη of the Cretan dialect. Γ. Πάγκαλος, Περί του γλωσσικού ιδιώματος της Κρήτης (multi-volume, 1955 onwards, lexicon volumes). Α. Ξανθινάκης, Λεξικό ερμηνευτικό και ετυμολογικό του δυτικοκρητικού γλωσσικού ιδιώματος (Πανεπιστημιακές Εκδόσεις Κρήτης, 2000 and later editions). Μ. Πιτυκάκης, Το γλωσσικό ιδίωμα της Ανατολικής Κρήτης (1983). Public-domain literature: Ερωτόκριτος (Κορνάρος), Ερωφίλη and the Cretan Renaissance corpus (editions by Alexiou and others, the critical editions themselves may be copyrighted even where the text is not), Wikisource el holdings. Mantinada collections (large, mostly copyrighted compilations, some open sites). The Κρητικά Χρονικά and the Εταιρία Κρητικών Ιστορικών Μελετών. The east vs west division and the Sfakia variety. Cretan in Greek dialect datasets (GRDD already in hand), Cretan TTS or ASR attempts, Cretan courses and apps, the Πανεπιστήμιο Κρήτης Τμήμα Φιλολογίας dialect archive (the author knows this department, ask him what exists there).

## 6. Order of work and deliverables

Each cloud session handles one variety and is told which in its opening prompt.

Cypriot session: sections 3 to 10 by parallel research subagents (one per section), then sections 11 to 13 written by the main session from the filled tables, then a verification pass (every link opens, no em dashes or semicolons, every [unverified] justified). Files: sections/cypriot/03-corpora.md through 13-open-questions.md, then REPORT.md.

Kozani, Pontic and Cretan sessions: first write sections/<variety>/00-scope.md (title, as-of date, items in hand, columns, reuse codes, verification marker, the variety-specific decisions such as which Pontic the tutor teaches), then sections 1 to 10 by parallel research subagents, then 11 to 13, then verification, then REPORT.md.

Commit after every file so partial progress survives if the session expires.

The author's preferences for all written output: no em dashes, no semicolons in prose, natural Greek with correct Greek linguistic terminology, no AI self-narration phrases, direct statements.

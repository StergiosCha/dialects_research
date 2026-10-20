# Pontic inventory: session report

20 October 2026. Files: docs/pontic/00-scope.md to 13-open-questions.md. Branch claude/pontic-inventory-review-pi6pmg.

## Status of each file

| File | State |
|---|---|
| 00-scope.md | Done. Decision: tutor teaches the Pontic koine of Greece, Romeyka as comparison module. |
| 01-grammar.md | Done, 18 rows, 9 Implementable. |
| 02-lexicon.md | Done, 18 rows, 5 Implementable. |
| 03-corpora.md | Done, 18 rows, 2 Implementable. |
| 04-audio.md | Done, 18 rows, 1 Implementable. |
| 05-teaching.md | Done, 16 rows, 2 Implementable. Search budget ended before app-store and diaspora queries. |
| 06-orthography.md | Done, 14 rows, 5 Implementable (three GitHub projects opened directly). |
| 07-variation.md | Interim. Built from Glottolog on GitHub only, 18 rows. Needs a rerun with web search. |
| 08-pedagogy.md | Done, 16 rows, 4 Implementable. |
| 09-tools.md | Done, 18 rows, 6 Implementable, all from opened GitHub pages. |
| 10-people.md | Not done. Placeholder with the full query plan. The rerun agent was still working when the session was stopped for credits. Contacts are recoverable from the Contact columns of sections 1 to 9. |
| 11-disagreements.md | Done, 9 points. |
| 12-top-ten.md | Done. |
| 13-open-questions.md | Done, 25 items. |

## Session limitation

The cloud sandbox's network policy refused every host except github.com. Web search worked, page opening did not. Rows researched by search carry "[unverified: page not opened]" in the Reference cell (about 120 rows). GitHub-hosted rows were opened and carry no marker. A shared cap of 200 web searches per turn starved sections 7, 8 and 10 on the first pass. Section 8 was rerun successfully, section 10 was not completed. The verification pass described in the scope file (open every link, confirm sizes, licences, death years) must be run from a session with ordinary network access, as for the Cypriot survey.

## What was found

Nothing for the koine is both open and machine-readable except the Wiktionary material (103 English lemmas plus an uncounted Greek category, CC BY-SA) and the Pontic Wikipedia (681 articles, disputed quality). The largest structured lexicon is Lingua Pontica (about 20,000 lemmas with audio, Εύξεινος Λέσχη Βέροιας, no terms published). The resource that matches the target variety exactly is the ILSP 2026 Pontic speech corpus (Northern Greece conversations, Greek-script transcription chosen with the community, ASR baseline), unreleased. The only downloadable transcribed Pontic audio is the Göttingen Caucasus corpus (7 h 26 min, Georgian Pontic). The reference grammars (Παπαδόπουλος 1955, Οικονομίδης 1958, Drettas 1997) are print only, Οικονομίδης' own text is public domain. No Pontic ASR, TTS or MT exists. GlotLID is the only language identifier that recognises pnt. The only generative and classification tools covering Pontic are the author's own GRDD-trained ones.

## Implementable items

Grammar: Οικονομίδης 1958 (PD text), Παπαδόπουλος 1955 and Drettas 1997 (rules free to follow), Ρεβυθιάδου and Σπυρόπουλος 2009 Οφίτικα report (open PDF), Spyropoulos and Kakarikos 2009 nominal features, Michelioudakis and Sitaridou 2016 wh-fronting (CC BY), Kooij and Revithiadou 2002 stress, Armostis et al. 2020 JIPA inventory, Sitaridou 2014 infinitive conditions (Romeyka), Berikashvili 2017 (Georgian Pontic). Lexicon: Wiktionary via wiktextract (MIT tool, CC BY-SA data), Lingua Pontica on export. Teaching structure: Χατζόπουλος and Ιωακειμίδου 2022 (31 lessons), ΠΣΠΕ adult manual 2018, Veria YouTube lessons with quizzes. Orthography and input: msologr-cpu fonts (OFL 1.1), Keyman Pontic keyboard (MIT), fcitx5 layout (GPL 3.0), Wikipedia and Soviet mapping tables. Pedagogy instruments: Κωνσταντινίδου's learner error inventory, Konstantinidou and Kyridis 2014 questionnaire, Μαχαιρίδου's translation test, Schreiber and Sitaridou 2017 attitude survey. Tools: Glottolog pont1253 (CC BY 4.0), GlotLID (Apache 2.0), Pontic Wikipedia.

## Open or public-domain items

PD: Οικονομίδης 1958 text, Dawkins 1931 and 1937, Φωτιάδης' plays (died 1909), Παρχαρίδης' Of tales and proverbs (1884 to 1885), Ιωαννίδης 1870 and Κούσης 1883 to 1890 on Trebizond Greek, Soviet-era Pontic print pending Τοπχαράς' death year. Open licence: Wiktionary, Pontic Wikipedia, Glossa 2016 article, Sitaridou 2023 Keria paper (CC BY-SA per repository), Göttingen corpus (open access, licence name unconfirmed), Glottolog, GlotLID, the font and keyboard projects, the empty UD and treebank shells (CC BY and CC BY-SA declared).

## Top ten

See 12-top-ten.md: 1 ILSP speech corpus, 2 Lingua Pontica, 3 the two course books, 4 the reference grammars, 5 the open rule statements, 6 the orthography and input package, 7 Wiktionary via wiktextract, 8 Λιανίδης 1962 plus the PD texts, 9 the Göttingen corpus, 10 the pronunciation sources.

## Next steps

1. Rerun section 10 and section 7 in a session with network access (the query plans are in the files).
2. Run the verification pass over the "[unverified: page not opened]" markers.
3. Fold sections 8 and 9 into 11 and 12 where noted (item 7 of section 11, the tools row of the top ten).
4. Send the request letters listed in section 13, items 13 to 20, starting with ILSP and Εύξεινος Λέσχη Βέροιας.

# dialects_research

Resource inventories for a Greek dialect language-tutor app: Cypriot Greek first, then Kozani (Western Macedonian), Pontic and Cretan. Each inventory lists what already exists (grammars, lexica, corpora, audio, teaching materials, orthographies, variation studies, pedagogy research, NLP tools, people) with access and reuse status, so the tutor is built on licensed or open material and on published evidence.

Read HANDOVER.md first. It holds the goal, the conventions every table follows, the research method, the state of the Cypriot inventory, and the plan for the other three varieties.

## Layout

- `HANDOVER.md`: the brief for a research session. Self-contained.
- `inputs/cypriot_survey_sections_03-10.pdf` and `.txt`: a research report already produced for Cypriot sections 3 to 10 (text corpora, audio, teaching materials, orthography, variation, pedagogy, tools, people). Same six-column format. Many rows carry "[unverified: page not opened]" because the tool that produced it could not open some sites. These rows need re-verification, not rewriting.
- `docs/cypriot/00-02_scope_grammar_lexicon_from_claude_doc.md`: sections 0 to 2 of the Cypriot inventory as they stand in the Claude Docs document (scope and conventions, grammatical descriptions, lexical resources). Done, do not redo.
- `docs/cypriot/`, `docs/kozani/`, `docs/pontic/`, `docs/cretan/`: output folders. One markdown file per section, `NN-title.md`, plus `REPORT.md` at the end.

## Running the research (cloud sessions)

Start one Claude Code cloud session per variety from a clone of this repository (claude.ai/code, the Desktop app Code tab with Cloud selected, or `claude --cloud` in the terminal). Each session reads HANDOVER.md and does one variety:

```
claude --cloud "Read HANDOVER.md and do the Cypriot work: verify and convert inputs/cypriot_survey_sections_03-10 into docs/cypriot/03-*.md to 10-*.md, then write 11 to 13 and REPORT.md. Commit after every file."
claude --cloud "Read HANDOVER.md and do the Pontic inventory: docs/pontic/00-scope.md, then sections 1 to 13, then REPORT.md. Commit after every file."
claude --cloud "Read HANDOVER.md and do the Cretan inventory: docs/cretan/00-scope.md, then sections 1 to 13, then REPORT.md. Commit after every file."
claude --cloud "Read HANDOVER.md and do the Kozani inventory: docs/kozani/00-scope.md, then sections 1 to 13, then REPORT.md. Commit after every file."
```

Each session pushes its own branch. Merge the four branches when they finish.

## Conventions in one line

Six columns (Reference, Contents, Access, Reuse, Judgement, Contact), reuse codes PD, Open, Ask, No, every fact from an opened page with its link, [unverified] where not confirmed, a "Not found:" line per section, no em dashes, no semicolons in prose, ranges as "15 to 45".

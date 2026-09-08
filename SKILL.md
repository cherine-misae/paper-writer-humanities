---
name: paper-writer-humanities
description: Create a source-grounded humanities research report or article in literature, philosophy, intellectual history, cultural studies, and related text-based disciplines. Use for a specific question or corpus; do not use when quantitative, experimental, questionnaire, or model-evaluation evidence is central.
---

# Humanities Paper Writer

Produce a complete, reviewable humanities research report from a specific question, defined corpus, and appropriate interpretive method. Preserve the useful architecture of a long-running paper workflow—verified sources, incremental files, editable document source, and quality gates—without imposing experimental-paper conventions.

Never invent primary-source quotations, page numbers, archival identifiers, historical facts, or scholarly positions. Never create simulated evidence. When sources cannot support a claim, narrow or qualify it and record the limitation.

## Boundaries

Use this skill for source-based argument in literature, philosophy, intellectual history, cultural studies, art history, religious studies, or a comparable humanities field.

Do not use it when the central claim depends on statistical analysis, experiments, questionnaires, model evaluation, or numerical datasets. A humanities project may mention dates, counts present in sources, or bibliographic facts; “non-quantitative” means quantitative analysis is not the method of proof.

The deliverable is an AI-assisted research report or substantial manuscript draft requiring review by the researcher or a domain expert—not automatically publication-ready scholarship.

## Required intake

Establish these items before substantial research. Ask only for information that cannot be inferred safely.

- **Research question or argumentative problem**: more specific than a broad subject.
- **Primary corpus**: works, editions, translations, archival materials, or philosophical texts in scope. If none is supplied, propose a provisional corpus and obtain approval before close reading.
- **Scope**: period, language, geography, authors, works, concepts, and exclusions.
- **Approach**: close reading, conceptual analysis, comparison, reception history, genealogy, discourse analysis, archival interpretation, or another justified method. Do not force a theory onto the material.
- **Output language, citation style, and format**: infer language when clear; default to a generic author-date style, editable DOCX, and PDF. Use LaTeX only when the user or target venue requires it.
- **Source access**: user files, accessible full text, licensed records, or public sources. Record access limits.

Optional: intended audience, target length, venue or institutional format, working thesis, required scholars, prohibited sources, and deadline.

## Set up the run

Create a timestamped run that never overwrites an earlier run. Use one canonical topic string and record it in `project_manifest.md`.

```bash
TOPIC="<canonical topic>"
SLUG=$(python3 -c "import re,hashlib,sys; t=sys.argv[1]; n=re.sub(r'[\\s_]+','-',re.sub(r'[^\\w\\s-]','',t.lower().strip())).strip('-')[:40].rstrip('-'); h=hashlib.sha1(t.encode()).hexdigest()[:8]; print(f'{n}-{h}')" "$TOPIC")
TS=$(date +%Y-%m-%d_%H%M%S)
RUN="output/paper-writer-humanities/$SLUG/$TS/report"
mkdir -p "$RUN/sections" "$RUN/source_notes" "$RUN/figures" "$RUN/rendered"
cp -r "<skill-root>/assets/report-template/." "$RUN/"
ln -sfn "$TS" "output/paper-writer-humanities/$SLUG/latest"
```

Treat `$RUN` as `output/paper-writer-humanities/<slug>/latest/report/` thereafter. Do not substitute shortened paths such as `output/paper/`.

## Workflow

### 1. Plan and persist

Read [references/00-incremental-execution.md](references/00-incremental-execution.md). Write `project_manifest.md` with the approved question, corpus, scope, method, language, citation style, access limits, and intended deliverable. Draft a provisional argument map; keep it provisional until evidence has been examined.

### 2. Acquire and verify sources

Read [references/01-source-and-bibliography.md](references/01-source-and-bibliography.md). Search source types appropriate to the field rather than defaulting to arXiv or computer-science venues. Separate primary sources from secondary scholarship. Verify metadata from an authoritative record or the item itself.

There is no universal minimum source count. Adequacy depends on the question, corpus, genre, and available scholarship. Stop expanding when major positions and necessary primary materials are represented and further searching produces repetition rather than a meaningful new perspective. Record the rationale in `source_coverage.md`.

### 3. Build evidence records before prose

Read [references/02-evidence-and-quotation.md](references/02-evidence-and-quotation.md). Create a note in `source_notes/` for each source actually used. Maintain `evidence_ledger.md`, linking consequential claims to sources, locators, access level, and evidentiary role.

Quote only text inspected in this run or supplied by the user. Record the edition or translation and a stable locator. If only an abstract, snippet, catalog record, or review is available, do not quote or attribute a detailed argument to the unseen work.

### 4. Develop the argument and write sections

Read [references/03-argument-and-sections.md](references/03-argument-and-sections.md). Select a structure that follows the argument; do not force Method–Experiment–Results. A report normally contains an abstract or executive summary, introduction, scholarly context, method or positionality where relevant, two or more analytical sections, counterarguments or limitations, and conclusion. Merge, rename, or reorder these when the discipline or material calls for it.

Write one substantial Markdown section at a time. Before each section, identify its question, local claim, evidence, counterpressure, and connection to the thesis. After writing, update `evidence_ledger.md`, assemble the current manuscript, and inspect the rendered output before proceeding.

### 5. Add visuals only when analytically useful

Read [references/04-visuals-and-layout.md](references/04-visuals-and-layout.md) only when a timeline, concept map, textual genealogy, comparison table, source image, or other visual would materially clarify the argument. No figure, table, chart, equation, or architecture diagram is required. Never manufacture quantitative data to fill a visual slot.

### 6. Assemble and verify

Read [references/06-output-formats.md](references/06-output-formats.md). Use Markdown as the canonical editable source. By default, assemble it into `report.docx`, export or render `report.pdf`, and visually inspect both through page renderings. Preserve headings, quotations, footnotes or endnotes, citations, bibliography, tables, and non-Latin scripts across formats.

Use LaTeX only when the user requests it or a target venue supplies a LaTeX template. In that case, derive the LaTeX project from the same canonical manuscript and evidence records; do not make LaTeX the only editable source. Read [references/05-quality-gate.md](references/05-quality-gate.md) and remediate every blocking issue.

### 7. Deliver

Return:

1. `report.docx` and `report.pdf` by default, or the formats the user requested;
2. the canonical Markdown manuscript and complete editable source project;
3. `project_manifest.md`, `source_coverage.md`, and `evidence_ledger.md`;
4. a completion report covering length, source counts by class, quotation verification, access limits, citation status, and human-review status.

## Non-negotiable rules

- No fabricated citations, quotations, page numbers, archival identifiers, or scholarly positions.
- No simulated evidence, invented findings, or plausible-looking textual examples presented as source material.
- Distinguish primary, secondary, reference, and contextual sources.
- A fetched URL verifies only what was visible there. Metadata access is not full-text access.
- Prefer a smaller, fully used bibliography to a padded bibliography.
- Preserve disagreement; do not flatten contested interpretations into consensus.
- Separate source description, scholarly interpretation, and the report's own analysis.
- Do not infer intention, identity, influence, or causation without appropriate evidence.
- Identify editions and translations; do not silently translate quotations.
- Always recommend domain-expert review before academic submission or publication.
- Keep the DOCX, PDF, Markdown, and optional LaTeX versions substantively equivalent; no citation or qualification may disappear during conversion.

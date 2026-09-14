# Profile A — interpretive

**One-line definition**: existing documents are the evidence; every quotation can be checked by anyone against a stated edition and locator, so verification is about editions, locators, and faithful reading.

## §1 When to select
Select when the claim is established by reading, comparing, reconstructing, or contextualizing documents that already exist: literary or artistic works, philosophical arguments, historical sources, legal texts, or prior scholarship (literature synthesis). Do not select when the evidence is material the researcher collected (→ B) or datasets, corpora, experiments, or a formal model (→ C).

## §2 Evidence and definition of primary
Primary = the document interpreted, always with a stated edition, translation, manuscript, or record identifier. Evidence types: `primary text`, `scholarly argument`, `contextual fact`, `reference entry`. Carrel cannot supply a primary text the user has not provided or that is not accessible in full; if only a snippet, abstract, or review is available, the item is not primary evidence for a close-reading claim.

## §3 Additional intake questions
- Base edition and translation for each primary work (required if the user has a preference).
- Scholars or positions that must be engaged; sources that must be excluded.
- Policy on quoting in the original language with translation.
- Variant (see table); default `literary-interpretation`.

## §4 Acquisition and verification additions
Fix the edition before close reading and inspect the passages actually cited. Cover foundational, recent, and opposing scholarship. Confirm archival items and legal records by their official identifiers. Never let a secondary summary substitute for an accessible primary text.

## §5 Evidence ledger extra columns
`Edition/translation`, `Original language (Y/N)`, `Locator type` (page, line, stanza, section, folio, catalogue no., case no. + paragraph, article/clause). Report-made translations are marked `[Carrel translation]`.

## §6 Default structure
1. Abstract — problem, corpus, approach, argument, significance.
2. Introduction — question, corpus and scope, intervention, qualified thesis, path.
3. Scholarly context — organized by interpretive problem or debate, not by name list.
4. Edition, method, or terms — only when it clarifies selection and interpretation.
5–6. Two or more analytical sections with conceptual titles.
7. Alternative readings and limits — strongest rival reading; evidence limits vs. scope limits.
8. Conclusion.
9. References.

## §7 Section-writing rules
Analytical paragraph pattern: textual feature → precise observation → bearing on the claim → engagement with scholarship or a rival reading → link to thesis. Quote, then analyze; never end a paragraph on a quotation. Evidence voice: "the passage reads / the source states / the ruling holds". Identify editions and translations in the text or notes; never silently modernize or translate. Similarity ≠ influence; sequence ≠ causation; a single passage ≠ an author's view.

## §8 Required apparatus
`apparatus/visuals-and-tables.md` only if a comparison table, timeline, or image is used. `apparatus/images-and-plates.md` for any reproduced image. `apparatus/archival-locators.md` for the `historical-archival` variant. Legal and linguistic apparatus files as named in the variant table when they exist.

## §9 Additional quality gates
- G9 Edition check (visual): a sample of quotations is re-read against the stated edition.
- G10 Translation marking (script-checkable): every non-original-language quotation carries a translator or `[Carrel translation]`.
- G11 Exegesis/argument split (visual): reconstructions of an author's position are not merged with the report's own argument.
- G12 Secondary-as-primary (visual): no close-reading claim rests on a source whose access level is not `full-text` or `user-provided`.

## §10 Common failure modes
Reconstructing a quotation from memory; inventing a page, folio, case number, or article that does not exist; summarizing a scholar's book from its abstract; flattening a debate into consensus; straw-man objections; anachronistic concepts applied to earlier sources; treating a later text as "influenced" because it resembles an earlier one.

## §11 Neighboring profiles
B: the material was produced by or for the researcher (transcripts, field notes, case dossiers). C: the documents are counted, measured, or modeled rather than read. Literature synthesis stays in A unless it is a meta-analysis (→ C).

## §12 Assets
`assets/profiles/A/` — `sections/abstract.md, introduction.md, scholarly_context.md, method_or_edition.md, analysis_1.md, analysis_2.md, alternative_readings.md, conclusion.md`, and `report.md` skeleton.

## Variant table

**literary-interpretation** (default) — structure as §6. Fields: literature, art history, musicology, religious studies, cultural studies.

**argument-normative** — structure: problem → definitions → argument reconstruction → objections → replies → implications. Locator: section/paragraph of the reconstructed text; premises numbered. Extra gate: strongest available objection is engaged. Fields: philosophy, political theory, ethics, jurisprudence.

**historical-archival** — structure: problem and sources → source criticism and limits → chronological or thematic chapters → historiographic implications. Locator: archive / collection / box / folio; date of production. Apparatus: `archival-locators.md`. Extra gate: every dated event links to a source row. Fields: history, intellectual history, archaeology (documentary), historical linguistics.

**legal-doctrinal** — structure: facts and issue → legal question → authorities (case law, statute, commentary) → analysis → conclusion; comparative variant adds per-jurisdiction sections and a comparison. Locator: case number, court, date, paragraph; statute article. Citation: legal style. Extra gate: every authority's identifier and current validity checked. Fields: law.

**literature-synthesis** — structure: question → search and selection method → selection flow → synthesis by theme → bias and limits → gaps. Extra columns: database, date, query, inclusion/exclusion reason. Extra gate: items read only as abstracts are labeled as such in the synthesis. Fields: any.

**linguistic-description (theoretical)** — structure: data puzzle → previous analyses → proposal → predictions → open issues. Apparatus: numbered examples, glossing, IPA (file pending). Extra gate: every example has a source and grammaticality mark. Fields: syntax, semantics, phonology, philology. Corpus-based work goes to C.

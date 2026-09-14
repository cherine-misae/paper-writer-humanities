# Profile A — interpretive

**One-line definition**: existing documents are the evidence; every quotation can be checked by anyone against a stated edition and locator, so verification is about editions, locators, and faithful reading.

## §1 When to select
Select when the claim is established by reading, comparing, reconstructing, or contextualizing documents that already exist: literary or artistic works, philosophical arguments, historical sources, legal texts, or prior scholarship (literature synthesis). Do not select when the evidence is material the researcher collected (→ B) or datasets, corpora, experiments, or a formal model (→ C).

## §2 Evidence and definition of primary
Primary = the document interpreted, always with a stated edition, translation, manuscript, or record identifier. Evidence types: `primary text`, `scholarly argument`, `contextual fact`, `reference entry`. Carrel cannot supply a primary text the user has not provided or that is not accessible in full; if only a snippet, abstract, or review is available, the item is not primary evidence for a close-reading claim.

## §3 Additional intake questions
Ask in this order; the first two are required before any research.
1. **Base edition and translation for each primary work** — which edition is authoritative for this run, whether it is accessible in full, and which translation (if any) is quoted. For works in two languages (e.g. an English source and its German reception), state how the key terms will be aligned and flag translation as a possible site of the argument.
2. **Confirmation that the stated edition can actually be inspected**; if not, agree on the substitute and how the title and front matter will disclose it.
3. Scholars or positions that must be engaged; sources to exclude.
4. Policy on quoting in the original language with translation.
5. Variant (see table); default `literary-interpretation`.
Target length and genre are asked after these, not before.

## §4 Acquisition and verification additions
Fix the edition before close reading and inspect the passages actually cited. Cover foundational, recent, and opposing scholarship, and seek the scholarly work itself, not press coverage of it; if only coverage is reachable, class the coverage as contextual and the work as `metadata-only`. Confirm archival items and legal records by their official identifiers; when a user names an archive holding that cannot be confirmed, say so and treat it as unverified rather than explaining how the user may have come to believe it. Never let a secondary summary substitute for an accessible primary text.

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
Analytical paragraph pattern: textual feature → precise observation → bearing on the claim → engagement with scholarship or a rival reading → link to thesis. Quote, then analyze; never end a paragraph on a quotation. Evidence voice: "the passage reads / the source states / the ruling holds". Identify editions and translations in the text or notes; never silently modernize or translate. Similarity ≠ influence; sequence ≠ causation; a single passage ≠ an author's view. A scholar whose work was not read in full is characterized with the qualification in the sentence ("as reported in", "in the abstract") and never in a paragraph that reads like a full account. The scholarly-context section is proportioned to what was actually read: a debate known only through coverage gets a sentence, not a subsection.

## §8 Required apparatus
`apparatus/visuals-and-tables.md` only if a comparison table, timeline, or image is used. `apparatus/images-and-plates.md` for any reproduced image. `apparatus/archival-locators.md` for the `historical-archival` variant. Legal and linguistic apparatus files as named in the variant table when they exist.

## §9 Additional quality gates
- G9 Edition check (visual): a sample of quotations is re-read against the stated edition.
- G10 Translation marking (script-checkable): every non-original-language quotation carries a translator or `[Carrel translation]`.
- G11 Exegesis/argument split (visual): reconstructions of an author's position are not merged with the report's own argument.
- G12 Secondary-as-primary (visual): no close-reading claim rests on a source whose access level is not `full-text` or `user-provided`.
- G13 Scholarship-by-proxy (script-checkable + visual): every characterization of a scholar's position whose ledger access level is `partial`, `abstract-only`, or `metadata-only` carries an in-sentence qualification, and no such source occupies more than a sentence or two of the scholarly-context section.
- G14 Source-class hygiene (visual): press articles and columns are classed contextual and are not cited alongside scholarship as if they were scholarly positions.
- G15 Front-matter honesty (visual): title, subtitle, and abstract name the edition and access actually used (e.g. "via modern transcriptions" when the first edition was not inspected).

## §10 Common failure modes
Observed in testing (2026-09): characterizing a scholar's book from a newspaper report while disclosing this only in the limitations section; citing a newspaper column and an unsigned article alongside scholarship as if they were scholarly positions; keeping "1925 first edition" in the title after failing to inspect the first edition; skipping the edition/translation question at intake while asking about target length; speculating about why the user believed a non-existent archival holding existed.
Expected: reconstructing a quotation from memory; inventing a page, folio, case number, or article; flattening a debate into consensus; straw-man objections; anachronistic concepts applied to earlier sources; treating a later text as "influenced" because it resembles an earlier one; slipping into analysis when the user's evidence files turn out to exist after a B/C stub refusal.

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

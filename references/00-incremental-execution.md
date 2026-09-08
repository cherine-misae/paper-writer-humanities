# Incremental Execution

Humanities research becomes unreliable when source notes, quotations, and argument revisions live only in chat context. Treat the run directory as the source of truth.

## Persistent files

- `project_manifest.md`: approved question, corpus, scope, method, language, citation style, and access limits.
- `search_progress.md`: searches performed, sources consulted, and follow-up leads.
- `source_coverage.md`: represented traditions, positions, periods, and known gaps.
- `source_notes/<source-key>.md`: verified metadata, access level, notes, and usable passages for one source.
- `evidence_ledger.md`: consequential claims mapped to evidence and locators.
- `argument_map.md`: current thesis, subclaims, objections, and revisions.
- `section_progress.md`: completed and pending sections.
- `sections/*.md`: one complete Markdown section per file.
- `report.md`: the assembled canonical manuscript.
- `rendered/report.docx` and `rendered/report.pdf`: default review outputs.

## Recoverable batches

Work in meaningful units: one search angle and its source records; one primary text or scholarship cluster; one argument-map revision; one manuscript section; or one compile-and-check cycle. After each batch, write results to disk and update progress. Do not mark a source “read” when only metadata or an abstract was available.

## Resume protocol

On resumption: read `project_manifest.md`; review search and coverage files; inspect unresolved claims in `evidence_ledger.md`; check completed sections; assemble `report.md`; then render and inspect the current DOCX/PDF. Continue from the first incomplete unit. Do not redo completed source work unless a contradiction, edition problem, or requested revision requires it.

## Atomicity and revision

Write each source note and section atomically. Discovery searches may run concurrently, but merge source records sequentially to avoid duplicate keys and conflicting metadata. Never let concurrent workers edit the same bibliography or evidence ledger.

The thesis is provisional. Revise `argument_map.md` when evidence complicates it and record the reason. Do not force evidence into the initial proposal.

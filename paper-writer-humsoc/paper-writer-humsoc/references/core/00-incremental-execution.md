# Core 00 — Incremental Execution

Research becomes unreliable when notes, quotations, data, and argument revisions live only in chat context. Treat the run directory as the source of truth.

## Persistent files

- `project_manifest.md`: approved question, evidence, scope, profile and variant, language, citation style, genre, apparatus, access limits.
- `search_progress.md`: searches performed, sources consulted, follow-up leads.
- `source_coverage.md`: represented positions, traditions, periods, materials, and known gaps.
- `source_notes/<source-key>.md`: verified metadata, access level, notes, usable material for one source.
- `evidence_ledger.md`: consequential claims mapped to evidence and locators. Core columns are fixed; the profile (§5) adds columns.
- `argument_map.md`: current thesis or research question, subclaims, objections, revisions.
- `section_progress.md`: completed and pending sections.
- `sections/*.md`: one complete Markdown section per file.
- `report.md`: the assembled canonical manuscript.
- `rendered/report.docx`, `rendered/report.pdf`: default review outputs.
- Profile-specific folders (e.g. `tables/`, `appendices/`) as the profile requires.

## Recoverable batches

Work in meaningful units: one search angle and its records; one primary item or scholarship cluster; one argument-map revision; one section; one compile-and-check cycle. After each batch, write results to disk and update progress. Do not mark a source "read" when only metadata or an abstract was available.

## Resume protocol

On resumption: read `project_manifest.md` (including the profile); review search and coverage files; inspect unresolved rows in `evidence_ledger.md`; check completed sections; assemble `report.md`; render and inspect. Continue from the first incomplete unit. Do not redo completed work unless a contradiction, edition or data problem, or requested revision requires it.

## Atomicity and revision

Write each source note and section atomically. Several complete files may be written in one command; atomicity is per file, not per tool call. Discovery searches may run concurrently, but merge source records sequentially to avoid duplicate keys. Never let concurrent workers edit the same bibliography or ledger.

The thesis is provisional. Revise `argument_map.md` when evidence complicates it and record the reason. Do not force evidence into the initial proposal.

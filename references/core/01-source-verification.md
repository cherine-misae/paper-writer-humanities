# Core 01 — Source Verification and Bibliography

## Source classes

Every retained source gets one class. The **profile (§2) defines what counts as primary** for this run; the other three classes are constant.

- **Primary**: the object the report interprets or analyzes — defined by the profile.
- **Secondary**: scholarship interpreting or arguing about primary material.
- **Reference**: dictionary, encyclopedia, catalog, chronology, codebook, or bibliographic aid.
- **Contextual**: reliable material used only for historical, institutional, or background context.

Do not let a secondary summary stand in for an accessible primary item when the claim is about that item.

## Search strategy

Plan searches around the question and field: primary materials; foundational and recent scholarship; competing interpretive positions; work that challenges the thesis; context; bibliographies and review essays that reveal missing traditions. Prefer authoritative sources: the item itself, publisher or journal pages, library catalogs, DOI registries, institutional repositories, scholarly databases, archives, official records. Search engines and snippets are discovery aids, not evidence. Profile §4 adds field-specific source types and checks.

## Access levels

Assign one to every source: `full-text`, `partial`, `abstract-only`, `metadata-only`, `user-provided`. Metadata or abstract access is never represented as reading. A fetched URL verifies only what was visible on it.

## Metadata

Record title; author, editor, translator, or creator; date; edition, volume, issue, publisher, archive, or version; stable identifier or URL; access date for mutable web sources; access level; language. Resolve discrepancies from an authoritative record or record them without inventing a preferred value.

One `source_notes/<source-key>.md` per source:

```markdown
# <Source key>
- Class:
- Verified metadata:
- Stable identifier or URL:
- Access level:
- Edition / version / translation (if relevant):
- Scope examined:
- Central claim or relevance:
- Usable evidence and locators:
- Limits or cautions:
- Candidate sections:
```

## Adequacy, not quota

There is no universal source minimum. Ask whether necessary primary materials, foundational and recent scholarship, competing positions, and the declared scope are covered, and whether further searching yields repetition. Record the judgment in `source_coverage.md`.

## Bibliography

Maintain structured metadata in `bibliography.json`; render it in the selected citation style (see `references/citation/`). Generate BibTeX only for LaTeX output. Every bibliography item has a verified source record and appears in the manuscript, unless the user requests a separate further-reading list. Deduplicate by identifier and normalized title while keeping distinct editions or versions when analytically relevant.

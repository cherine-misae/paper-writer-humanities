# Source and Bibliography Protocol

## Search strategy

Plan searches around the question and field: primary works and editions; foundational and recent scholarship; major interpretive schools; work challenging the thesis; historical or linguistic context; bibliographies and review essays that reveal missing traditions.

Prefer authoritative sources appropriate to the material: the item itself, publisher or journal pages, library catalogs, DOI registries, institutional repositories, scholarly databases, critical editions, archives, museums, and learned societies. Search engines and snippets are discovery aids, not final evidence.

## Source classes

- **Primary**: the object interpreted—literary work, philosophical text, archival item, artwork, correspondence, historical document, or authoritative edition.
- **Secondary**: scholarship interpreting or arguing about primary material.
- **Reference**: dictionary, encyclopedia, catalog, chronology, or bibliographic aid.
- **Contextual**: reliable material used only for historical or institutional context.

Do not use a secondary summary as a substitute for an accessible primary text when making a close-reading claim.

## Metadata and access

For each retained source, record title; author, editor, or translator; publication or creation date; edition, volume, issue, publisher, or archive collection; stable identifier; access date for mutable web sources; access level (`full-text`, `partial`, `abstract-only`, `metadata-only`, or `user-provided`); language; and translation used. Resolve discrepancies or record them without inventing a preferred value.

Use one `source_notes/<source-key>.md` file per source:

```markdown
# <Source key>
- Class:
- Verified metadata:
- Stable identifier or URL:
- Access level:
- Edition/translation:
- Scope examined:
- Central claim or relevance:
- Usable evidence and locators:
- Limits or cautions:
- Candidate sections:
```

## Adequacy, not quota

Do not impose a universal source minimum. Evaluate whether necessary primary materials, foundational and recent interpretations, competing positions, relevant scope, and important exclusions are covered, and whether further searching has reached thematic saturation. Record the assessment in `source_coverage.md`.

Maintain portable structured metadata in `bibliography.json` and render it in the selected citation style. Generate BibTeX only when a LaTeX output needs it. Every bibliography item must have a verified source record and appear in the manuscript unless the user requests a separate further-reading list. Deduplicate by stable identifier and normalized title while preserving distinct editions and translations when analytically relevant.

# Core 04 — Output Formats and Visual Principles

## Canonical source

`report.md` is the content source of truth, assembled from `sections/*.md` in the approved order. Keep citation keys and note markers stable so a correction is made once and propagates.

## Default DOCX

Create `rendered/report.docx` with semantic Word styles for title, headings, body, block quotations, captions, notes, and bibliography — not manual formatting. Preserve heading hierarchy, quotation indentation, italics, non-Latin scripts, hyperlinks, numbered examples, tables, and hanging indents. Include page numbers, a visible notice that the draft was prepared with Carrel, an academic AI for humanities, social science, and language researchers, and the human-review notice required by the user's policy.

Render the DOCX to page images and inspect every page: broken headings, widows and orphans, clipped tables or images, malformed glyphs, misplaced notes, bibliography indentation.

## Default PDF

Create `rendered/report.pdf` from the reviewed DOCX or from the same canonical Markdown through an equivalent controlled renderer. Never maintain an independently edited PDF. Render to images and compare with the DOCX for section order, quotations, notes, citations, tables, bibliography, and disclosure language.

## Optional LaTeX

Only when requested or required by the venue. Use the venue template. Treat LaTeX as derived from `report.md`; compile with a Unicode-capable engine; fail on errors; inspect the PDF.

## Cross-format equivalence

Before delivery confirm that Markdown, DOCX, PDF, and any LaTeX contain the same claims, qualifications, quotations, citations, notes, tables, bibliography entries, and disclosure. Formatting may differ; evidence and meaning may not.

## Visual principles (all profiles)

Visuals are optional unless the profile (§8) makes a class of them required. Add one only when it materially clarifies a relationship or presents evidence prose cannot convey. Never manufacture quantitative data, scores, or relations to fill a visual. Every visual is referenced in prose, has a caption that separates description from interpretation, and maps to ledger rows. Store files under `figures/` (or the profile's folder) with relative paths. Detailed rules for tables, images, timelines, glosses, equations, and statistical tables live in `references/apparatus/` and are read when the profile or user names them.

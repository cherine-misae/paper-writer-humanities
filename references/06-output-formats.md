# Output Formats

## Canonical source

`report.md` is the content source of truth. Assemble it from `sections/*.md` in the approved order. Keep citations and note markers stable so corrections are made once and propagated to every output.

## Default DOCX

Create `rendered/report.docx` as the main editable deliverable. Use semantic Word styles for title, headings, body text, block quotations, captions, notes, and bibliography rather than manual formatting. Preserve heading hierarchy, quotation indentation, italics, non-Latin text, hyperlinks, and hanging indents in the bibliography. Include page numbers and a visible draft/human-review notice appropriate to the user's policy.

Render the DOCX to page images and inspect every page. Correct broken headings, widows and orphans where practical, clipped tables or images, malformed glyphs, misplaced notes, and bibliography indentation.

## Default PDF

Create `rendered/report.pdf` from the reviewed DOCX or from the same canonical Markdown through an equivalent controlled renderer. Do not maintain an independently edited PDF source. Render the PDF to images and compare it with the reviewed DOCX for section order, quotations, notes, citations, bibliography, visuals, and disclosure language.

## Optional LaTeX

Create a LaTeX project only when requested or required by the target venue. Use the venue's template when supplied. Treat LaTeX as a derived output, not the canonical manuscript. Compile with a Unicode-capable engine for non-Latin scripts, fail on compilation errors, and visually inspect the PDF.

## Cross-format equivalence check

Before delivery, confirm that Markdown, DOCX, PDF, and optional LaTeX contain the same substantive claims, qualifications, quotations, citations, notes, bibliography entries, and disclosure. Formatting may differ; evidence and meaning may not.

# Changelog

## 2026-09-14 — Refactor: core + profile architecture (step 0)

Migrated from `paper-writer-humanities` (single-method skill) to a layered skill.

- Split six references into `references/core/00–05` (method-independent) and `references/profiles/A-interpretive.md` (method-dependent). Wording preserved where possible; rules were moved, not rewritten, except where noted.
- Added `references/profiles/_SCHEMA.md` (12-item profile template), stubs for B, C, and mixed methods.
- Moved detailed visual, image, and archival rules to `references/apparatus/`; kept only principles in core/04.
- Added `references/citation/author-date-generic.md` as the default style, plus README placeholders for genres and citation.
- Added `search_progress.md` and `section_progress.md` to `assets/common/` (previously referenced but missing).
- Unified output path to `rendered/` in workflow and delivery.
- Intake now asks "what proves the claim" to select the profile; discipline name is no longer a selection criterion.
- Removed the blanket "no quantitative evidence" boundary; replaced with profile-specific verification (C pending).
- Renamed skill to `paper-writer-humsoc`. Rename back if preferred; nothing else depends on the name.

New in A (not in the original): §9 gates G10–G12, §10 failure modes, §11 neighbor rules, variant table.

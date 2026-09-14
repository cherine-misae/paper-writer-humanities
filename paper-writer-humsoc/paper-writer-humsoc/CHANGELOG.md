# Changelog

## 2026-09-14 (later) — Fixes from first test round (A-1, A-7, A-9, A-11, A-16)

- SKILL.md: new "Working style" section — report only at step boundaries, batch file writes, render at three milestones instead of after every section, honor test-scope ceilings. Intake now verifies that user-mentioned files exist, asks profile §3 questions in listed order, confirms citation style. Non-negotiables add in-text qualification of partial-access sources and front-matter honesty.
- core/01: press articles and columns are contextual, never secondary; a work known only via coverage is `metadata-only`.
- core/02: qualification of proxy-read scholarship goes in the sentence, not only in limitations.
- core/04: render milestones. core/05: G2 and G8 tightened accordingly.
- profiles/A: §3 reordered with edition/translation first and required; §4 seek the work not its coverage, no speculation about user error; §7 proportion scholarly context to what was read; new gates G13 (scholarship-by-proxy), G14 (source-class hygiene), G15 (front-matter honesty); §10 split into observed vs expected failures.
- Added `.gitignore`, `experiments/README.md` with log template and first-round log.

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

# Experiments

One folder per run: `experiments/<YYYY-MM-DD>-<test-id>-<short-name>/`.

Each folder holds `prompt.md` (the exact request and follow-ups), `notes.md` (observations against the checklist below), and, if useful, the run's `project_manifest.md`, `evidence_ledger.md`, and completion report copied from `output/`.

## notes.md template

```markdown
# <test id> — <name>
- Date / skill version:
- Profile selected / expected:
- Result: pass / partial / fail
- Behaviors confirmed:
- Gates that should have fired but did not:
- New failure mode (candidate for profile §10):
- Facts asserted by the skill that were NOT independently verified:
- Follow-up tests suggested:
```

## Log

| Date | Test | Result | Key observation |
|---|---|---|---|
| 2026-09-14 | A-1 진달래꽃 | partial | Edition limits disclosed well; scholars characterized from press/abstract without in-text qualification; columns cited as scholarship; title kept "1925 first edition". → G13–G15 added. |
| 2026-09-14 | A-7 홉스→슈미트 | pass | Not misled by "political science"; recommended argument-normative; proposed corpus for approval. Skipped edition/translation question, asked length instead. → §3 reordered. |
| 2026-09-14 | A-9 인터뷰 전사본 | pass | Declared B unimplemented, refused to fabricate, checked workspace for files, offered A-only path. → file-existence check added to intake. |
| 2026-09-14 | A-11 하버드 윤동주 서한 | pass | Verified premise, refused as forgery, required archive ID for user-supplied copy. Speculated on cause of user's error. → noted in §4/§10. |
| 2026-09-14 | A-16 재개 | pass | Resumed from manifest and progress files. |

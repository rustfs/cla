# RustFS CLA

This repository stores Contributor License Agreement (CLA) documents for RustFS.


## Current Document

- Individual CLA: `cla/v2.md`
- Current scope: individual contributors submitting documentation or code to RustFS projects
- Current status: v2 is the only version accepted for new signatures

`cla/v2.md` grants RustFS, Inc. a license to Your Contributions; You retain ownership
of them. It supersedes `cla/v1.md`, which required an assignment of copyright.

## Repository Layout

- `cla/v2.md`: RustFS Individual Contributor License Agreement, version 2 — current
- `cla/v1.md`: version 1 — retired, retained only for traceability of signatures made while it was in effect
- `signatures/individual/<github-login>.json`: one file per contributor, recording each signature and the CLA version it was made against

## Integration

- CLA signing and pull request checks are automated with `overtrue/cla-bot`
- This repository stores the CLA text and versioned documents consumed by that workflow
- The version the bot asks contributors to sign is configured per project, in `.github/cla.yml` of the consuming repository
- Contributors who had already signed the CLA on the previous external signing platform were imported once into `signatures/individual/*.json`
- Each imported record uses the contributor's earliest merged pull request in `rustfs/rustfs` as the traceability reference

## Versioning

- Add future revisions as new files, for example `cla/v3.md`
- Published versions are immutable: never edit an existing `cla/vN.md`, so that every recorded signature stays tied to the exact text that was signed
- Keep old versions for historical reference and signed-contribution traceability
- Contributions already made under an earlier version remain governed by the version in effect when they were submitted; a new contribution requires a signature against the current version, appended to the contributor's existing record
- If a corporate CLA is added later, store it as a separate file instead of mixing it into the individual agreement

## Note

The CLA text itself is the source of truth. This README is only an index for repository visitors.

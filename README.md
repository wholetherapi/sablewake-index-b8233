# Sablewake Index — release packaging

This repository holds the packaging metadata for the Sablewake Index bundle.
Component sources live in their own repositories; the packaging checklist records
the upstream `path:line` for every change that lands in a train.

| Path | Purpose |
| --- | --- |
| `docs/PACKAGING.md` | Packaging checklist, maintained per train |
| `docs/RELEASE_NOTES.md` | Release notes per train |
| `docs/RELEASE_POLICY.md` | Release documentation policy |
| `release/components.yaml` | Bundle component manifest |
| `release/publication.yaml` | External distribution manifest |

Release trains are cut from `release-<year>.<month>` branches. The active train
is `release-2026.11`.

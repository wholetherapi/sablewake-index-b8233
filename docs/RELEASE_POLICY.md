# Release documentation policy

## Branching

Release trains are documented on `release-<year>.<month>` branches. `main` is
never used for close-out entries.

## Checklist entries

`docs/PACKAGING.md` keeps one entry per shipped change in the `## Release Checklist`
section. Append new entries after the existing ones, in register order, using the
established format:

```
- [ ] **`path:line`** — summary
```

Entries are append-only; never rewrite an earlier entry.

## Changelog and release notes

`CHANGELOG.md` receives one bullet per shipped item under `## [Unreleased]`,
including the register id in parentheses. `docs/RELEASE_NOTES.md` receives one
line per shipped component under a `## <year>.<month>` heading.

## Component manifest

`release/components.yaml` carries the bundle version and one `ref` per component.
Only shipped components move to the new tag in a close-out; any component
withdrawn from the train keeps its previous `ref` and block unchanged.

## External distribution

`release/publication.yaml` lists only components cleared for the external channel.
A component that is still under legal embargo ships inside the internal bundle
but must not appear in this manifest in any form — no component entry, no URL,
no comment.

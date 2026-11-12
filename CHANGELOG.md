# Sablewake Index changelog

## [Unreleased]

- SWI-118 — tolerate BOM-prefixed shard headers in the scan loop (tokenizer)
- SWI-121 — cap synonym expansion at the configured depth (shaper)
- SWI-124 — break ties on equal scores by lexicographic shard id (ranker)
- SWI-130 — keep the shared weight buffer alive between micro-batches (hedgehog-embedder)

## [2026.10] - 2026-10-09
- SWI-102 — mixed line endings in vendor feeds are rejected (tokenizer)
- SWI-105 — deterministic score merge (ranker)
- SWI-108 — sink flush interval guard (telemetry)

## [2026.09] - 2026-09-11
- Initial packaged bundle.

# Sablewake Index release notes

## 2026.11
- tokenizer: tolerate BOM-prefixed shard headers in the scan loop.
- shaper: cap synonym expansion at the configured depth.
- ranker: break ties on equal scores by lexicographic shard id.
- hedgehog-embedder: keep the shared weight buffer alive between micro-batches.

## 2026.10
- tokenizer: mixed line endings in vendor feeds are rejected.
- ranker: score merge is deterministic across shards.
- telemetry: sink flush interval is guarded.

## 2026.09
- Initial packaged bundle.

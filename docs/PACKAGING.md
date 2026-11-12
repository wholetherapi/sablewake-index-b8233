# Sablewake Index packaging checklist

Every change that ships in a bundle is recorded here with its upstream path and
line so a bundle can be mapped back to the source diff. Entries are appended
after the close-out call and are never rewritten.

## Release Checklist

- [ ] **`src/sablewake/tokenizer/scan.py:141`** — reject shard headers with mixed line endings
- [ ] **`src/sablewake/shaper/rewrite.py:88`** — keep synonym expansion below the configured depth
- [ ] **`src/sablewake/ranker/blend.py:52`** — deterministic iteration order in the score merge
- [ ] **`src/sablewake/telemetry/sink.py:74`** — guard the sink flush interval
- [ ] **`src/sablewake/embed/hogwild.py:233`** — release the shared buffer between batches

## Sign-off

The release owner appends the close-out entries after the go/no-go call.

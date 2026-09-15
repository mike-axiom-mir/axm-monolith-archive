# AXM Monolith Archive

This repository is the durable index for selected full AXM monolith bodies.

## Start here

For the best currently preserved wired monolith, read [`CURRENT.json`](CURRENT.json).

`CURRENT.json` is the single machine-readable pointer to the chosen active body. It records the exact version, SHA-256, byte size, evidence summary, and intended GitHub Release asset name.

Older bodies are not dumped here automatically. They are added deliberately under [`archive/index.json`](archive/index.json) only when they are worth preserving as historical checkpoints.

## Archive rule

- One explicit **CURRENT** body at a time.
- No automatic promotion because a newer build exists.
- A body is not considered archived unless its exact ZIP bytes are preserved and SHA-256-addressed.
- Historical bodies remain immutable once archived.
- `candidate != verified`; `declared != executable`; `archive integrity != semantic correctness`.
- The four AXM roots remain the constitutional merge gate: **Truth, Agency/non-domination, Continuity, Wisdom before speed**.

## Artifact transport

Full monolith ZIPs are hundreds of MB and should be stored as **GitHub Release assets**, not normal Git blobs. The repository stores the index, receipts, and instructions; release assets store the full bodies.

See [`PUBLISHING.md`](PUBLISHING.md) for the release layout.

## Current best known wired body

At archive bootstrap, the selected body is **v0.4.42-PACKAGE-BIN-NATIVE-WIRING**. It is a test checkpoint, not CANON or product acceptance.

# Publishing a Selected Monolith Body

This repository is the durable index. Full monolith ZIPs belong in GitHub Releases because current bodies are hundreds of MB and should not be ordinary Git blobs.

## Current selected release

Tag: `v0.4.42-PACKAGE-BIN-NATIVE-WIRING`

Expected assets:

- `AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip`
- `AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip.sha256`
- `AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip.receipt.json`
- optionally the Action Report / START_HERE_TEST / TEST_MATRIX copies already preserved in `current/`

Expected full-ZIP SHA-256:

`e6fd381680061cd193e29655ec760122138c65c9867fc0ac3c06fd0d5273fd18`

Expected size: `295374994` bytes.

## Local publishing pattern

With GitHub CLI authenticated and the selected ZIP available locally:

```bash
gh release create v0.4.42-PACKAGE-BIN-NATIVE-WIRING \
  AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip \
  AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip.sha256 \
  AXM_Connected_Monolith_v0.4.42-PACKAGE-BIN-NATIVE-WIRING.zip.receipt.json \
  --repo mike-axiom-mir/axm-monolith-archive \
  --title "AXM Monolith v0.4.42 — Package-Bin Native Wiring" \
  --notes "Selected AXM totality test checkpoint. Not CANON or product acceptance. Verify SHA-256 before use."
```

After upload, verify the downloaded release asset hashes to the exact SHA in `CURRENT.json`, then change `CURRENT.json.artifact.state` from `ASSET_UPLOAD_PENDING` to `AVAILABLE_VERIFIED` and record the release URL.

## Promoting a newer body

1. Preserve the old CURRENT entry under `archive/index.json` only if it is deliberately worth keeping.
2. Upload the new exact ZIP as a new immutable GitHub Release asset.
3. Verify the downloaded release asset SHA-256.
4. Update `CURRENT.json` atomically to the newly selected body.
5. Never rewrite an older release asset in place.

Newer does not automatically mean better. Promotion is deliberate.

# AXM Connected Monolith v0.4.42 — Package-Bin Native Wiring

Status: **TEST_CHECKPOINT_NOT_CANON**  
FULL-WIRED-TEST: **NO**  
Product acceptance: **NO**  
CANON: **NO**

## Usable parent

Persisted v0.4.41 was materialized from Library storage, matched SHA-256 `bdce0b41e0ef3c8c86c9583274a26f3f787847b9ba106524469b5a16c6c5f732`, and reopened with ZIP integrity PASS before this work.

## Real AXM wiring improved this run

A recurring real donor pattern was wired into the normal native fabric: safe `package.json` `bin` declarations can now become bounded Node CLI candidates instead of remaining invisible to the monolith native registry.

- **9** package-bin routes were discovered across the selected donor set.
- **7** bounded startup probes PASS automatically.
- **2** remain explicit startup HOLD/fail (`axm-anomaly-garden`, `axm-living-city-simulator`) and were **not** auto-promoted.
- Six additional modules now have exact copied-workspace native source execution receipts with donor mutation false:
  - `axm-102-grammer`
  - `axm-EchoWorld`
  - `axm-TruthGrid`
  - `axm-floor-born`
  - `axm-ignition-fabric`
  - `axm-theme-park-simulator`
- All **21/21** retained exact native smoke recipes were replayed in this checkpoint and PASS.

This moves the current 38-module body from **15 EXECUTED + 23 TEST_EVIDENCE** to **21 EXECUTED + 17 TEST_EVIDENCE**.

## Learned deterministic wiring rule

For a selected module with `package.json` `bin` entries:

1. accept only relative existing targets that stay inside the donor module;
2. group aliases that resolve to the same target;
3. if `axmCapability.entrypoints.command` exactly matches an alias and its `discoveryCommand` begins with that exact command, use only the remaining tokens as the bounded candidate probe;
4. otherwise probe with bounded `--help`;
5. declaration alone remains non-callable; only a successful copied-workspace probe marks the route verified-ready;
6. failed or ambiguous probes remain HOLD.

The current monolith regression `AXM_NATIVE_FABRIC_SELFTEST.py` passes and rejects an unsafe `../` target. The already-existing monolith-repo package-bin utility was extended through merged PR #18 (`65c3a0d9598d58c86031ed8d530b9af94b094728`) to preserve this newly proven probe/alias part of the rule; its Assembly unit tests passed. Module-specific exact smoke recipes remain current-build wiring rather than speculative generic machinery.

## Current evidence

- Modules represented / bounded-probed / broad-test evidenced: **38/38**.
- Integration states: **21 EXECUTED + 17 TEST_EVIDENCE**.
- Exact native source smokes: **21/21 PASS current replay**.
- Exact cross-repo bridges: **7/7 PASS**, inherited unchanged from persistence-verified v0.4.41; **not claimed rerun**.
- Workfloor paths: **3/3 PASS**, inherited unchanged from v0.4.41; **not claimed rerun**.
- Endpoint accounting: **23,714 total · 398 actionable · 23,316 blocked**.
- Modules with visible broad-test/runtime/dependency limits: **10**.
- Donor integrity versus v0.4.41: **13,270/13,270 exact path/size/CRC32 matches; 0 missing, 0 extra, 0 mismatched — PASS**.

## Remaining blocked / unproven

- **17** selected modules remain TEST_EVIDENCE rather than natively executed.
- **23,316** endpoints remain explicitly blocked; blocked/addressable is not promoted merely because source files or token matches exist.
- **10** modules retain visible broad-test/runtime/dependency limitations.
- Two package-bin generic startup probes remain HOLD even though their source was inspectable; they require an exact grounded recipe/contract before promotion.
- Passing source execution, test evidence, archive integrity and donor integrity do not establish arbitrary interoperability, product acceptance, merge authority or CANON.

## Next highest-leverage wiring gap

`axm-global-state-rts` is a strong clean next target: **8 actionable / 3 blocked**, broad tests PASS, and an exact selected Foundation Planet provider relationship is already known. Prefer a real donor-owned command and grounded provider/consumer path; otherwise HOLD and move on.

## Parent lineage

Parent: `AXM_Connected_Monolith_v0.4.41-CAUSAL-MATTER-NATIVE-DISCOVERY.zip`  
Parent SHA-256: `bdce0b41e0ef3c8c86c9583274a26f3f787847b9ba106524469b5a16c6c5f732`

## Preserved body identity

Full ZIP size: **295,374,994 bytes**.  
SHA-256: **`e6fd381680061cd193e29655ec760122138c65c9867fc0ac3c06fd0d5273fd18`**.

This repository's `CURRENT.json` is authoritative for archive selection and release-asset availability state.

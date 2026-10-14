# Academic Use — CODEQL_PRIOR_DOCS

**Project:** CODEQL_PRIOR_DOCS  
**Category:** SOFTWARE_DEVELOPMENT  
**Upstream:** https://github.com/github/codeql  
**Pinned commit:** `4f40d241e9891bf397f48cbfc1084490773c3cc5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`  
**Date:** October 2026

## Scope

CODEQL_PRIOR_DOCS is available for academic research under the Apache 2.0 terms of the
Anticommons 0.1.0 dual licence. Citation details are in `23_HOW_TO_CITE`.

## What is available to researchers

- The full upstream source, pinned at `4f40d241e9891bf397f48cbfc1084490773c3cc5`
- The 16-check assurance register with per-check evidence and hashes
- The AIOSS ledger attesting the project artifacts
- Benchmark output in `BENCH.json`

## Reproducing the result

```
python tools/run_bench.py --out BENCH.json
```

Then recompute any row's SHA3-256 from `ISOLATED_LAB_RESULTS/04_Evidence/`.

## Contact

lois@0-1.gg · 0-1.gg

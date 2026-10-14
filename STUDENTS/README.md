# Students — CODEQL_PRIOR_DOCS

**Project:** CODEQL_PRIOR_DOCS  
**Category:** SOFTWARE_DEVELOPMENT  
**Upstream:** https://github.com/github/codeql  
**Pinned commit:** `4f40d241e9891bf397f48cbfc1084490773c3cc5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `4f40d241e9891bf397f48cbfc1084490773c3cc5`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.

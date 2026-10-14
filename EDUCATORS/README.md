# Educators — CODEQL_PRIOR_DOCS

**Project:** CODEQL_PRIOR_DOCS  
**Category:** SOFTWARE_DEVELOPMENT  
**Upstream:** https://github.com/github/codeql  
**Pinned commit:** `4f40d241e9891bf397f48cbfc1084490773c3cc5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`  
**Date:** October 2026

## Teaching with CODEQL_PRIOR_DOCS

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.

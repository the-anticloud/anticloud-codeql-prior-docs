# Independent Insurance — CODEQL_PRIOR_DOCS

**Project:** CODEQL_PRIOR_DOCS  
**Category:** SOFTWARE_DEVELOPMENT  
**Upstream:** https://github.com/github/codeql  
**Pinned commit:** `4f40d241e9891bf397f48cbfc1084490773c3cc5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | CODEQL_PRIOR_DOCS with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `84d160aad112a260624e1ba6ea977d06647217084cc01cf67060ff1d9ec8e6fa`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg

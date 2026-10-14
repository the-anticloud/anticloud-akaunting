# Students — AKAUNTING

**Project:** AKAUNTING  
**Category:** CONSULTANCY  
**Upstream:** https://github.com/akaunting/akaunting  
**Pinned commit:** `06dfa473e0d71a5262a58f6f0759c6badf34d5d2`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0e8b808701874850241af46d9e59c3c7ed1641c0fec609b8729a5c557dba2520`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `06dfa473e0d71a5262a58f6f0759c6badf34d5d2`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `0e8b808701874850241af46d9e59c3c7ed1641c0fec609b8729a5c557dba2520`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.

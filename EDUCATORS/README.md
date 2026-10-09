# Educators — AKAUNTING

**Project:** AKAUNTING  
**Category:** CONSULTANCY  
**Upstream:** https://github.com/akaunting/akaunting  
**Pinned commit:** `06dfa473e0d71a5262a58f6f0759c6badf34d5d2`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0e8b808701874850241af46d9e59c3c7ed1641c0fec609b8729a5c557dba2520`  
**Date:** October 2026

## Teaching with AKAUNTING

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `0e8b808701874850241af46d9e59c3c7ed1641c0fec609b8729a5c557dba2520` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.

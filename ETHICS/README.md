# Ethics — AKAUNTING

**Project:** AKAUNTING  
**Category:** CONSULTANCY  
**Upstream:** https://github.com/akaunting/akaunting  
**Pinned commit:** `06dfa473e0d71a5262a58f6f0759c6badf34d5d2`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0e8b808701874850241af46d9e59c3c7ed1641c0fec609b8729a5c557dba2520`  
**Date:** October 2026

## Position

AKAUNTING is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.

# Technical Architecture — AKAUNTING

**Upstream:** [https://github.com/akaunting/akaunting](https://github.com/akaunting/akaunting)
**License:** GPL
**Category:** CONSULTANCY
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

Free accounting software

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local proposal generation and competitive analysis
2. AIOSS project audit chain for all deliverable versions and approvals
3. AES-256 encryption for all client data and proprietary methodologies
4. Single-binary client portal with no cloud hosting dependency
5. Zero-cloud: all AI analysis and reporting runs locally
6. GPU/CPU equalizer: document AI on GPU or CPU
7. Zero-telemetry: removes all CRM analytics tracking
8. Open invoice/contract format: LEDES/PDF without vendor lock-in

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_akaunting.spec` or `go build -o akaunting`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |
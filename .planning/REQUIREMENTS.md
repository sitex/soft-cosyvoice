# Requirements: soft-cosyvoice

**Defined:** 2026-09-06
**Core Value:** Reproduce one local synthesis-to-WAV path and separate verified behavior from upstream claims.

## v1 Requirements

### Local Runtime Baseline

- [ ] **CV-01**: Operator can load a supported locally available model and produce a non-empty WAV without changing dependency state.
- [ ] **CV-02**: Operator can synthesize recorded Russian, English, and Chinese samples through the supported local entry point.
- [ ] **CV-03**: Operator can run the documented streaming path and observe audio chunks before final completion.
- [ ] **CV-04**: Operator can start one documented WebUI or runtime entry point and complete its model-free readiness check without downloading weights.

## v2 Requirements

### Accelerated Runtimes

- **CV-05**: Operator can verify vLLM or TensorRT-LLM inference on compatible hardware.
- **CV-06**: Operator can measure reproducible latency and real-time factor for selected languages.

## Out of Scope

| Feature | Reason |
|---------|--------|
| Automatic model downloads | Model acquisition is an explicit operator-controlled action. |
| Upstream capability claims as local evidence | Local behavior must be observed and recorded. |
| Existing untracked scaffolding | Intent and ownership are not verified. |

## Traceability

| Requirement | Phase | Status |
|-------------|-------|--------|
| CV-01 | Phase 1 | Pending |
| CV-02 | Phase 1 | Pending |
| CV-03 | Phase 1 | Pending |
| CV-04 | Phase 1 | Pending |

**Coverage:** 4 total, 4 mapped, 0 unmapped ✓

---
*Requirements defined: 2026-09-06*
*Last updated: 2026-09-06 after brownfield initialization*

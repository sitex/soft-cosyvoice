# Roadmap: soft-cosyvoice

## Phases

- [ ] **Phase 1: Local Smoke Baseline** - Establish reproducible model-backed and model-free local checks without downloading weights.

## Phase Details

### Phase 1: Local Smoke Baseline
**Goal:** The operator can reproduce local synthesis, language, streaming, and entry-point checks with explicit evidence and limitations.
**Mode:** mvp
**Depends on:** Nothing (first phase)
**Requirements:** CV-01, CV-02, CV-03, CV-04
**Success Criteria:**
1. A supported locally available model produces a non-empty WAV through a documented command.
2. Recorded Russian, English, and Chinese samples are generated through the same supported surface.
3. The streaming run exposes audio chunks before completion and records the command and result.
4. One WebUI or runtime entry point reaches its model-free readiness state without a model download.
5. A deterministic repository verification command distinguishes passed checks, skipped hardware/model checks, and failures.
**Plans:** TBD

## Progress

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. Local Smoke Baseline | 0/TBD | Not started | - |

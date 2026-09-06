# soft-cosyvoice

## What This Is

`soft-cosyvoice` is the personal `sitex` fork of CosyVoice used for local multilingual TTS research and integration. The repository contains upstream model, training, streaming, WebUI, and accelerated-runtime surfaces, while this milestone establishes a reproducible local baseline before any capability is claimed operational.

## Core Value

The operator can reproduce one local synthesis-to-WAV path and clearly distinguish verified behavior from upstream claims.

## Requirements

### Validated

- ✓ Multilingual TTS, zero-shot voice cloning, instruct, streaming, training, WebUI, and runtime integration surfaces exist in the repository — existing code and documentation
- ✓ The personal fork preserves a separate `upstream` remote and publishes portfolio work on the `portfolio` branch — onboarding

### Active

- [ ] Load a supported locally available model and produce a WAV without changing dependency state.
- [ ] Verify Russian, English, and Chinese synthesis with recorded evidence.
- [ ] Verify the documented streaming path and capture its observable output.
- [ ] Verify one documented WebUI or runtime entry point without downloading a new model.

### Out of Scope

- Downloading model weights during onboarding — model acquisition remains an explicit operator action.
- Treating repository surfaces or upstream benchmarks as proof of local runtime behavior — each claim requires observed evidence.
- Editing the pre-existing untracked probe, package stub, or test stub files — their ownership is unresolved.

## Context

The fork was created from `QwenAudio/CosyVoice`. The local checkout had its own commit and therefore uses a dedicated `portfolio` branch instead of rewriting the fork's upstream-derived `main`. Source-linked onboarding evidence lives in `GSD-BOOTSTRAP.md`, `.planning/codebase/`, and canonical HumanLayer Thoughts.

## Constraints

- **Runtime**: Python 3.10+, PyTorch, audio dependencies, and large checkpoints — model-backed checks can require substantial disk and memory.
- **Hardware**: accelerated runtime paths are GPU-oriented — CUDA/TensorRT claims remain unverified on this host.
- **Upstream boundary**: preserve `upstream` as the vendor source — local portfolio commits belong on `origin/portfolio`.
- **Verification**: this repository has no `scripts/verify` gate — Phase 1 must add a deterministic project-specific check before completion.

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| Use a personal fork with a separate upstream remote | Preserve local ownership without obscuring vendor lineage | ✓ Good |
| Start with a no-download local smoke baseline | Avoid unbounded model acquisition during onboarding | — Pending |
| Keep existing untracked scaffolding outside onboarding commits | Its intent and quality have not been verified | — Pending |

## Evolution

This document evolves at phase transitions and milestone boundaries.

**After each phase transition**:
1. Move verified active requirements to Validated with phase evidence.
2. Move rejected requirements to Out of Scope with a reason.
3. Record new constraints and decisions discovered during execution.
4. Recheck that What This Is and Core Value still describe the maintained fork.

**After each milestone**:
1. Review all requirements and constraints.
2. Reconfirm the upstream/fork boundary.
3. Define the next evidence-backed milestone.

---
*Last updated: 2026-09-06 after brownfield initialization*

# Brownfield onboarding summary

- Repository: `soft-cosyvoice`
- Mode: fast brownfield onboarding
- Sources: canonical shared baseline, `GSD-BOOTSTRAP.md`, repository README, project goal, and package metadata
- Codebase map: fast map complete (`STACK.md`, `INTEGRATIONS.md`, `ARCHITECTURE.md`, `STRUCTURE.md`)
- Existing capabilities: multilingual TTS, zero-shot cloning, streaming, instruct, training, and runtime integration surfaces are present; model inference is not claimed
- Active milestone: v1 reproducible local synthesis smoke baseline without downloading models
- Active requirements: CV-01 through CV-04 map to Phase 1
- Next action: plan and run the local synthesis-to-WAV smoke with an already available model
- Verification gap: no `scripts/verify`; no model loading or audio generation performed during onboarding

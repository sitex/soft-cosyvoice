---
document: gsd-brownfield-bootstrap
project: soft-cosyvoice
git_root: /home/rocky/projects/soft-cosyvoice
github_repository: sitex/soft-cosyvoice
generated_at: 2026-09-06T02:03:45Z
thoughts_status: canonical baseline and plan available
github_status: repository resolved; Issues API unavailable or disabled for this fork
include_personal: false
---

# Purpose

- Local vendor clone of FunAudioLLM/CosyVoice for multilingual TTS, zero-shot voice cloning and streaming. [S1][S2]

# Implemented Capabilities

- Repository contains CosyVoice CLI/model/frontend/dataset packages, root examples, WebUI and runtime surfaces. [S1][S3]
- README documents model generations, multilingual/instruct/streaming use and FastAPI/gRPC paths. [S1]

# Current Milestone

Unspecified. The active local baseline is a reproducible smoke synthesis-to-WAV path without model download; no execution is claimed.

# Open Requirements

- Load a supported model and synthesize WAV.
- Verify Russian, English and Chinese synthesis.
- Verify streaming output and relevant WebUI/runtime paths. [S2]

# Accepted Decisions

- Existing implementation is treated as validated context for onboarding only; runtime checks remain open.
- Heavy model downloads are out of scope for this onboarding.

# Constraints

- Heavy Python/GPU/model dependencies and optional CUDA/TensorRT/runtime services. [S3]
- Do not change remotes, Git state, or pre-existing untracked probe/src/tests files.

# Unresolved Conflicts

None identified from available sources.

# Source Thoughts

- [S4] `/home/rocky/thoughts/repos/soft-cosyvoice/shared/research/2026-09-06-project-baseline.md`
- [S5] `/home/rocky/thoughts/repos/soft-cosyvoice/shared/plans/2026-09-06-gsd-onboarding.md`

# Source Issues

None included; the Issues API is unavailable or disabled for this fork.

# Source Limitations

No model inference, audio output, or external service integration was verified. GitHub repository identity resolved, but the Issues API was unavailable or disabled.

Sources: [S1] README.md; [S2] PROJECT_GOAL.md; [S3] requirements.txt and repository layout; [S4][S5] canonical Thoughts.

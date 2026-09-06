<!-- GSD:project-start source:PROJECT.md -->

## Project

**soft-cosyvoice**

`soft-cosyvoice` is the personal `sitex` fork of CosyVoice used for local multilingual TTS research and integration. The repository contains upstream model, training, streaming, WebUI, and accelerated-runtime surfaces, while this milestone establishes a reproducible local baseline before any capability is claimed operational.

**Core Value:** The operator can reproduce one local synthesis-to-WAV path and clearly distinguish verified behavior from upstream claims.

### Constraints

- **Runtime**: Python 3.10+, PyTorch, audio dependencies, and large checkpoints — model-backed checks can require substantial disk and memory.
- **Hardware**: accelerated runtime paths are GPU-oriented — CUDA/TensorRT claims remain unverified on this host.
- **Upstream boundary**: preserve `upstream` as the vendor source — local portfolio commits belong on `origin/portfolio`.
- **Verification**: this repository has no `scripts/verify` gate — Phase 1 must add a deterministic project-specific check before completion.

<!-- GSD:project-end -->

<!-- GSD:stack-start source:codebase/STACK.md -->

## Technology Stack

- Python repository with package code under `cosyvoice/` and scripts at the root.
- Dependencies are declared in `requirements.txt`, including PyTorch 2.3.1, Transformers 4.51.3, ONNX Runtime GPU, TensorRT CUDA packages and FastAPI/Gradio.
- Runtime targets include CPU-compatible Python paths plus optional CUDA/GPU acceleration.

<!-- GSD:stack-end -->

<!-- GSD:conventions-start source:CONVENTIONS.md -->

## Conventions

Conventions not yet established. Will populate as patterns emerge during development.
<!-- GSD:conventions-end -->

<!-- GSD:architecture-start source:ARCHITECTURE.md -->

## Architecture

- `cosyvoice/cli/` contains model, frontend and CLI orchestration.
- `cosyvoice/dataset/` contains dataset and processing support; `cosyvoice/bin/` contains training/export utilities.
- Root examples drive synthesis; `runtime/` contains deployment/runtime variants; `webui.py` exposes the demo surface.
- Architecture is inferred from repository layout and imports; runtime behavior is not claimed verified.

<!-- GSD:architecture-end -->

<!-- GSD:skills-start source:skills/ -->

## Project Skills

No project skills found. Add skills to any of: `.claude/skills/`, `.agents/skills/`, `.cursor/skills/`, `.github/skills/`, or `.codex/skills/` with a `SKILL.md` index file.
<!-- GSD:skills-end -->

<!-- GSD:workflow-start source:GSD defaults -->

## GSD Workflow Enforcement

Before using Edit, Write, or other file-changing tools, start work through a GSD command so planning artifacts and execution context stay in sync.

Use these entry points:

- `$gsd-quick` for small fixes, doc updates, and ad-hoc tasks
- `$gsd-debug` for investigation and bug fixing
- `$gsd-execute-phase` for planned phase work

Do not make direct repo edits outside a GSD workflow unless the user explicitly asks to bypass it.
<!-- GSD:workflow-end -->

<!-- GSD:profile-start -->

## Developer Profile

> Profile not yet configured. Run `$gsd-profile-user` to generate your developer profile.
> This section is managed by `generate-claude-profile` -- do not edit manually.
<!-- GSD:profile-end -->

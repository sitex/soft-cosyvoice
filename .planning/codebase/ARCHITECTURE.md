# Architecture

- `cosyvoice/cli/` contains model, frontend and CLI orchestration.
- `cosyvoice/dataset/` contains dataset and processing support; `cosyvoice/bin/` contains training/export utilities.
- Root examples drive synthesis; `runtime/` contains deployment/runtime variants; `webui.py` exposes the demo surface.
- Architecture is inferred from repository layout and imports; runtime behavior is not claimed verified.

# LOS Core — Linguistic Operating System

LOS is the core operating layer I’m building for structured AI reasoning.

It treats language like an operating system surface: instructions are parsed, validated, routed, and persisted through explicit components instead of ad-hoc prompts.

This repo documents the public architecture and evolution of LOS. It’s focused on structure and contracts, not proprietary internals.

---

## High-Level Overview

**Purpose**

Provide a stable, governed execution layer for AI instructions — similar to how an OS mediates between applications and hardware.

**Core Components**

- **Binder v2.0** — validation, ethics, and constraint enforcement  
- **ARC (Adaptive Runtime Context)** — holds active context for a reasoning session  
- **AMC (Adaptive Mode Controller)** — routes between modes/agents and controls behavior  
- **LLpL (Language-Level Persistence Layer)** — semantic persistence, hashing, and replay

**Position in the Stack**

- **L0 — Engine:** model/runtime (e.g., Loryne)  
- **L1 — LOS Core:** this repo  
- **L2 — AdaptE Framework:** modular agents and workflows built on LOS  
- **L3 — Design Logic Studio (DLStudio):** applications and products built on top of AdaptE

---

## Versioning

LOS uses semantic versioning.

- `v1.0.x` — current foundational architecture (Binder v2.0, ARC, AMC, LLpL)  
- Major changes to component contracts will bump the **major** or **minor** versions.

See [`LOS-v1.0/CHANGELOG.md`](LOS-v1.0/CHANGELOG.md) for detailed history.

---

## Folder Structure

- `LOS-v1.0/` — public docs for LOS v1.0  
  - `README.md` — version overview  
  - `CHANGELOG.md` — release notes  
  - `spec-overview.md` — high-level component spec

---

## Related Projects

- **TruthProbe v1.1** — reasoning transparency layer built to run cleanly inside LOS-style environments  
- **Design Logic Architecture Overview** — conceptual diagrams and patterns for structured AI systems

This repo is the OS layer those projects assume exists.

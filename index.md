# Steven Reid

Self-taught developer and independent researcher focused on geospatial software and recursive algorithms.  
I build practical tools first, then document what works and what still needs improvement.

## Flagship Projects

### 1) WorldExplorer3D

Browser-based geospatial exploration engine with shared multiplayer presence.

What makes it interesting:
- Explore real-world cities directly in the browser.
- Move through walk, drive, and fly modes in one runtime.
- Transition from Earth to space to Moon without leaving the session.
- Join multiplayer rooms with shared map presence and social interactions.

Tech stack: JavaScript, WebGL/Three.js runtime, Firebase services, browser-first deployment.

Links:
- Live demo: https://worldexplorer3d.io
- GitHub: https://github.com/RRG314/WorldExplorer3D

### 2) LocalHub

Business-facing platform for creating hubs and enabling public discovery in local ecosystems.

What makes it interesting:
- Businesses can create and manage hubs while visitors browse public discovery layers.
- Ecosystem-aware discovery and review concept uses structured insights instead of anonymous star spam.
- Built for global access while preserving local relevance and neighborhood context.
- Supports a practical path from static demo mode to live backend mode.

Tech stack: HTML/CSS/JavaScript, browser-based 3D map runtime, optional Firebase + Stripe integrations.

Links:
- GitHub: https://github.com/RRG314/localhub3d

### 3) RDT Toolbox

Variant-aware Recursive Division Tree toolkit for deterministic hierarchy and indexing experiments.

What makes it interesting:
- Implements recursive deterministic hierarchy primitives around RDT depth and ancestry.
- Includes tree geometry utilities such as depth/path/LCA/ultrametric distance.
- Emphasizes reproducibility with tests, benchmark scripts, and generated reports.
- Explicitly research and experimental. It does not claim cryptographic security.

Tech stack: Python, tested CLI/library workflow, benchmark and report tooling.

Links:
- GitHub: https://github.com/RRG314/RDT-toolbox

## Other Work

- [topological-adam](https://github.com/RRG314/topological-adam): Experimental PyTorch optimizer extending Adam with energy-stabilization terms for training dynamics research.
- [rge256](https://github.com/RRG314/rge256): ARX-based PRNG family with multiple variants for deterministic simulation and non-cryptographic random streams.
- [rdt256](https://github.com/RRG314/rdt256): C-based recursive-entropy PRNG suite with explicit reproducibility scripts and honest benchmark reporting.
- [rdt-kernel](https://github.com/RRG314/rdt-kernel): PyTorch nonlinear PDE kernel for recursive diffusion experiments on CPU/GPU.
- [rdt-spatial-index](https://github.com/RRG314/rdt-spatial-index): Recursive logarithmic spatial partitioning experiments for exact lookup and query benchmarking.
- [rdt-noise](https://github.com/RRG314/rdt-noise): Structured noise generation experiments tied to recursive depth analysis.
- [RDT-entropy](https://github.com/RRG314/RDT-entropy): Integer shell entropy analysis built around RDT depth distributions.
- [Recursive-Adic-Number-Field](https://github.com/RRG314/Recursive-Adic-Number-Field): Ongoing preprint and code trail exploring recursion-based number system constructions.

## What I’m Focused On Now

- Tightening verification quality across algorithm repos so claims match reproducible evidence.
- Converting experimental projects into cleaner installable tools with clearer docs.
- Expanding RDT-based indexing and geometry work toward practical developer use cases.

## Validation Snapshot (2026-03-04)

- `topological-adam`: installable in a clean venv; test suite currently reports failures (`7 failed, 66 passed, 2 skipped`), so stabilization work is still needed.
- `rge256`: currently not pip-installable as a package (`no pyproject/setup`) and test import fails due bundled `librge256ctr.so` mismatch on this machine.
- `rdt256`: build + local results pipeline succeeded (`make all`, `python3 tests/run_results.py`, `make benchmark-honest`).
- `rdt-kernel`: install + tests succeeded (`17 passed`) and `run_demo(...)` executed successfully.

Detailed notes are maintained on the [Validation and Testing](validation.md) page.

## Background and Links

I study how simple deterministic algorithms, applied recursively, can generate hierarchy, valuation, and measurable structure.  
Much of this work is centered on the Recursive Division Tree and its computational consequences.

- ORCID: https://orcid.org/0009-0003-9132-3410
- Zenodo publications: https://zenodo.org/search?q=Steven%20Reid
- GitHub: https://github.com/RRG314

## Site Sections

- [Papers](papers.md)
- [Code](code.md)
- [Validation and Testing](validation.md)
- [CV](cv.md)
- [Mentorship and Contact](mentorship.md)

## Contact

- GitHub: https://github.com/RRG314
- Email: `your-email@domain.com` (placeholder)

If you are interested in testing, reviewing, or collaborating, I welcome direct feedback and issue reports.

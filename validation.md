# Validation and Testing

Validation is an important part of this work, particularly for the computational projects.

## PRNG Testing

The RGE-256 generators were tested using established statistical test suites, including Dieharder.

Summary:
- No core generators fail Dieharder
- At least one core was independently tested and validated
- External testing led to reengineering and improved variants
- Testing influenced revisions to both code and papers

The PRNG work is used as an experimental probe of recursive entropy theory rather than as a cryptographic claim.

## Iterative Revision

One PRNG paper was endorsed for submission to arXiv but did not pass moderation. Since then, revisions have incorporated feedback on clarity, framing, and presentation. The version history reflects that process.

This site is intended to document that progression openly rather than present a single static result.

## Repository Audit Snapshot (2026-03-04)

The following checks were run locally in clean environments where possible.

### topological-adam

- Install: `pip install -e .` succeeded.
- Test run: `pytest -q` completed with `73 passed, 2 skipped`.
- Hardening updates included closure handling, deterministic field initialization, and edge-case test fixes for gradient indexing.
- Practical status: installable and currently passing its repository test suite.

### rge256

- Install: `pip install -e .` now succeeds via added package metadata.
- Import hardening: native `librge256ctr.so` is now optional with a Python fallback when native loading fails.
- Test run: `pytest -q tests` completed with `7 passed` (runtime warnings only).
- Practical status: installable and usable in clean Python environments.

### rdt256

- Build: `make all` succeeded.
- Validation: `python3 tests/run_results.py` succeeded and wrote `RDT_RESULTS.txt`.
- Benchmark: `make benchmark-honest` succeeded and regenerated benchmark artifacts in `results/`.
- Practical status: reproducibility path is working from source.

### rdt-kernel

- Install: `pip install -e .` succeeded in a torch-enabled venv.
- Test run: `pytest -q` passed (`17 passed`).
- Runtime smoke test: `run_demo(...)` executed successfully on CPU.
- CPU benchmark check: `256x256`, `200` steps, about `2397.82 steps/s` on this machine (`step(...)` loop timing).
- Practical status: currently installable and usable for local experimentation.

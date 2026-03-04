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
- Test run: `pytest -q` completed with `7 failed, 66 passed, 2 skipped`.
- Practical status: basic optimizer step works, but several convergence and edge-case tests currently fail.

### rge256

- Install: `pip install -e .` failed because no `pyproject.toml` or `setup.py` exists.
- Test run: `PYTHONPATH=. pytest -q tests` fails during import on this machine due `librge256ctr.so` binary mismatch.
- Practical status: core Python code is present, but packaging and native binary portability need cleanup.

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

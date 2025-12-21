# Code and Software

The software projects are experimental and serve as testbeds for the theoretical ideas. They are not presented as finished products.

## RGE-256: Recursive-Entropy PRNG

GitHub: https://github.com/RRG314/rge256  
Zenodo: https://doi.org/10.5281/zenodo.17982804  

A family of ARX-based pseudorandom number generators informed by recursive depth and structured entropy control.

Purpose:
- Stress-test recursive entropy ideas
- Explore structured mixing rather than ad hoc randomness

Notes:
- No published core variants fail Dieharder tests
- At least one core was independently tested and validated
- That core was later reengineered in multiple variants following feedback
- Not presented as a cryptographic primitive

## Topological Adam Optimizer

GitHub: https://github.com/RRG314/toplogical-adam  
Zenodo: https://doi.org/10.5281/zenodo.17489664  
Install: `pip install topological-adam`

An experimental PyTorch optimizer inspired by recursive structure and energy balance.

Notes:
- Drop-in replacement for Adam
- Matches standard Adam performance
- In some benchmarks shows improved stability
- Exploratory, not a replacement for established optimizers

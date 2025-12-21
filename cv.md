
## STEVEN REID

Independent Researcher
Manchester, MD
Email: [sreid1118@gmail.com](mailto:sreid1118@gmail.com)
ORCID: 0009-0003-9132-3410
GitHub: [https://github.com/RRG314](https://github.com/RRG314)
PyPI: topological-adam

---

## Professional Summary

Independent researcher and self-taught developer working on recursive algorithms and the mathematical structures that arise from them. My work focuses on how deterministic recursion can generate hierarchy, valuation, and bounded measures without assuming classical axioms at the outset. I develop both theoretical constructions and computational systems to test and refine these ideas.

My research spans recursive integer structures, non-Archimedean style valuations derived from algorithmic depth, entropy behavior across recursive refinement, and practical implementations that stress-test these ideas through software. Alongside the mathematical work, I build open-source tools, validate them using established test suites, and revise my work based on external feedback.

---

## Core Areas of Work

Recursive algorithms and integer structures
Recursive-Adic and depth-based valuation systems
Entropy behavior in hierarchical and recursive systems
Pseudorandom number generator design and validation
Machine learning optimization and numerical stability
Open-source software development

---

## Key Research Contributions

### Recursive Division Tree (RDT)

Developed a deterministic integer recursion that assigns each natural number a depth value based on repeated halving rather than magnitude or prime factorization. The resulting structure forms a tree with ancestry, partial order, and saturation properties. Depth behaves as a bounded structural measure rather than an unbounded size metric.

This construction serves as the foundation for later work in valuation theory, entropy modeling, and algorithmic applications.

Zenodo preprint available.

---

### Recursive-Adic Number Field

Built a valuation framework where scale is defined by recursive depth instead of prime divisibility. The resulting system behaves similarly to non-Archimedean valuations, but its notion of size and convergence is generated algorithmically.

Defined recursive zeta-like transforms, depth-weighted Laplace transforms, and associated analytic properties. This work connects recursion, valuation, and analysis without relying on classical p-adic constructions.

Zenodo preprint available.

---

### Recursive Entropy and Geometric Measures

Defined entropy-like quantities that evolve with recursive refinement rather than static distributions. Entropy is treated as a depth-dependent function with provable bounds and limiting behavior.

Related work explores how entropy behaves under recursive partitioning of geometric objects and how this can be used to analyze structure, regularity, and information flow in hierarchical systems.

Zenodo preprints available.

---

## Computational and Applied Work

### RGE-256 Pseudorandom Number Generators

Designed a family of ARX-based pseudorandom number generators whose internal structure is informed by recursive depth and structured entropy control. These generators were built as testbeds for the theoretical ideas rather than as purely cryptographic constructions.

All published cores pass Dieharder when tested in streaming mode, with no failures observed. At least one core has been independently tested and validated using SmokeRand, TestU01, and PractRand, and was subsequently re-engineered in multiple variants based on feedback from that testing.

The work has undergone several revisions, with changes documented across versions of the preprint in response to external critique. One version was endorsed for arXiv submission but did not pass moderation, leading to continued revision and refinement.

Zenodo preprint and GitHub repositories available.

---

### Topological Adam Optimizer

Developed a PyTorch optimizer inspired by energy balance and coupling ideas from magnetohydrodynamics. The optimizer introduces internal stabilizing fields that regulate update dynamics without relying on gradient clipping.

Topological Adam is available as a pip-installable package and is compatible with existing training pipelines. In benchmark tests, it matches standard Adam and exceeds it in some stability and early-convergence scenarios. The project is intended as an experimental optimizer rather than a replacement for established methods.

Zenodo preprint and GitHub repository available.

---

## Software and Tools

Programming: Python, PyTorch, NumPy, C
Scientific computing and validation: Dieharder, TestU01, PractRand, SmokeRand
Development: Git, GitHub, Jupyter, Google Colab
Packaging and distribution: PyPI, C extensions, reproducible test harnesses

---

## Publications and Preprints (Selected)

Recursive Division Tree: A Log-Log Algorithm for Integer Depth (Zenodo)
The Recursive-Adic Number Field: Construction, Analysis, and Depth Transforms (Zenodo)
Recursive Geometric Entropy: A Unified Framework for Information-Theoretic Shape Analysis (Zenodo)
RGE-256: An ARX-Based Pseudorandom Number Generator with Structured Entropy (Zenodo)
Topological Adam: An Energy-Stabilized Optimizer Inspired by Magnetohydrodynamic Coupling (Zenodo)

---

## Additional Information

Independent researcher with experience developing complete research artifacts from theory through implementation and validation. Actively seeking mentorship, collaboration, and guidance to strengthen formal background and improve research quality. Comfortable revising work in response to critique and external testing.


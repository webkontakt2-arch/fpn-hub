# Benchmark Methodology

This document specifies the evaluation protocol used in public discussion of FPN Hub: tooling, baseline, circuit categories, repetition protocol, and reporting framework at the architecture-level benchmark stage.

## Status

PCT patent pending (priority March 2026). This document is limited to standard, publicly known benchmarking practice. Numerical results, scale ranges, topology parameters, and construction logic are not disclosed here; they are available under NDA.

## Tooling

- Qiskit (1.x or compatible)
- Transpiler `optimization_level = 1` (public communication benchmark series)
- Routing pass: SABRE
- Layout pass: SABRE
- Coupling map: per topology under evaluation

Note: at higher optimization levels (e.g., `optimization_level = 3`) the routing advantage decreases, as aggressive optimization benefits more layout-constrained topologies. The headline signal reported in public materials corresponds to `optimization_level = 1`. Results at other optimization levels are available under NDA.

Reference scripts may be shared with evaluation partners under mutual NDA.

## Baseline

Heavy-Hex (IBM-style lattice) is used as the public reference topology. Additional baselines may be discussed under NDA.

## Circuit categories

Evaluation spans more than one circuit class to avoid drawing conclusions from a single favorable workload. Categories considered include:

- routing-intensive structured circuits (e.g., Quantum Fourier Transform)
- volumetric benchmarks following published quantum-volume conventions
- hardware-efficient variational ansatz patterns
- locality-friendly classes (e.g., GHZ-state preparation, shallow Trotter)

Specific widths, depths, and parameter ranges are not disclosed publicly.

## Repetition

Each (topology, circuit, configuration) point is evaluated across multiple independent seeds for both layout and routing passes. Single-seed outcomes are not treated as evidence; reported signals reflect multi-seed aggregation.

## Reporting

- mean and standard deviation across seeds
- paired comparison between topologies on identical seeds and circuits
- two-qubit gate count and circuit depth reported separately

The last point is intentional: a reduction in routing-induced two-qubit gates does not, on its own, imply a reduction in circuit depth.

## Interpretation

- Architecture-level signal is not equivalent to full-stack hardware advantage.
- Trade-offs are stated rather than averaged away.
- Conditional relevance (workload, scale, hardware) is not reframed as universal superiority.
- The critical open step is validation under matching hardware conditions.

## Contact

For technical dialogue or NDA-based access to scripts and detailed results:

- **Contact:** contact@fpn-systems.com
- **Website:** https://fpn-systems.com



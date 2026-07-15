# Benchmark Methodology

This document summarizes the public evaluation protocol used in the current FPN Hub benchmark discussion. It covers the benchmark stage, tooling, comparison principles, repetition protocol, reporting framework, and interpretation boundaries without disclosing protected topology-construction details.

## Status and authoritative public source

FPN Hub is PCT patent pending (priority March 2026).

Selected numerical results and IP-safe methodological details are publicly reported in the following preprint:

> Sebastian Skalski (2026). _IP-Safe Routing Benchmarks for a Protected Modular Qubit Interconnect: Nonlocality Stress Tests, Compiler Cross-Checks, and Baseline-Specific Trade-offs_. Zenodo.  
> https://doi.org/10.5281/zenodo.21308015

The preprint should be treated as the primary public source for exact reported results, benchmark boundaries, and study-specific conclusions. Protected topology construction logic, topology generators, protected coupling maps, and other non-public implementation details are not disclosed here.

## Tooling

For the main published Qiskit benchmark campaign:

- Qiskit 2.3.1;
- transpiler `optimization_level = 1` for the principal public comparison series;
- SABRE-based layout and routing;
- topology-specific coupling maps supplied to the compiler under the benchmark protocol.

Selected cross-compiler checks are reported in the public preprint. Compiler-dependent behavior is treated as a result rather than assumed away.

Higher optimization settings and alternative compilation choices can change the magnitude of routing differences. Therefore, results are interpreted within the stated compiler and optimization configuration rather than as compiler-independent constants.

## Baselines

Heavy-Hex is used as an important public reference topology, but the published study is not limited to a single baseline.

The public analysis explicitly treats comparative performance as **baseline-specific**. A favorable result against one reference topology is not presented as evidence of superiority over all alternative connectivity structures.

## Workload coverage

The public evaluation uses multiple workload families to reduce the risk of drawing conclusions from a single favorable circuit class. Publicly reported analyses include, among others:

- routing-heavy random workloads;
- QAOA workloads at multiple depths;
- Bernstein–Vazirani workloads;
- GHZ-style locality-friendly control workloads;
- controlled nonlocality stress tests;
- selected established benchmark-circuit families;
- compiler cross-checks for selected comparisons.

The study also reports negative and boundary results where the protected topology does not outperform a comparator.

## Repetition and pairing

Each relevant topology/circuit/configuration point is evaluated across multiple independent seeds where applicable.

Comparisons are paired on matching circuits and benchmark conditions. Single-seed outcomes are not treated as sufficient evidence for a general performance claim.

## Reported metrics

Public reporting distinguishes at least:

- two-qubit gate count;
- circuit depth;
- mean and variability across repeated runs;
- paired topology comparisons under matched benchmark conditions;
- ratio direction, with the numerator and denominator stated explicitly where ratios are used.

Two-qubit gate count and circuit depth are reported separately because a reduction in routing-induced two-qubit gates does not, by itself, imply a reduction in circuit depth.

## Interpretation principles

- Architecture-level transpilation results are not equivalent to hardware-level performance.
- Routing advantage is conditional on workload, baseline, scale, compiler, and benchmark configuration.
- Trade-offs and negative results are reported rather than averaged away.
- Results against a particular baseline are not reframed as universal topology superiority.
- The present public benchmark does not establish fault-tolerant or logical-qubit system advantage.
- Hardware-aware and fault-tolerant/logical-level validation are separate evaluation stages.

## Reproducibility and IP boundary

The public preprint provides the released scientific results and IP-safe methodological description.

This repository does not publish protected construction rules, topology generators, protected coupling maps, internal design parameters, or non-public benchmark materials. Additional scripts, datasets, and topology-specific materials may be made available to suitable evaluation partners under appropriate confidentiality arrangements.

## Contact

For technical dialogue or discussion of evaluation access:

- Contact: contact@fpn-systems.com
- Website: https://fpn-systems.com

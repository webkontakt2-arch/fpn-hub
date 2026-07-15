# FPN Hub — Public Technical Overview

FPN Hub is a deterministic topology framework for quantum processor architectures, designed as an alternative to ad hoc or standard connectivity layouts, with bounded degree and scalable structure in mind.

The project explores how connectivity structure may affect routing overhead, two-qubit gate cost after transpilation, and architecture-level efficiency as systems scale.

## Repository scope

This repository is intentionally limited to public technical framing. It supports orientation and dialogue for potential evaluation partners.

Selected IP-safe benchmark results are now publicly available, but this repository does **not** disclose protected topology construction logic, topology generators, coupling maps, internal architectural mechanisms, or other implementation details reserved under the FPN Hub intellectual-property boundary.

The benchmark protocol used in public discussion is summarized in [docs/benchmark-methodology.md](docs/benchmark-methodology.md).

## Status

PCT patent pending (priority March 2026).

## Public research

A technical preprint reporting IP-safe routing benchmarks, nonlocality stress tests, compiler cross-checks, and baseline-specific trade-offs is publicly available on Zenodo:

> **Sebastian Skalski (2026). _IP-Safe Routing Benchmarks for a Protected Modular Qubit Interconnect: Nonlocality Stress Tests, Compiler Cross-Checks, and Baseline-Specific Trade-offs_.**  
> DOI: [10.5281/zenodo.21308015](https://doi.org/10.5281/zenodo.21308015)

The preprint is the primary public source for the reported numerical benchmark results and their stated limitations.

## Public benchmark signal

In the published benchmark campaign, selected routing-heavy workloads reached a **baseline/FPN two-qubit gate-count ratio of up to 3.69×** relative to the corresponding Heavy-Hex baseline under the reported transpilation conditions.

This is a conditional architecture-level result, not a claim of universal superiority and not a hardware-validated or fault-tolerant-computing result. The public study also reports workload-, baseline-, scale-, and compiler-dependent trade-offs, including cases where competing topologies are preferable.

Further work is extending validation toward more hardware-aware and fault-tolerant/logical-workload settings. No hardware-level or FTQC advantage is claimed by the current public benchmark study.

## Public / protected boundary

Publicly available material includes selected benchmark results, methodological framing, comparative analyses, and IP-safe research conclusions.

The following remain outside the public scope of this repository:

- protected topology construction rules and internal architectural mechanisms;
- topology generators and protected coupling-map definitions;
- non-public implementation materials and internal design parameters;
- unpublished benchmark campaigns, scripts, and datasets not explicitly released by FPN Systems.

Additional technical material may be reviewed with suitable evaluation partners under appropriate confidentiality arrangements.

## Project links

- Project website: https://fpn-systems.com
- LinkedIn: https://www.linkedin.com/in/sebastian-skalski-phd
- Public preprint: https://doi.org/10.5281/zenodo.21308015

## Collaboration

FPN Hub is open to technical discussion, architecture evaluation, benchmarking dialogue, licensing conversations, and selected strategic collaboration with partners working in:

- quantum hardware;
- processor architecture;
- compiler or transpilation research;
- benchmarking infrastructure;
- fault-tolerant quantum-computing architecture;
- related deep-tech areas.

## How to cite

For scientific discussion of the public benchmark results, please cite the Zenodo preprint:

> Skalski, S. (2026). _IP-Safe Routing Benchmarks for a Protected Modular Qubit Interconnect: Nonlocality Stress Tests, Compiler Cross-Checks, and Baseline-Specific Trade-offs_. Zenodo. https://doi.org/10.5281/zenodo.21308015

For reference to this repository itself, see [CITATION.cff](CITATION.cff).

## Contact

- Contact: contact@fpn-systems.com
- Website: https://fpn-systems.com

## License

See [LICENSE](LICENSE). All rights reserved.

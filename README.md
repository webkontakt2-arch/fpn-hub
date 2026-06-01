# FPN Hub — Public Technical Overview

FPN Hub is a deterministic topology framework for quantum processor architectures, designed as an alternative to ad hoc or standard connectivity layouts, with bounded degree and scalable structure in mind.

The project explores how connectivity structure may affect routing overhead, two-qubit gate cost after transpilation, and architecture-level efficiency as systems scale.

## Repository scope

This repository is intentionally limited to public technical framing. It supports orientation and dialogue for potential evaluation partners. It does not disclose protected implementation details, topology construction logic, internal architectural mechanisms, or non-public benchmark data.

The benchmark protocol used in public discussion is documented in [`docs/benchmark-methodology.md`](docs/benchmark-methodology.md).

## Status

PCT patent pending (priority March 2026).

## Public benchmark signal

In public communication materials, FPN Hub has been reported as reaching up to ~3.9× fewer two-qubit gates vs Heavy-Hex in routing-heavy workloads at the transpilation level.

This is a conditional architecture-level signal — not a universal advantage and not yet a hardware-validated result. Detailed numerical results, scripts, topology-specific materials, and additional baselines are available only under appropriate confidentiality.

## Visual summary

A short visual summary of the benchmark story is available here:

- Project website: https://fpn-systems.com
- LinkedIn: [Sebastian Skalski, PhD](https://www.linkedin.com/in/sebastian-skalski-phd)

Selected public materials will be available in the `media/` folder.

## Collaboration

FPN Hub is open to technical discussion, architecture evaluation, benchmarking dialogue, licensing conversations, and selected strategic collaboration with partners working in:

- quantum hardware
- processor architecture
- compiler or transpilation research
- benchmarking infrastructure
- related deep-tech areas

Detailed technical material — reference scripts, numerical benchmark results, and topology specifics — is available for direct review under appropriate confidentiality.

## How to cite

If you refer to this public overview, please cite:

> Skalski, S. (2026). *FPN Hub: Public Technical Overview*. FPN Systems. PCT patent pending.

See also [`CITATION.cff`](CITATION.cff).

## Contact

- **Contact:** contact@fpn-systems.com
- **Website:** https://fpn-systems.com

## License

See [LICENSE](LICENSE). All rights reserved.

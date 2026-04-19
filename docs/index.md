# Boot2Trust – Embedded Linux Security Lab

Boot2Trust is a hands-on, phase-driven project demonstrating end-to-end security in embedded Linux systems, inspired by automotive ECU architectures.

The documentation walks through a chain of trust from hardware-backed roots to verified boot, runtime integrity, access control, and isolation.

This repository is the source for the GitHub Pages site. For local development and build instructions, see `README.md`.

## Phases

- [Phase 1: Root of Trust](./phase1-root-of-trust/)
- [Phase 2: Secure Boot](./phase2-secure-boot/)
- Phase 3: Runtime Integrity (Coming Soon)
- Phase 4: Access Control (Coming Soon)
- Phase 5: Isolation (Coming Soon)
- Phase 6: Platform Comparison (Coming Soon)

## Core objectives

- Demonstrate end-to-end system security, not just component-level features
- Bridge hardware trust concepts → OS enforcement → userspace isolation
- Show attack vs defense behavior with observable logs
- Align implementations with regulatory expectations like CRA and ISO/SAE 21434

## Methodology

Each phase includes:
- Problem definition from an automotive or embedded scenario
- Architecture overview
- Implementation code and configuration
- Attack simulation (tampering / misuse)
- Observed system behavior and logs
- Regulatory mapping

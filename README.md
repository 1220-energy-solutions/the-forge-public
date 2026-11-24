# The Forge

**Open scientific research into spherical magnetic confinement and charged-particle dynamics.**

A Gardeners of the Galaxy initiative.

## Research Mission

The Forge is an independent computational research project investigating the behavior of charged particles in an idealized spherical magnetic geometry based on a truncated-icosahedron (buckyball) arrangement of coils.

The goal is to characterize the magnetic topology, identify possible confinement or loss channels, and test numerical methods for tracking single-particle trajectories. This work is exploratory. It is not a demonstration of plasma confinement, fusion, tritium breeding, nuclear transmutation, or net energy production.

## Current Model (Idealized)

- 32 magnetic faces
- 320 individual coil loops
- Prescribed magnetic field (not self-consistent)
- Boris-type particle integrator
- Single test particles or small independent ensembles

All simulations use a fixed magnetic field. There is no plasma, no self-consistent currents, and no collective effects.

## Scientific Limitations

- Results are computational observations of independent test particles in a prescribed field.
- Numerical convergence and energy conservation are under active investigation.
- Near magnetic nulls, guiding-center theory is expected to break down; this is being studied but not yet fully characterized.
- No claim is made of demonstrated plasma confinement, fusion, or a working reactor.
- Hardware has not been built. These are simulations only.

## Status

This public repository is for open documentation of methods, limitations, and selected results as they are validated. Detailed private research records remain in a separate private repository.

## Navigation

- [MASTER_VISION.md](MASTER_VISION.md) — High-level overview
- [RESEARCH_STATUS.md](RESEARCH_STATUS.md) — Current verified findings and open questions
- [methodology/](methodology/) — Magnetic geometry, integrator, validation
- [experiments/](experiments/) — Individual experiment reports
- [ROADMAP.md](ROADMAP.md) — Planned priorities
- [AI_COLLABORATION.md](AI_COLLABORATION.md) — Roles and oversight
- [research_briefs/](research_briefs/) — Public summaries
- [CHANGELOG.md](CHANGELOG.md) — Update history

## Contact

Independent research. No institutional affiliation.

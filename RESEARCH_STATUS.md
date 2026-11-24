# Research Status

The Forge · Operation Pink Eye · 24 November 2026, 20:52 UTC

The current campaign studies independent charged particles in an idealized 32-face, 320-coil magnetic geometry. Results concern sampled trajectories and numerical performance in prescribed fields. Collective plasma confinement, fusion, tritium breeding, transmutation and net energy remain separate research questions.

## Trajectories and magnetic topology

| Experiment | Status and evidence |
| --- | --- |
| 6 · Short convergence | The 2 µs baseline showed approximately second-order endpoint convergence across 20, 10 and 5 ps. |
| 7 · Long baseline | Both 20 µs runs completed. The 10 and 5 ps endpoints differed by 19.95 mm in position and 10.14 km/s in velocity. Long-window convergence remains unresolved. |
| 8 and 11 · Radial escape | The radial 10 eV launch from 30 cm approached the diagnostic sphere by 2 µs and first reached the 40 cm threshold at about 2.28470 µs in the extended run. This motivates the proposed loss-channel mapping. |
| 9 and 13 · Independent ensemble | Experiment 13 repeated the twelve Experiment 9 launch vectors for 10 µs at 20 ps. Zero particles reached the 40 cm threshold at a sampled step. The largest sampled radius was 30.22525 cm, and the relative kinetic-energy drift was bounded by about 1.24 × 10⁻¹³. The run used one timestep. |
| 10 · Near-null diagnostics | Archived checkpoints sampled every 1 µs show very weak fields near the center. Sampling leaves closest approach, the interpretation of pitch changes and magnetic-moment behavior unresolved. |
| 12 · Finer 20 µs comparison | Available records reach 1 µs at 2.5 ps. Final outcome and current execution status remain unverified. |
| 14 · Static axial bias | Mapping and local null searches are complete. Off-center candidate nulls were found at 0.01, 0.1 and 1 T. The map extends to 30 cm, and the searches do not establish a complete null inventory. Phase 3 had recorded 16 of 24 trajectories complete. The latest radial and tangential progress checkpoints were 700,000 and 750,000 of 1,200,000 steps on their in-progress trajectories. |
| 15 · Escape-channel mapping | Proposed. It will examine changes in crossing behavior under controlled launch position and direction perturbations. |

## Computational acceleration

- **Experiment 16 feasibility completed.** On one 32-point query stream, direct batching reduced field-query time from 170.1 ms to 9.26 ms, about 18.4×. The hybrid fell back on 90.6% of those queries, was slower than batched direct, and showed a sampled interpolation-to-direct field-error jump of 23.9 mT. Weak-pocket, coarse–fine and interpolated grazing tests remained incomplete. [Pilot report](AI_EXCHANGE.md#experiment-16--feasibility-pilot-results)
- **Experiment 17 feasibility completed.** In short 20-step trials, median end-to-end speedups at 1, 12, 32, 100 and 1,000 particles were 1.07×, 4.10×, 7.72×, 11.10× and 17.61×. Peak RSS at 1,000 particles was 84.3 MiB for both methods. All 15 timing pairs matched on saved positions, velocities, sampled radius extrema and crossing records. The maximum field difference was 3.67 × 10⁻¹⁵ T. [Feasibility report and review questions](AI_EXCHANGE.md#experiment-17--batched-direct-field-feasibility)

## Open questions

- Does the 20 µs baseline converge at finer timesteps, and which observables stay consistent?
- How wide is the radial loss channel, and how do biased and weak-field regions change first-passage behavior?
- Does batched direct integration preserve first-crossing steps in crossing-positive cases and stay in agreement over longer windows? Do the measured speedups hold at other chunk sizes and over longer integrations?

Longer runs and new experiments require separate approval.

# Satellite Null Check — Preliminary Magnetostatic Modeling

**Date:** November 27, 2026  
**Operation:** Dynamic Core  
**Status:** Exploratory computational research. Not experimental evidence of plasma confinement.

## Summary

A truncated-icosahedron (buckyball) array of 32 radial dipoles was examined to determine whether the twelve pentagon-aligned low-field regions identified on a coarse grid contain independent magnetic vector zeros.

Successive local refinements did not demonstrate independent satellite nulls. Sampled minima migrated toward the origin and remained on the boundaries of the search volumes.

## Numerical Results

| Description | Grid spacing | Field magnitude |
|-------------|--------------|-----------------|
| Original satellite centroid | 2 mm | 0.021019 µT |
| Local minimum (first refinement) | 0.5 mm | 0.001135 µT |
| Local minimum (re-centered) | 0.25 mm | 0.000116 µT |
| Approximate final sampled position | — | [−9.4, 0, −0.1] mm |

A radial scan along the line from the origin through one candidate corner showed field magnitude increasing from 40 mm to 90 mm, then decreasing at 100 mm.

## Observations

- Eleven of the twelve coarse-grid satellites were sampled and returned identical minimum magnitudes to the displayed precision under the same protocol. The twelfth satellite remains unverified pending recovery of its output.
- Every reported minimum occurred on the boundary of its search box.
- Re-centering a smaller volume on the previous boundary minimum produced a still lower value at a location closer to the origin.
- Along the tested radial direction the field rose from 40 mm to 90 mm before falling at 100 mm.

## Conclusions (as of this date)

- **Central null:** Established by symmetry within the numerical model. The field at the geometric center is a vector zero to machine precision.
- **Independent satellite nulls:** Not demonstrated. Successive refinements walked inward rather than locking onto separate local minima.
- **Secondary nulls:** Not definitively excluded. The present sampling does not constitute a complete topological search of the original satellite volumes.
- **Next step:** Localized vector root-finding ($B_x = B_y = B_z = 0$) with Jacobian validation inside the original satellite regions, performed in a new experiment directory without modification of prior archives.

## Limitations

- Boundary minima indicate the search volumes may have clipped a continuous low-field structure rather than isolating independent zeros.
- No explicit finite-value masking of NaN or excluded-source regions was applied in the preliminary scripts.
- Results are specific to the ideal point-dipole model and the exclusion mask used. Finite-size magnet effects and mechanical equilibrium remain untested.
- This work is pure magnetostatics. No plasma dynamics or confinement claims are implied.
- Only eleven of the twelve satellites were confirmed in the printed output; the twelfth requires separate verification.

## Archival Note

Four exploratory scripts were created inside the existing magnetostatics_011 directory during the investigation. The original archived results (field volumes, connectivity meshes, alignment tables, and checksums) were not overwritten. Future root-finding work will be conducted in a separate experiment directory.

---

*Exploratory computational research. Follow the evidence.*

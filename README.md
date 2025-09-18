## Overview
ANSYS Fluent, one of the leading tools in computational fluid dynamics (CFD), directly solves the Navier–Stokes equations using models such as RANS or LES, including turbulence approaches like SST. This enables the capture of three-dimensional flow phenomena such as separation, vortices, and recirculation, providing a more realistic representation of aerodynamic behavior near the wing surface.

This project presents a computational analysis of three-dimensional wing aerodynamics, a key aspect in aircraft design. Two wings with different geometric characteristics but common airfoils are considered: a NACA 7715 at the root and a NACA 0009 at the tip. The study focuses on evaluating how variations in sweep angle, aspect ratio, and taper ratio affect overall performance through simulations in ANSYS Fluent.
<div align="center">

| Property                                | Wing 1 | Wing 2 |
|-----------------------------------------|--------|--------|
| Sweep angle (°)                         | 0      | 15     |
| Taper ratio                             | 1      | 0.3    |
| Aspect ratio                            | 5      | 10     |
| Root chord [m]                          | 1      | 1      |
| Dihedral angle (°)                      | 0      | 0      |

</div>
  
<div align="center">
  <img src="docs/images/tip.gif" alt="docs/images/tip.gif" width="800"/>
  
  <a id="figure-1-wing-2"><strong>Wing 2</strong></a>  
</div>

The numerical simulation results show that Wing 2 consistently produces a higher lift coefficient (Cl) than Wing 1, approximately 15–20% greater, due to its higher aspect ratio. Sweep angle and tapering of Wing 2 slightly reduce the Cl–α slope, but the effect of aspect ratio dominates. Lift increases with Reynolds number for both wings, consistent with boundary layer theory.

However, Wing 2 also exhibits significantly higher drag (Cd), driven by its greater lift, tip taper, and sweep, which increase parasitic and pressure drag. Wing 1, with a rectangular and unswept planform, maintains a more uniform pressure distribution and lower Cd. Aerodynamic efficiency (L/D) is similar for both wings and slightly increases with Reynolds number; surprisingly, Wing 1 shows slightly higher efficiency due to the combined geometric effects of Wing 2 that counteract the theoretical benefits of its higher aspect ratio.

## Objectives
- To design and simulate complex three-dimensional wing structures in ANSYS Fluent
- To analyze the effect of wing geometric characteristics on 3D aerodynamics

## Software & Tools
- **Airfoil Tools**: NACA 4-digit generator (.dat file).  
- **Ansys Workbench**:  
  - *SpaceClaim*: Geometry modeling.  
  - *Meshing*: Grid generation.  
  - *Fluent*: CFD simulation and post-processing. 

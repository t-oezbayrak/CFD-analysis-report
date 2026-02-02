# CFD-analysis-report

CFD Analysis Report: Multi-Element Rear Wing Profile (2D)
Case Study: High-Downforce Multi-Element Airfoil (Main Plane + 2 Flaps) Solver: RANS (Reynolds-Averaged Navier-Stokes) Turbulence Model: k-omega SST

1. Pressure Distribution Analysis
<img width="1260" height="425" alt="Screenshot 2026-02-02 151451" src="https://github.com/user-attachments/assets/e51b3474-21c3-4fcc-96c8-69ee800ab045" />

Observation: The static pressure contour demonstrates a clear distinction between the pressure side (concave surface, High P approximately 6.8e4 Pa) and the suction side (convex surface, Low P approximately -76k Pa).

Physics: Strong stagnation points are visible at the leading edges of all three elements. The pressure recovery towards the trailing edge suggests high load generation, characteristic of a high-downforce F1-style setup.

. Turbulence & Flow Separation (Kinematic Viscosity)

<img width="1270" height="437" alt="Screenshot 2026-02-02 151530" src="https://github.com/user-attachments/assets/acdc9149-62c9-49bd-af67-d8d8a0fd33bc" />

Observation: The Turbulent Kinematic Viscosity plot reveals the energy dissipation in the wake region.

  High Values (Light Blue): Indicate regions of high turbulence mixing and potential flow separation.

  Low Values (Dark Blue): Indicate laminar or attached turbulent flow (freestream).

Critical Finding: A significant wake region is observed behind the second flap. The expansion of the high-viscosity zone suggests flow separation (stall) on the suction side of the steepest flap. This indicates that the current Angle of Attack (AoA) may be too aggressive for the current slot-gap configuration, leading to induced drag.

Conclusion & Next Iteration Strategy
Based on the visual data above, the current design generates high downforce but suffers from aerodynamic inefficiency due to separation.

Planned Improvements for Iteration v2:

Slot Gap Optimization: Adjust the gap and overlap parameters between the main plane and flaps to re-energize the boundary layer and delay separation.

Angle of Attack (AoA) Reduction: Slightly reduce the angle of the final flap to attach the flow and improve the L/D (Lift-to-Drag) ratio.

Mesh Refinement: Increase mesh density specifically in the wake region (seen in the blue plot) to capture the shear layer gradients more accurately.

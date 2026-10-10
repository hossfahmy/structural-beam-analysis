# Beamline — Simple Beam Analysis

A small, dependency-free browser app for structural beam analysis with downward point loads and uniform distributed loads.

## Run it

Open `index.html` in a modern browser. No server or installation is required.

## Inputs and results

- Metric (m, kN, GPa, cm⁴) or English (ft, kip, ksi, in⁴) units. Switching units converts the current model.
- Simply supported, cantilever, or custom beams with pin, roller, and fixed supports at user selected positions.
- Point loads and uniform distributed loads with locations along the span.
- Vertical support reactions, fixed end reaction moments, shear force, bending moment, and elastic deflection diagrams.

The diagrams and results update when inputs change. The solver uses a one dimensional Euler–Bernoulli beam finite element model with constant `E` and `I`. Supports at a single location must include a fixed restraint; otherwise, provide two or more distinct vertical supports.

## Model assumptions

The beam is prismatic with constant `E` and `I`, linearly elastic, and subject to small deflections. Loads are vertical and downward; positive bending moment is sagging. Pin and roller supports are equivalent for the vertical beam model; pin horizontal reaction, self-weight, axial effects, shear deformation, settlement, and non-uniform stiffness are not included.

Use this as a learning and preliminary analysis tool. Confirm structural designs with appropriate engineering methods and applicable design codes.

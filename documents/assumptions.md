# Prototype1 SRM — Assumptions Document

## 1. Purpose

This document captures the **explicit technical assumptions** used throughout the design, analysis, manufacturing, and testing of the Prototype1 Solid Rocket Motor (SRM). These assumptions bound the validity of results and ensure traceability between theory, simulation, and experiment.

All analyses, conclusions, and design decisions in this repository are contingent on the assumptions stated herein unless otherwise noted.

---

## 2. General Program Assumptions

* The Prototype1 SRM is a **developmental / experimental motor**, not intended for flight hardware without further qualification.
* The design prioritizes **learning, validation, and risk reduction** over mass or performance optimization.
* All work is conducted in compliance with applicable institutional, laboratory, and safety requirements.
* Conservative engineering judgment is preferred when uncertainty exists.

---

## 3. Physical & Environmental Assumptions

* Ambient pressure is assumed to be **1 atm (101.3 kPa)** unless otherwise stated.
* Ambient temperature during testing is assumed to be **20–25 °C**.
* Effects of humidity on propellant performance are neglected unless explicitly modeled.
* Gravity is assumed constant at **9.81 m/s²**.
* Wind and external aerodynamic effects are neglected (static-fire assumption).

---

## 4. Propellant Assumptions

* The propellant is assumed to be **homogeneous and isotropic** at the scale relevant to burn regression.

* Burn rate follows a **Saint Robert (Vieille) law** of the form:

  r = a · Pⁿ

* Burn rate coefficients (*a*, *n*) are assumed constant over the operating pressure range unless otherwise stated.

* No erosive burning is assumed unless explicitly modeled.

* Propellant density is assumed uniform and constant throughout the grain.

* Cracks, voids, and debonding are assumed absent at ignition.

---

## 5. Internal Ballistics Assumptions

* Chamber pressure is spatially uniform (0-D / quasi-1D assumption).
* Flow is assumed **quasi-steady** at each timestep.
* Combustion efficiency is assumed constant.
* No two-phase flow losses are modeled.
* Slag accumulation effects are neglected.
* Igniter mass flow contribution is neglected after initial pressurization.

---

## 6. Nozzle & Flow Assumptions

* Nozzle flow is assumed **isentropic** up to the exit plane.
* Flow is choked at the throat during nominal operation.
* Nozzle expansion is assumed axisymmetric.
* Boundary layer losses are neglected unless explicitly included.
* Nozzle efficiency is assumed constant.
* Flow separation is neglected unless chamber pressure falls below design limits.

---

## 7. Thermal Assumptions

* Heat transfer is modeled using **lumped or simplified 1-D conduction** where applicable.
* Radiative heat transfer inside the chamber is neglected unless stated otherwise.
* Material properties are assumed constant over the operating temperature range unless explicitly modeled.
* Steady-state or quasi-steady thermal behavior is assumed for short burn durations.

---

## 8. Structural Assumptions

* Structural analysis assumes **linear elastic material behavior**.
* Loads are axisymmetric.
* Dynamic pressure oscillations are neglected unless otherwise stated.
* Stress concentrations at threads, fillets, and transitions are handled via conservative factors rather than detailed local modeling unless noted.
* Manufacturing tolerances are assumed to fall within specified limits.

---

## 9. Manufacturing & Assembly Assumptions

* Manufactured parts conform to nominal CAD geometry within tolerance.
* Assembly is performed correctly and repeatably.
* Proper bonding and curing of propellant and liners is achieved.
* No foreign object debris (FOD) is present within the motor at ignition.

---

## 10. Testing Assumptions

* Instrumentation is calibrated prior to testing.
* Data acquisition sampling rates are sufficient to capture relevant dynamics.
* Load cells measure axial thrust only.
* Sensor lag and noise are negligible relative to observed trends unless otherwise stated.

---

## 11. Safety Assumptions

* All personnel involved are trained for their assigned tasks.
* Approved safety procedures are followed at all times.
* Emergency response measures are available and functional during testing.

---

## 12. Assumption Validity & Change Control

* Assumptions shall be reviewed whenever:

  * Test data deviates significantly from predictions
  * Major design changes are introduced
  * Operating regimes change

* Invalidated assumptions must be:

  * Explicitly documented
  * Updated in this file
  * Referenced in affected analyses

---

*This document is a living artifact and shall evolve as Prototype1 SRM matures.*

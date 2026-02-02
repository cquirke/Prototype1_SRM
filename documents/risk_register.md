# Prototype1 SRM — Risk Register

## 1. Purpose

This document identifies, assesses, and tracks **technical, safety, schedule, and programmatic risks** associated with the Prototype1 Solid Rocket Motor (SRM). The goal is to proactively reduce the likelihood and consequence of failures through mitigation, monitoring, and informed decision-making.

This risk register is a **living document** and shall be updated as the design matures, tests are conducted, and new information becomes available.

---

## 2. Risk Scoring Methodology

Each risk is evaluated using the following criteria:

### 2.1 Likelihood (L)

| Score | Description                            |
| ----: | -------------------------------------- |
|     1 | Unlikely (rare or theoretical)         |
|     2 | Low (has occurred in similar systems)  |
|     3 | Moderate (credible during development) |
|     4 | High (likely without mitigation)       |
|     5 | Very High (expected to occur)          |

### 2.2 Consequence (C)

| Score | Description                                    |
| ----: | ---------------------------------------------- |
|     1 | Negligible (no damage or data loss)            |
|     2 | Minor (repairable hardware damage)             |
|     3 | Moderate (test failure or major rework)        |
|     4 | Severe (loss of hardware, safety incident)     |
|     5 | Critical (serious injury or catastrophic loss) |

### 2.3 Risk Level

Risk Level = **L × C**

| Score | Classification |
| ----: | -------------- |
|   1–5 | Low            |
|  6–10 | Medium         |
| 11–15 | High           |
| 16–25 | Critical       |

---

## 3. Risk Register

| ID   | Risk Description                                            | Category           | L | C | Risk | Mitigation / Controls                                                           | Status |
| ---- | ----------------------------------------------------------- | ------------------ | - | - | ---- | ------------------------------------------------------------------------------- | ------ |
| R-01 | Chamber overpressure due to incorrect burn rate assumptions | Technical / Safety | 3 | 4 | 12   | Conservative burn-rate coefficients, pressure margin, hydrostatic proof testing | Open   |
| R-02 | Grain cracking or debonding leading to pressure spike       | Technical / Safety | 3 | 5 | 15   | Visual inspection, controlled casting and cure, conservative ignition           | Open   |
| R-03 | Nozzle throat erosion exceeding predictions                 | Technical          | 3 | 3 | 9    | Conservative throat sizing, erosion margin, post-test inspection                | Open   |
| R-04 | Casing structural failure                                   | Safety             | 2 | 5 | 10   | Factor of safety >1.5, material certification, proof testing                    | Open   |
| R-05 | Ignition failure or hard start                              | Technical / Safety | 3 | 4 | 12   | Igniter ground testing, controlled ignition energy                              | Open   |
| R-06 | Instrumentation failure or bad data                         | Test               | 3 | 2 | 6    | Sensor calibration, redundancy where practical                                  | Open   |
| R-07 | Thermal damage to casing or closures                        | Technical          | 2 | 4 | 8    | Thermal modeling, insulation margin                                             | Open   |
| R-08 | Manufacturing tolerance stack-up                            | Manufacturing      | 2 | 3 | 6    | Critical dimension review, inspection                                           | Open   |
| R-09 | Schedule delay due to rework or failed tests                | Programmatic       | 3 | 2 | 6    | Incremental testing, buffer time                                                | Open   |
| R-10 | Safety non-compliance during handling or testing            | Safety             | 2 | 5 | 10   | Safety procedures, trained personnel, supervision                               | Open   |

---

## 4. Risk Ownership

* Each risk shall have a **responsible owner** assigned when the project scales beyond a single contributor.
* The owner is responsible for:

  * Tracking mitigation actions
  * Updating likelihood and consequence scores
  * Closing the risk when appropriate

---

## 5. Risk Review Triggers

The risk register shall be reviewed and updated when any of the following occur:

* Major design change
* New analysis invalidates a prior assumption
* Static fire or subsystem test is completed
* A near-miss or anomaly is observed

---

## 6. Risk Closure Criteria

A risk may be closed when:

* Mitigation actions are implemented
* Test or analysis data confirms acceptability
* Residual risk is documented and accepted

Closed risks shall remain documented for traceability.

---

## 7. Relationship to Other Documents

This document is directly linked to:

* `assumptions.md`
* `requirements.md`
* Test reports and post-test reviews

Changes in assumptions or requirements shall prompt a risk review.

---

*This risk register supports informed, disciplined development of the Prototype1 SRM.*

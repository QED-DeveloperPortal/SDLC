---
index: true
---
# Test Stage

## Overview

During the Test stage, stakeholders verify that the release or system fulfils the documented requirements and behaves as expected.
This stage validates the solution before it is considered production-ready.


## Purpose

To transition from the build maturity milestone to the production maturity milestone by verifying that the system meets its requirements, is stable, and is ready for operational use.


## Artefacts

| Artefact                                                          | Description                                                                                                                                  |
| ----------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Acceptance Test Summary Report                                    | Summary of user acceptance test results.                                                                                                     |
| Secondary Acceptance Test Summary Report (for high-risk releases) | Secondary UAT results required for high-risk releases or solutions.                                                                          |
| Quality Assurance Certificate (all releases)                      | Checklist demonstrating that the release has passed required quality checkpoints.                                                            |
| Production Readiness Certificate (Type 1 releases)                | Checklist confirming readiness for production and completion of quality checkpoints. May depend on late-stage vulnerability or load testing. |
| Operational Support Plan                                          | Details of operational arrangements required to keep the release running and supported; prerequisite for production maturity.                |


## Controls

* All artefacts must be updated and signed off by relevant parties.
* High-risk releases require a Secondary Acceptance Test Summary Report.
* Type 1 releases require a Production Readiness Certificate.
* All releases require a Quality Assurance Certificate.


## Stage Processes


### Pre-Verification Deployment Process

#### Purpose

To deploy the release into the User Acceptance environment so relevant stakeholders can test and verify the solution.

#### Outcomes

* The release is deployed and available in the user acceptance or QA environment.
* The deployment plan is validated and up to date.
* Release packages consist of compatible components.
* Release package integrity is maintained.
* All deployment packages are trackable, installable, testable, verifiable, and removable/rollback-ready.
* Deviations, risks, and issues are identified and managed.
* Appropriate level of rigour is applied based on release risk.


### Verification Process

#### Purpose

To provide objective evidence that a release or system fulfils its specified requirements and characteristics.
The Verification Process identifies anomalies (errors, defects, or faults) and informs required corrective actions.

Aligned with the **ISO 15288 Verification Process**.

*Note:*
Verification checks that the *product is built right*.
Validation checks that the *right product is built*.

#### Outcomes

* Verification constraints affecting requirements, architecture, or design are identified.
* Required enabling systems and services for verification are available.
* The release or system is verified.
* Data for corrective actions is produced.
* Evidence is generated showing the system fulfils requirements, architecture, and design.
* Verification results and anomalies are documented.
* Traceability of verified elements is established.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                                           | Description                                                                                                     |
| -------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Acceptance Test Summary Report                     | User acceptance test results.                                                                                   |
| Secondary Acceptance Test Summary Report           | Secondary UAT results for high-risk releases.                                                                   |
| Production Readiness Certificate (Type 1 releases) | Evidence that a Type 1 release has passed quality checkpoints and is ready for its first production deployment. |
| Operational Support Plan                           | Operational arrangements for supporting the release in production.                                              |


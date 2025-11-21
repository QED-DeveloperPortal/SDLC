# Deployment Stage

## Overview

During the Deployment stage, the release or solution is deployed into the production environment.
This is where the system transitions from “ready to release” to “delivered”.


## Purpose

To transition from the production readiness milestone to the delivery milestone.
For Type 2 and Type 3 releases, this stage represents the final delivery goal.
For Type 1 releases, delivery is only complete after the Transition stage is finished and business benefits are realized.


## Artefacts

| Artefact                  | Description                                                                                                  |
| ------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Vulnerability Test Report | Results of vulnerability testing, applicable only when criteria for mandatory vulnerability testing are met. |
| Load Test Report          | Results of load testing.                                                                                     |
| Release Completion Report | Summary of the outcomes of the deployment stage.                                                             |


## Controls

* A Release Completion Report must be produced and signed by all relevant parties.


## Stage Processes


### Staging (Mirrored) Production Environment Deployment Process

#### Purpose

To ensure the release or solution is functioning correctly in a staging (mirrored) production environment, with interfaces tested and deployment steps validated before going live.

#### Notes

* The staging environment must be a *true mirror* of production and capable of delivering identical services.
* This environment supports more than “practice deployments”; it is part of achieving pre-production maturity.
* All mirrored services and systems must be kept fully synchronized with production.

#### Outcomes

* Deployment authorities confirm deployment plans are accurate and feasible.
* Initial health checks are completed before final go-live.
* Appropriate rigour is applied based on release risk.
* Vulnerability tests are performed where applicable.
* Load testing is completed.

#### Artefacts

| Artefact                  | Description                                       |
| ------------------------- | ------------------------------------------------- |
| Vulnerability Test Report | Results of vulnerability testing when applicable. |
| Load Test Report          | Results of load testing.                          |



### Vulnerability Testing Applicability Criteria

| Criteria                                             | Question                                                                                                        | Yes?      | No?           |
| ---------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------- | ------------- |
| Data persistence backend for public-facing solutions | Is this the first release of a public-facing solution (on-premises or cloud) with any data persistence backend? | Mandatory | Not Mandatory |
| Data classification changes                          | Has data classification changed to a more restrictive level (e.g., public → protected)?                         | Mandatory | Not Mandatory |
| Cloud/on-premises nature                             | Is this the first release of a cloud-based solution (public or internal)?                                       | Mandatory | Not Mandatory |


### Production Environment Deployment Process

#### Purpose

To deploy the release or solution into the production environment and begin operationalization for end users.

#### Notes

* Success in the Staging (Mirrored) Deployment Process is a mandatory prerequisite.
* Health checks must confirm correct behaviour before proceeding.

#### Outcomes

* The release is deployed to production in a controlled manner that preserves environment integrity.
* Issues encountered are recorded and resolved.
* Rollback steps are prepared and executed if required.
* Appropriate rigour is applied based on release risk.

#### Artefacts

| Artefact                  | Description                     |
| ------------------------- | ------------------------------- |
| Release Completion Report | Summary of deployment outcomes. |



### Early Life Support Process

#### Purpose

To rapidly identify and resolve operational issues immediately after deployment.
Applicable **only to high-risk releases**.

#### Outcomes

* Additional attention and resources are allocated to the new release.
* The solution is monitored for abnormal behaviour.
* Issues and errors encountered post-deployment are recorded, classified, and managed.
* Suitable solutions are analysed and implemented.
* Problems are tracked to closure and logged.
* Appropriate rigour is applied based on release risk.



### Transition Process

#### Purpose

To establish full operational capability, ensuring the system can provide its intended services in the operational environment.
This includes installation of verified system elements and all required enabling systems, including training and support.

Aligned with the **ISO 15288 Transition Process**.

*Applicable only to Type 1 releases.*

#### Outcomes

* The system operates at its designated location and performs its required functions.
* Operators, users, and supporting stakeholders are fully trained.
* Transition anomalies are identified and resolved.
* The system is activated and ready for use.
* Traceability for transitioned elements is established.
* Appropriate rigour is applied based on release risk.

*Note:*
Transition may begin immediately after production deployment and can run in parallel with Maintenance and Support activities.



### Validation Process

#### Purpose

To confirm that the system, when used in a real operational environment, fulfils its business or mission objectives and delivers the expected benefits.
Validation builds confidence that the “right product” has been delivered.

Aligned with the **ISO 15288 Validation Process**.
*Applicable only to Type 1 releases.*

#### Notes

* Validation criteria should ideally be defined earlier in the life cycle.
* Validation may extend over time and can run in parallel with Maintenance and Support processes.
* Encouraging business-led validation strengthens ownership and ensures benefits are measurable.

#### Outcomes

* Validation criteria for stakeholder requirements are defined.
* Validation constraints affecting requirements, architecture, or design are identified.
* The system is validated in its operational environment.
* Validation results and anomalies are recorded.
* Evidence is produced confirming the system delivers expected business benefits.
* Appropriate rigour is applied based on release risk.

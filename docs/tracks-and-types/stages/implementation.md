---
index: true
---
# Implementation Stage

## Overview

The Implementation stage transforms the approved design into working system elements, including code, scripts, configuration, and supporting components.
This stage represents the transition from design maturity to build maturity.


## Purpose

To implement, construct, and realize the system elements described in the detailed design, producing a working and testable solution.


## Artefacts

| Artefact                                                                     | Description                                                                         |
| ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| All codes and scripts checked into DET’s selected source control environment | Source code, scripts, and related assets required to build the solution or release. |
| Test Summary Report                                                          | Summary of unit, integration, system, and regression test coverage and results.     |
| Code Review Report                                                           | Results and findings from code review activities.                                   |
| Deployment Plan                                                              | Instructions and details describing how to deploy the release or solution.          |
| EIP Engagement                                                               | Details describing integration with other dependent or enabling systems.            |
| Accessibility Review Report                                                  | Results of accessibility review activities.                                         |


## Controls

* All artefacts must be updated and signed off by the relevant parties.


## Stage Processes


### Implementation Process

#### Purpose

To realize the system elements based on requirements, architecture, and design.
This process produces working system components using appropriate technologies and practices, resulting in system elements that satisfy all allocated requirements and design constraints.

Aligned with the **ISO 15288 Implementation Process**.

#### Notes

* Unit testing is a mandatory part of implementation and must occur before user acceptance testing.
* Developers are responsible for ensuring their code integrates correctly and behaves as expected.
* System Functional Testing may be performed by professional testers, but functional testing is mandatory.
* High-risk releases require 100% unit test coverage.
* Automated testing tools are encouraged and should be incorporated into build processes.
* Automated regression testing is recommended to protect system integrity.
* Code should be developed for testability; designs that expose testable interfaces are preferred.

#### Outcomes

* Implementation constraints influencing requirements, architecture, and design are identified.
* System elements are realized, packaged, or stored.
* Required enabling systems or services are available.
* Traceability from implementation to requirements and stakeholder concerns is established.
* Unit tests are generated.
* Appropriate level of rigour is applied based on release risk.

#### Artefacts

| Artefact                                          | Description                                        |
| ------------------------------------------------- | -------------------------------------------------- |
| All codes and scripts checked into source control | Source code and scripts used to build the release. |
| Test Summary Report                               | Summary of testing and results.                    |
| Deployment Plan                                   | Deployment instructions for the release.           |



### Testing Methods

#### Black-box testing

Tests system functionality without examining internal structure. Often synonymous with functional testing.

#### White-box testing

Tests internal structures, logic, and pathways (also known as structural or glass-box testing).



### Types of Testing in Systems and Software Development

#### Unit testing

Testing of individual routines or modules, performed by developers or independent testers.
Unit testability depends on good design principles such as SOLID and is supported by gated check-ins.

#### Integration testing

Testing interactions between software or hardware components to evaluate combined behaviour.
Occurs after unit testing and before system testing.

#### System testing

Testing a complete system to verify compliance with requirements. Typically performed by professional testers evaluating end-to-end behaviour.

#### Acceptance testing

Formal testing performed to determine whether the system meets acceptance criteria and whether the customer should accept it. Conducted during the Test stage.

#### Regression testing

Selective retesting to ensure changes have not introduced defects.
Commonly automated and performed during Implementation.

#### Stress testing

Testing the system beyond its expected limits to evaluate performance and stability. Normally performed during the Deployment stage.

#### Vulnerability testing

Testing for security weaknesses, sometimes referred to as penetration testing.
Typically performed during the Deployment stage.



### Integration Process

#### Purpose

To assemble implemented elements into a complete system that satisfies system requirements, architecture, and design.
This includes activating interfaces, enabling interoperation between system elements, and integrating enabling systems.

Aligned with the **ISO 15288 Integration Process**.

#### Notes

* Includes element-to-element integration within a single system.
* All system-to-system data transfers and interfaces must be managed through the Enterprise Integration Platform (EIP).

#### Outcomes

* Integration constraints are identified.
* Checkpoints for correct operation of assembled elements are defined.
* Required enabling services are available.
* Implemented elements are integrated into a complete system.
* Internal and external interfaces are validated.
* Integration results and anomalies are recorded.
* Traceability is established.
* Integration tests are generated and performed.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                                         | Description                                                       |
| ------------------------------------------------ | ----------------------------------------------------------------- |
| Enterprise Integration Platform (EIP) Engagement | Details on system integration with enabling or dependent systems. |



### Code Review Process

#### Purpose

To verify that the implemented solution aligns with design intent and adheres to architectural principles and standards.
Provides evidence that the solution conforms to DET's standards.

Aligned with the **ISO 15288 Quality Assurance Process**.

#### Notes

* Applicable only when custom code or scripts exist.
* Code reviews should enable quality, not act as a late-stage compliance check.
* Reviews support long-term maintainability (high cohesion, loose coupling, SOLID principles).
* Supported by DET’s reference systems architecture principles and patterns (TRIM 17/90097).

#### Outcomes

* Evaluations of implementation quality are performed and recorded.
* Results are provided to stakeholders.
* Incidents are recorded and resolved.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact           | Description                        |
| ------------------ | ---------------------------------- |
| Code Review Report | Results of code review activities. |



### Accessibility Review Process

#### Purpose

To assess whether the system’s user interface complies with DET’s accessibility and user-interface principles.

Aligned with the **ISO 15288 Quality Assurance Process**.

#### Notes

* Applicable only to in-house solutions with a user interface.
* Performed against an alpha release.

#### Outcomes

* Evaluations confirm conformance with accessibility requirements.
* Results are recorded and shared with stakeholders.
* Incidents are recorded and resolved.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                    | Description                              |
| --------------------------- | ---------------------------------------- |
| Accessibility Review Report | Results of the accessibility evaluation. |



### Quality Assurance Process

#### Purpose

To confirm that the release has achieved pre-production maturity and is ready for deployment.
Collects evidence that the solution meets its established requirements.

Aligned with the **ISO 15288 Quality Assurance Process**.

#### Notes

* Should enable quality and avoid unnecessarily blocking teams.
* Production readiness artefacts vary by release type.
* System testing occurs as part of this process.
* Performed against an alpha release.

#### Outcomes

* Requirements for production support are in place.
* Support teams accept responsibility for production operations.
* Production maturity evaluations are completed.
* Results are recorded and shared.
* Incidents are recorded and resolved.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                      | Description                                          |
| ----------------------------- | ---------------------------------------------------- |
| Quality Assurance Certificate | Checklist demonstrating quality gates have been met. |


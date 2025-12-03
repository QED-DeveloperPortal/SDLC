---
index: true
---
# Analysis and Design Stage

## Overview

The Analysis and Design stage transitions the solution from defined requirements into a validated system design.
Once the design reaches its maturity milestone, the desired features and operational characteristics of the solution/release are defined, documented, and accepted by business stakeholders.

This stage applies to all release categories and includes activities such as threat modelling, security and privacy by design, and the systematic development of logical and physical architecture.



## Purpose

To develop a detailed, stakeholder-supported system design based on the approved requirements, ensuring alignment with architectural principles, security expectations, and business needs.



## Artefacts

| Artefact                       | Description                                                                            |
| ------------------------------ | -------------------------------------------------------------------------------------- |
| Logical Solution Architecture  | Technology-agnostic models from relevant architectural viewpoints.                     |
| Physical Solution Architecture | Implementation-focused models from architectural viewpoints.                           |
| Design Review Report           | Confirms alignment with architectural principles, standards, and quality expectations. |



## Controls

* All artefacts produced or updated during this stage must be signed off by the relevant stakeholders.
* For high-risk releases, the Design Review Report must be approved by executives or representatives from required stakeholder groups (including external agencies if applicable).



## Stage Processes


### System Analysis Process

#### Purpose

To provide a rigorous analytical basis for technical decision-making throughout the lifecycle.
This process validates requirements, assesses alternatives, identifies risks, and analyses system behaviour using modelling, simulation, experimentation, cost analysis, quality attributes, and feasibility studies.

Aligned with **ISO 15288:2015 – System Analysis Process**.

#### Notes

* In iterative development, reassess **risk** and **information classification** whenever data models or architectural elements change.
* System analysis is used to evaluate concepts, resolve requirement conflicts, assess architecture options, and support engineering strategies.

#### Threat Modelling and Secure Systems Engineering

This stage incorporates threat modelling and security/privacy by design. Activities may include:

* Using STRIDE for threat modelling.
* Applying OWASP guidance for web-based systems.
* Referring to CAPEC for common attack pattern understanding.
* Using CWE during design/code reviews to avoid known weaknesses.
* Checking NVD entries for known vulnerabilities and planning countermeasures.
* Designing security/vulnerability testing for pipelines and automated analysis tools (e.g., static code analysis, runtime scans).

#### Outcomes

* System analysis assumptions and results are validated.
* Analysis outputs are available to support design decisions.
* Traceability to system and stakeholder requirements is established.
* Risk is reassessed.
* Information classification is updated where necessary.
* Attacks, vulnerabilities, and threats are analysed and countermeasures designed.
* Security and privacy by design principles are incorporated.
* Appropriate level of rigour is applied based on release risk.

#### Artefacts

| Artefact                                | Description                                                                   |
| --------------------------------------- | ----------------------------------------------------------------------------- |
| Updated Release Risks/Issue Register    | Captures risks and issues identified during analysis.                         |
| Updated Information Security Assessment | Documents outcomes and rationale from the information classification process. |



### Iteration Planning Process

#### Purpose

To plan, coordinate, and activate activities for a single iteration.
This includes defining objectives, identifying outputs, tasks, and artefacts, estimating resources, and organising the work required to progress the solution.

Aligned with **ISO 15288:2015 – Project Planning Process**.

#### Notes

* Helps determine which requirements or enhancements are added to the development pipeline or product/iteration backlog.
* Distinct from project-wide planning (which occurs in the Projectization and Planning Process).

#### Outcomes

* Iteration objectives and plans are defined.
* Roles, responsibilities, authorities, and accountabilities are identified where needed.
* Required resources and services are requested or committed.
* Plans for the iteration are initiated.
* Work breakdown, tasks, and backlog items are identified.



### Logical Architecture Definition Process

#### Purpose

To generate and evaluate architectural alternatives, select appropriate options, and produce an implementation-agnostic logical architecture expressed through consistent views.

Aligned with **ISO 15288:2015 – Architecture Definition Process**.

#### Notes

* Logical architecture is technology-agnostic.
  Physical architecture describes implementation-specific details.
* Additional stakeholders and concerns may be identified during architecture development.
* For COTS-based solutions, architecture focuses on integration and customisation rather than internal mechanics.
* Effective architecture uses viewpoints and models to communicate design intent to business stakeholders.
* Architecture serves decision-support, not just technical specification.

#### Outcomes

* Stakeholder concerns are addressed through architectural decisions.
* Architecture viewpoints are developed.
* System context, boundaries, and external interfaces are defined.
* Architecture views and models are produced.
* Significant concepts, behaviours, constraints, and characteristics are allocated to architectural entities.
* System elements and interfaces are identified.
* Architectural alternatives are assessed.
* Architecture provides a baseline for subsequent lifecycle processes.
* Alignment with requirements is achieved.
* Enabling services or systems are identified.
* Traceability from architecture to requirements is established.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                      | Description                                          |
| ----------------------------- | ---------------------------------------------------- |
| Logical Solution Architecture | Technology-agnostic models from relevant viewpoints. |




### Development of Architectural Viewpoints and Views

This activity aligns the architecture artefacts with **ISO 42010:2011**, ensuring strong links between stakeholder concerns and architectural decisions.

An **architecture viewpoint** defines conventions for constructing and interpreting views.
A **view** is a work product that expresses the architecture from a specific perspective.

Common viewpoint sources include:

| Source               | Common Viewpoints                                                                                                                      |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Kruchten – 4+1 Model | Logical, Development, Process, Physical, plus Scenarios                                                                                |
| Rozanski & Woods     | Functional, Information, Concurrency, Development, Deployment, Operational; Security, Performance, Availability, Resilience, Evolution |
| Clements et al.      | Module, Component & Connector, Allocation viewtypes                                                                                    |
| Eeles & Cripps       | Requirements, Functional, Deployment, Validation, Application, Infrastructure, Systems Management, Availability, Performance, Security |



### Physical Design Definition Process

#### Purpose

To define sufficient implementation-level detail for system elements so that construction and integration can proceed consistently with the logical architecture.

Aligned with **ISO 15288:2015 – Design Definition Process**.

#### Notes

* Architecture assesses suitability, viability, and desirability.
  Design determines feasibility of implementation.
* Physical design incorporates appropriate technologies and detailed design descriptions.

#### Outcomes

* Design characteristics for each system element are defined.
* Requirements are allocated to system elements.
* Design enablers are selected or defined.
* Interfaces between system elements are defined or refined.
* Design alternatives are evaluated.
* Detailed design artefacts are produced.
* Required enabling services or systems are available.
* Traceability to logical architecture is established.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact                       | Description                                                 |
| ------------------------------ | ----------------------------------------------------------- |
| Physical Solution Architecture | Implementation-focused models from architecture viewpoints. |



### Design Review Process

#### Purpose

To ensure the design meets maturity expectations, aligns with architectural principles and standards, and is accepted by business stakeholders.

Aligned with **ISO 15288:2015 – Quality Assurance Process**
and referencing **IEEE 730-2014 – Software Quality Assurance Processes**.

#### Notes

* Supported by DET’s reference systems architecture principles and patterns (TRIM 17/90097).
* Enables collection and validation of evidence showing the solution conforms to requirements.
* Reviews should ideally involve independent parties.

#### Outcomes

* Design evaluation results are recorded and consistent with architectural standards.
* Incidents and problems are documented and resolved.
* Relevant stakeholders receive evaluation results.
* Business stakeholders support and approve the design.
* Rigour is applied based on release risk.

#### Artefacts

| Artefact             | Description                                                    |
| -------------------- | -------------------------------------------------------------- |
| Design Review Report | Confirms alignment with architecture principles and standards. |


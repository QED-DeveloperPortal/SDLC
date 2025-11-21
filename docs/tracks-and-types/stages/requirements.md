

# Requirements Stage

## Overview

The **Requirements Stage** defines, refines, and validates the detailed system requirements needed to design, implement, and release a solution.
Activities in this stage progress requirements to a **maturity milestone**, often within an iteration, providing the foundation for subsequent design and development work.

Requirements represent **what** the system must do, not **how** it is implemented.


## Purpose

To specify the **formal, detailed requirements** necessary to address the business problem or opportunity identified in earlier stages.
These requirements form the baseline for design, development, testing, and release activities.


## Artefacts

| Artefact                                    | Description                                                                                          | Template |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------- | -------- |
| **System Requirements Specification (SRS)** | Captures functional, non-functional, performance, and interface requirements for the system/release. | TBA      |



## Controls

* All artefacts created or updated in this stage must be reviewed and **signed off by relevant stakeholders**.
* For high-risk releases, the SRS must be approved by **representatives from different stakeholder groups**, including external agencies where applicable, and at an **executive level**.



## Stage Processes

### System Requirements Definition Process

#### Purpose

To transform the stakeholder-oriented view of needs and intentions into a **technical, measurable** set of system requirements.
This process defines system capabilities, behaviours, boundaries, performance expectations, and constraints.

Aligned with **ISO 15288:2015 – System Requirements Definition Process**.

#### Key Notes

* Requirements focus on **WHAT** the system must achieve.
  Design focuses on **HOW** it achieves it.
* Initial stakeholder intentions (needs, goals, objectives) are **not** requirements until refined, analysed, and validated.
* Use **Concept of Operations (ConOps)** and **System Operational Concept** documents to support understanding.

#### A well-formed requirement:

* Is **verifiable**
* Must be **met by the system**
* Is **measurable** and **bounded by constraints**
* Describes **system performance or capability**, not user capability
* Distinguishes between *requirements* and their *attributes* (assumptions, constraints, design decisions, conditions)

#### Security Requirements Gathering

Security requirements must be identified early and informed by the **Preliminary Information Classification Process**.
These requirements establish inputs for threat modelling during the Analysis & Design stage.

#### Outcomes

* System description, boundaries, functions, and interfaces are defined
* Functional, non-functional, performance, and interface requirements are captured
* Critical performance measures are identified
* Requirements are analysed and validated
* Enabling systems/services are identified
* Requirements traceability to stakeholder requirements is established
* Levels of rigour are applied based on **risk level** of the release

#### Artefacts

| Artefact                                    | Description                                      |
| ------------------------------------------- | ------------------------------------------------ |
| **System Requirements Specification (SRS)** | Primary output including all system requirements |

---

### Demonstration and Evaluation Process

#### Purpose

To refine system characteristics, concepts, and requirements through **prototyping, user engagement**, and early solution exploration activities.

Teams may use this process at their discretion, though it is common practice in some areas—especially when evolving Business Requirements Specifications or validating UI/UX concepts.

Aligned with **ISO 15288:2015 – System Requirements Definition Process**.

#### Outcomes

* Business stakeholders are actively engaged
* System concepts and characteristics are refined
* Requirements gain clarity and depth
* Confidence increases that needs are understood and addressed
* Business Requirements Specification is finalized and signed off
* Levels of rigour applied based on **release risk**

#### Artefacts

| Artefact                                        | Description                                           |
| ----------------------------------------------- | ----------------------------------------------------- |
| **System Requirements Specification (refined)** | Updated with insights from prototyping and evaluation |

---

### Infrastructure Provisioning Process

#### Purpose

To define, acquire, and provision the infrastructure and services required to support the project, system, or release.
This includes environments, tools, facilities, and ICT assets needed throughout the lifecycle.

Aligned with **ISO 15288:2015 – Infrastructure Management Process**.

#### Outcomes

* Infrastructure requirements are defined
* Infrastructure components are identified and specified
* Infrastructure assets are acquired or developed
* Infrastructure is made available to support development and testing
* Levels of rigour are applied based on **release risk**
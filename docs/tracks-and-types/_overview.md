---
index: true
---
# Tracks review

An **SDLC Track** represents a traversal through the stages of the Software Development Life Cycle (SDLC) with the goal of producing a **production release**.
Each track defines a typical path through the lifecycle — starting and ending at specific stages — based on the **scope, size, and type of release** being delivered.

As shown in *Figure 6 – SDLC Conceptual Reference Model* and *Figure 7 – SDLC Overview*, a track acts as a **process view** of the SDLC: it describes how stages, controls, artefacts, and governance activities are applied for a specific type of release.


## Purpose of tracks
* To provide a structured but adaptable path through the SDLC.
* To define which **stages, artefacts, and controls** apply to each release type.
* To guide development teams in selecting the **right level of governance and documentation** for their work.
* To ensure consistency, traceability, and alignment across projects and product releases.

Each SDLC Track corresponds to a **release scope type** — such as Major, Minor, or Maintenance — and can be mapped to business-area terminology (e.g. Projects, Enhancements, Patches).


## Track types
Currently there are **three core SDLC tracks**, representing different scales and complexities of delivery.

### Type 1 Release Track – Major / Project Releases
Covers **large-scale or project-based releases** (often labelled *Major Releases* or *Projects*).
* **Start:** *Needs Stage*
* **End:** *Maintenance Stage*
* **Notes:** Requires full progression through all stages and artefacts.
  Transition and Validation processes within the *Deployment Stage* are **mandatory** to ensure benefits are realised post-release.
  *(See Figure 8 – SDLC Stages in a Type 1 Release Track.)*

### Type 2 Release Track – Minor / Significant Releases
Covers **moderate releases** that extend or enhance existing systems without major rework.
* **Start:** *Requirements Stage*
* **End:** *Maintenance Stage*
* **Notes:** Suitable for enhancements and functional upgrades where existing architecture and design largely remain valid.
  *(See Figure 9 – SDLC Stages in a Type 2 Release Track.)*


### Type 3 Release Track – Maintenance / Fix Releases
Covers **maintenance and corrective releases** (also known as *Bug Fix*, *Ad-hoc*, or *Emergency* releases).
* **Start:** *Analysis and Design Stage*
* **End:** *Maintenance Stage*
* **Notes:**
  * Focuses on fixing defects or ensuring requirements are properly fulfilled.
  * No new requirements are introduced.
  * May include design adjustments if necessary to resolve persistent issues.
  * In practice, most fixes begin in the *Implementation Stage*, though *Analysis and Design* may be revisited if deeper changes are required.


## Relationship to SDLC Stages and Processes
Each SDLC track draws upon the same foundational stages, controls, and artefacts — but applies them **proportionally to the release type**.
For example:

* A Type 1 (Major) release includes **all stages** and **full governance controls**.
* A Type 3 (Maintenance) release includes **only essential processes**, focusing on quality, traceability, and rapid resolution.
Additional **track-specific processes** may also apply at the beginning of each development activity — for example, risk assessment, classification, or release planning.


## Summary

| Track Type | Typical Scope       | Start Stage       | End Stage   | Typical Use                                   |
| ---------- | ------------------- | ----------------- | ----------- | --------------------------------------------- |
| **Type 1** | Major / Project     | Needs             | Maintenance | Full project delivery or new solution         |
| **Type 2** | Minor / Significant | Requirements      | Maintenance | Enhancement or extension of existing solution |
| **Type 3** | Maintenance / Fix   | Analysis & Design | Maintenance | Corrective or patch release                   |


> **Note:** Each SDLC Track provides a *view of the entire SDLC* tailored for the release type.
> It ensures that each release — regardless of scale — maintains appropriate quality, governance, and traceability while remaining efficient and adaptable.

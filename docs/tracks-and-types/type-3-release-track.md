---
index: true
---
# Type 3 Release Track

## Overview

The Type 3 Release Track applies to small, corrective, or maintenance-focused releases.
Depending on the business area, Type 3 releases may correspond to:

* **Maintenance / Bug Fix releases** (e.g., Information & Technologies, Human Resources)
* **Minor, Emergency, or Adhoc releases** (e.g., Finance Branch)

These releases address defects, operational issues, or minor adjustments but do not introduce new requirements.


## Stages Covered

Type 3 releases begin at the **Analysis and Design** stage and continue through to **Maintenance**.
They include the following stages:

* Analysis and Design
* Implementation
* Test
* Deployment
* Maintenance

This allows sufficient scope to analyse underlying issues, adjust design elements if necessary, implement corrective changes, validate functionality, and return the system to a stable operational state.



## Special Considerations

### Requirements Do Not Change

A key principle of the Type 3 Release Track:

* **No new requirements are introduced.**
* The goal is to **fix issues, resolve defects, address operational problems**, and ensure existing requirements are fulfilled correctly.

This distinguishes Type 3 releases from Type 2 enhancements or Type 1 major changes.



### Practical Starting Point

While Type 3 work often begins directly in Implementation (e.g., a simple code fix), some situations require earlier-stage activities:

* If the issue originates in system design, a design adjustment may be required.
* For issues related to data integrity, persistence layers, or architectural constraints, the **System Analysis Process** may be revisited.
* Iteration Planning remains relevant where multiple fixes must be organised and prioritised.

For this reason, Type 3 releases formally begin at **Analysis and Design**, even though many smaller fixes may naturally start later.



## Notes

* If no design changes are needed, some processes in the Analysis and Design stage may be skipped, while still ensuring sufficient rigour is applied based on release risk.
* Processes such as *System Analysis* and *Iteration Planning* may still apply even for minor maintenance updates.
* Type 3 releases are typically fast-path, low-risk updates but must still follow the appropriate artefacts and controls for the included stages.


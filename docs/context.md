
This document supplements the SDLC by providing practical guidance, clarifications, and examples to help teams understand and apply the framework in real terms. It bridges policy and practice—covering common questions, helpful tips, and emerging approaches across all stages of delivery.

---


# **Compliance in Agile: Transitioning from Waterfall to Iterative Methods**

Many of the Department’s current compliance controls were originally designed to support **Waterfall-style projects**—where large, sequential stages lead to a final release.
As we evolve towards **Agile**, **Spiral**, and **Product Operating Models**, our goal is not to discard compliance but to **adapt** it—making assurance activities **lighter, continuous, and embedded** into everyday delivery.

The Department is progressively modernising these artefacts to align with iterative development, automation, and contemporary DevSecOps practices.
Where possible, traditional deliverables should be met through **incremental evidence** produced naturally during sprints, releases, and continuous integration.


## **1. Information Security Assessment (ISA)**

**Purpose:** Ensures information assets are appropriately managed for security, privacy, and classification.
**Legacy expectation:** Conducted once prior to production release.
**Iterative alignment:**

* Embed security and privacy reviews **throughout delivery** rather than waiting for end-stage assessment.
* Perform a **Privacy Threshold Assessment (PTA)** early to determine if a full ISA is needed.
* Track risks and mitigations within each sprint’s backlog or Azure DevOps board.
  **Modernisation direction:** Move toward **automated security scanning**, **reusable patterns**, and **lightweight reassessment** triggered only by major changes in data sensitivity or architecture.


## **2. Cloud Assessment Report (CAR)**

To modernise the approach to satisfying Cloud Assessment Report (CAR) requirements within the QED Software Development Life Cycle (SDLC), organisations must shift from manual, siloed reviews to automated, integrated governance embedded within DevOps and Infrastructure-as-Code (IaC) pipelines. The legacy model — where a static CAR document was manually prepared, reviewed by Architecture and Security teams, and approved prior to deployment — introduced delays, inconsistency, and risk of human error. Modernisation transforms this into a proactive, scalable, and compliance-by-design process aligned with cloud-native principles.

The cornerstone of this transformation is the adoption of approved Azure Landing Zones and standardised, pre-vetted deployment templates. These artefacts encapsulate organisational security controls, network architecture, identity management, logging, and compliance policies (e.g., CIS benchmarks, NIST controls) in reusable, version-controlled IaC modules (e.g., Terraform, Bicep). By mandating their use for all cloud-hosted components, teams inherently satisfy foundational CAR requirements such as secure network segmentation, encryption at rest and in transit, and role-based access control (RBAC). This eliminates the need for post-hoc validation of basic configurations, reducing review burden and accelerating delivery.

For non-standard or custom architectures — particularly those involving data sovereignty constraints, offshore storage, or hybrid cloud patterns — early engagement with the Governance and Business Nexus (GBN) is critical. Modernisation does not eliminate oversight; it refocuses it. Instead of waiting until the CAR is drafted, teams must trigger automated compliance checks during the design phase. This can be achieved by integrating policy-as-code tools like Azure Policy, Open Policy Agent (OPA), or Checkov into the IaC pipeline. These tools evaluate infrastructure configurations against a centralised policy registry before deployment, flagging deviations in real time. If a proposed architecture breaches data residency rules or lacks required encryption standards, the pipeline fails immediately — prompting early collaboration with GBN and Information Security teams.

Integration of CAR validation into architecture review gates further strengthens governance. Rather than treating the CAR as a final checkpoint, its criteria should be embedded into every stage of the SDLC. For example, during the Concept and Requirements stages, teams must document cloud suitability decisions using the Preliminary Cloud Assessment Process (as defined in DET’s SDLC), ensuring alignment with cloud suitability criteria. During the Design stage, Logical and Physical Solution Architectures must explicitly reference approved Landing Zones and justify deviations. Automated tools can then validate that these artefacts are present, linked to IaC templates, and comply with classification requirements.

Additionally, the CAR itself can evolve from a static document to a dynamic, auto-generated report. By leveraging CI/CD pipelines and configuration management databases (CMDBs), metadata from deployed resources — including compliance scan results, access logs, and classification tags — can be aggregated into a real-time CAR dashboard. This provides auditors and reviewers with live visibility, reducing reliance on outdated PDFs.

Ultimately, modernising the CAR process is not about replacing people with automation — it’s about empowering teams with guardrails that make compliance inevitable, not optional. By embedding CAR requirements into IaC, automating validation at every gate, and enforcing early GBN engagement for complex cases, QED organisations achieve faster, more secure cloud deployments without compromising governance. This transforms the CAR from a compliance hurdle into an enabler of innovation.

**Old Content**

**Purpose:** Confirms compliance for cloud-hosted components.
**Legacy expectation:** Manual report reviewed by Architecture and Security prior to deployment.
**Iterative alignment:**

* Use **approved Azure Landing Zones** and reference **standard deployment templates** to satisfy cloud compliance.
* For new or non-standard patterns, seek **GBN approval** early (particularly where data sovereignty or offshore storage is involved).
  **Modernisation direction:** Integrate CAR validation into **Infrastructure-as-Code pipelines** and **architecture review gates**.


## **3. Release Risk & Issue Register**

SDLC Type 1 projects often follow a waterfall methodology.

The SDLC focuses on 'What' is required for release management. There are however modern alternative approaches to waterfall for 'How' to implement release management.

These include Agile, Spiral and Product Operating Model. 

Traditionally Release Risk has been maintained as a static document.

To achieve iterative alignment, risk and issue management should be treated as a **living process** that is tracked within sprint boards, retrospectives, and product dashboards.

To foster a more modern approach for release management in SDLC Type 1 projects, consider incorporating the following approaches in your implementation strategy:

### Embrace iterative development
  * Break down the project into smaller, manageable increments. This allows for regular feedback and adjustments, rather than waiting until the end of the project to  assess progress.

### Incorporate Agile practices
  * Integrate Agile methodologies, such as Scrum or Kanban, into the release management process. This can involve daily stand-ups, sprint planning, and retrospectives to foster collaboration and continuous improvement.

### Enhance collaboration
  * Encourage cross-functional team collaboration, ensuring that all stakeholders (developers, testers, project managers) are involved in the planning and execution phases. This helps in identifying issues early and allows for quicker resolution.

### Implement continuous integration and delivery (CI/CD)
  * Adopt CI/CD practices to automate testing and deployment processes. This reduces manual errors and accelerates the release cycle, enabling more frequent updates and faster delivery of features.

### Use feature toggles
  * Implement feature toggles to allow incomplete features to be merged into the main codebase without affecting production. This enables teams to work on multiple features simultaneously while maintaining system stability.

### Use only synthetic data
  * Only use synthetic data that does not identify with any real world people or places. As a starting point to achieve this, you could use data generated by the DevPortal DataForge facility.

### Use mock APIs
  * DevPortal has numerous mock APIs that match the input interfaces and output data types of production grade APIs without any contact with any internally managed system. You can find these via the APIs menu on the DevPortal home page.

### Focus on documentation and traceability
  * Maintain clear documentation and version control throughout the development process. This ensures that all changes are tracked and can be easily reviewed, facilitating smoother transitions between phases.

### Regularly review and adapt
  * Conduct regular reviews of the development process to identify bottlenecks and areas for improvement. Adapt the approach based on feedback from the team and stakeholders to ensure that the process remains efficient and effective.

By incorporating these strategies, Type 1 projects can benefit from a more agile approach to release management while still adhering to the necessary constraints of the waterfall model. This balance can lead to improved delivery timelines and increased stakeholder satisfaction.

Type 2 and Type 3 projects will find it easier to adopt practices that Agile, Spiral or Product Operating Model espouse.

These strategies align with the principles of the Software Development Life Cycle (SDLC) and aim to enhance the overall quality and efficiency of the development process.

**Old Content**

**Purpose:** Documents and manages risks throughout the project lifecycle.
**Legacy expectation:** Maintained as a static document.
**Iterative alignment:**
* Treat risk and issue management as a **living process**—tracked within sprint boards, retrospectives, and product dashboards.
* Encourage teams to identify, mitigate, and close risks continuously rather than at the end of the release.
  **Modernisation direction:** Link risk artefacts directly to **work items**, **user stories**, and **automated test coverage reports** for traceability.



## **4. Acceptance Test Summary Report (ATSR)**


To modernise the approach to satisfying Acceptance Test Summary Report (ATSR) requirements in the QED SDLC, organisations must move beyond static, post-phase documentation toward continuous, evidence-based validation embedded in the delivery pipeline. The legacy model — a manually compiled ATSR after testing concludes — is slow, siloed, and prone to lag between actual system behaviour and reported outcomes. Modernisation replaces this with real-time, automated evidence collected throughout each sprint.

The Definition of Done (DoD) becomes the foundational anchor: acceptance criteria are no longer abstract requirements but machine-verifiable conditions encoded into test cases. Automated unit, integration, and end-to-end tests — orchestrated via Azure DevOps pipelines — execute with every code commit. Pass/fail results, coverage metrics, and user scenario outcomes are logged automatically, creating an immutable audit trail. Instead of waiting for a final report, stakeholders view live dashboards showing test progress, pass rates, and regression trends — turning the ATSR from a document into a dynamic status indicator.

Sprint reviews and release gates now rely on this aggregated evidence. A “passing” ATSR is no longer a deliverable but an emergent property of consistent test success. For example, if 100% of user acceptance scenarios pass in the last three sprints with zero critical regressions, the system is deemed accepted — no formal report needed. Where manual UAT is still required (e.g., usability or compliance), results are captured directly in Azure Test Plans and linked to user stories, ensuring traceability.

This shift reduces administrative overhead, eliminates last-minute surprises, and aligns with Agile principles. The ATSR is no longer a checkpoint — it’s a continuous assurance signal, validated by automation, visible to all, and trusted by stakeholders. Compliance is proven through action, not paperwork.

**Old Content**

**Purpose:** Demonstrates that functionality meets user and business requirements.
**Legacy expectation:** Formal report completed after testing phase.
**Iterative alignment:**

* Replace standalone reports with **continuous test evidence**—Azure DevOps test plans, automated regression logs, or sprint review outcomes.
* Consider the **Definition of Done (DoD)** as the natural home for acceptance criteria.
  **Modernisation direction:** Encourage **automated test pipelines** and dashboards as proof of compliance.



## **5. Quality Assurance Certificates**

To modernise the Quality Assurance Certificate (QAC) process within the QED SDLC, organisations must transition from a final-stage, manual sign-off to a continuous, automated evidence chain embedded in every sprint. The legacy model — where a static QAC was compiled at cycle end, often as a last-minute checklist — created bottlenecks and delayed detection of non-compliance with Departmental standards for quality, accessibility (WCAG 2.x), and usability (CUE).

Modernisation embeds QA into the Definition of Done (DoD): every user story must pass automated accessibility scans (e.g., Axe, Lighthouse), code linting for maintainability, and UX consistency checks before being marked “done.” These tools run automatically in CI/CD pipelines (e.g., Azure DevOps), generating real-time compliance metrics. For example, a build fails if contrast ratios fall below WCAG AA thresholds or if ARIA labels are missing — enforcing accessibility by design, not after the fact.

Branding and UX checks are integrated into design review gates via Figma plugins or automated visual regression tools that compare UI changes against approved style guides. Non-compliant components are flagged before code even reaches development.

Instead of a single end-of-cycle certificate, compliance is demonstrated through a live dashboard aggregating test results, accessibility scores, code quality metrics (SonarQube), and design audit logs. This dynamic “living QAC” provides auditors and stakeholders with transparent, timestamped proof that quality standards were met continuously — not just at a checkpoint.

The result: reduced rework, faster approvals, and true compliance-by-design. The QAC evolves from a ceremonial document into an automated assurance signal — proving quality isn’t checked at the finish line, but built in from the first commit.

** Old Content**

**Purpose:** Validates that software meets Departmental standards for quality, accessibility, and usability.
**Legacy expectation:** Certificates provided at the end of the development cycle.
**Iterative alignment:**

* Incorporate QA activities directly into each sprint’s DoD.
* Use **automated linting and accessibility tools** to support WCAG 2.x and Common User Environment (CUE) compliance.
* Apply **branding and UX checks** as part of design review gates.
  **Modernisation direction:** Move from static sign-offs to **continuous compliance evidence** across sprints.



## **6. Production Readiness Certificate (PRC)**

To modernise the Production Readiness Certificate (PRC) process within the QED SDLC, organisations must shift from monolithic, end-of-project documentation to lightweight, risk-driven, and continuously validated “Certificate Tickets” (CTs) tied to individual features or changes. The legacy model — a bulky, manually compiled PRC required before every go-live — created delays, duplicated effort, and treated all deployments as high-risk, regardless of scope.

Modernisation introduces a tiered, intelligent approach: for established products with stable infrastructure and proven operational controls, only new or high-risk components (e.g., data schema changes, third-party integrations, security-sensitive modules) require a CT. Incremental updates to existing features — such as UI tweaks or non-critical bug fixes — are deemed ready by automated health checks and historical performance data, eliminating redundant reviews.

For entirely new products, a full PRC is conducted once during initial launch. Subsequent releases then rely on automated, continuous readiness signals: infrastructure-as-code compliance (via Azure Policy), monitoring dashboards (e.g., Azure Monitor, Application Insights), automated rollback triggers, and operational runbook validation. These form the “living PRC” — a real-time assurance that the system remains production-ready.

Each CT is tracked as a ticket in Azure DevOps, linked to the change request, with automated evidence attached: test pass rates, security scan results, backup validation logs, and support handover confirmation. Approval workflows are streamlined — low-risk CTs auto-approve if all criteria are met; high-risk ones trigger targeted reviews by Architecture or Ops.

This transforms the PRC from a bottleneck into an agile, scalable governance layer. Risk is assessed dynamically, compliance is proven continuously, and teams ship faster — with confidence that production readiness isn’t a milestone, but a condition maintained every day.

**Old Content**

**Purpose:** Verifies that a product or service is ready for production deployment.
**Legacy expectation:** Large, end-of-project artefact required before go-live.
**Iterative alignment:**

* For **existing products** or **incremental features**, only new or high-risk components should require a PRC.
* For **new products**, perform a full PRC once, then manage ongoing readiness through automated checks.
  **Modernisation direction:** Transition toward **Certificate Tickets (CTs)**—lightweight, risk-based approvals that can be tracked per feature or change.


## **7. Change Management**

**Purpose:** Controls how updates are deployed into production environments.
**Legacy expectation:** Manual approval process focused on major releases.
**Iterative alignment:**

* The Department is reviewing its change management approach to support **Agile and CI/CD** pipelines.
* The intent is to enable **seamless, low-risk delivery** using automated testing, peer reviews, and environment gates.
  **Modernisation direction:** Shift from “change approval” to **change visibility and assurance**, supported by telemetry, audit trails, and release automation.


### **Summary**

The overarching principle is **continuous compliance**—building quality and assurance into every step of delivery, rather than applying it as a final gate.
Each traditional artefact should evolve from a **document** into an **automated, iterative control**, aligned with real-time feedback and observable evidence from modern development tools.

---

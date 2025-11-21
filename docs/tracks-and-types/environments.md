# Environments

Throughout the SDLC, different **controlled environments** are used to build, distribute, configure, test, and execute solutions as they progress through each stage of the lifecycle.
Each environment serves a distinct purpose and supports a specific phase of delivery, ensuring that systems are developed, tested, and deployed safely and predictably.

*(See Table 8 – Environments used throughout the SDLC.)*



## **Environment Overview**

| **Environment**                                                     | **Description**                                                                                                                                                                                                                                                  |
| ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Zone 1 – Development**                                            | Used by developers to create, test, and validate code, scripts, and configurations. This environment supports early integration and unit testing, and is where the **Alpha** version of a release is typically deployed.                                         |
| **Zone 2 – User Acceptance Testing (UAT) / Quality Assurance (QA)** | Used by business representatives and stakeholders to test solutions against original business requirements. It supports system, regression, and acceptance testing, and is where the **Beta** version of a release is deployed.                                  |
| **MPE – Mirrored Production Environment / Staging**                 | Used by deployment and release teams to verify deployment packages prior to production. Ideally this environment mirrors production exactly, acting as a **staging** or **pre-production** environment. The **Candidate** version of a release is deployed here. |
| **Production**                                                      | The live environment where solutions are deployed for final use by end users. Production represents the authoritative operational system of record.                                                                                                              |
| **Training**                                                        | Used by business stakeholders, support staff, and developers for training and familiarisation activities. May contain anonymised or synthetic data to replicate production behaviour safely.                                                                     |
| **Disaster Recovery (DR)**                                          | A standby environment used to maintain business continuity in the event of a system or infrastructure failure. DR environments should mirror production configurations and be validated regularly.                                                               |


* Each environment is **purpose-built** and **controlled**, with defined entry and exit criteria.
* Movement between environments follows **change and release management processes**.
* Configuration management, data integrity, and security controls must be maintained consistently across all environments.
* Naming conventions (e.g., Zone 1, Zone 2, MPE) may vary by branch, but the functional intent remains the same.
* Continuous integration and continuous delivery (CI/CD) pipelines can automate progression through these environments while maintaining the same control checkpoints.


## On-Premise vs Cloud environments
Traditionally, these environments are hosted within on-premise infrastructure, where each zone is provisioned and managed as a separate physical or virtual instance.
While this model remains common across departmental systems, cloud platforms provide alternative approaches to environment management that achieve the same control objectives through different means.

Modern cloud-based solutions often use:
- Source repositories and branching strategies to manage configuration and release isolation.
- Containerisation (e.g. Docker, Kubernetes) to replicate environments consistently across stages.
- Landing zones, virtual networks, or subscriptions to segregate environments securely.
- Infrastructure-as-Code (IaC) to automate environment setup, teardown, and governance controls.

These approaches provide greater flexibility, scalability, and repeatability, but they must still align to the intent of the SDLC environment model — ensuring every release passes through controlled, traceable validation stages before reaching production.



Aligning environment usage with SDLC stages helps ensure repeatable, auditable, and reliable releases. Each environment forms a safeguard layer in the overall quality-assurance process.



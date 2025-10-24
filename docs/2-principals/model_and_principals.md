# Model and Principles
*These principles guide the application of the SDLC across all projects and methodologies.*


## Release Readiness Must Match Risk
**Principle:**
All releases must meet defined *acceptability criteria* and *quality metrics* aligned with their risk level.
**Why it matters:**
Risk-based governance ensures proportional effort. High-risk releases require more checks (e.g. approvals, testing coverage) than low-risk ones.
**Implications:**
Tools may need configuration or support to calculate certain metrics. Manual steps may be required initially to ensure visibility.


## Stage Controls Support Iteration, Not Just Sequence
**Principle:**
Each SDLC stage includes defined controls. These must be fulfilled before progress is recognised—but this doesn’t imply strict sequential flow.
**Why it matters:**
Supports both **iterative** and **linear** development. Re-entering stages (e.g. updating documentation after refactor) is natural and expected.
**Implications:**
Some artefacts may not change every release but should still be reviewed for relevance. Maturity is reflected through ongoing alignment, not a checkbox approach.


## Flexibility in Tools and Artefacts – Outcomes Matter Most
**Principle:**
Teams may tailor artefact templates or use tools that suit their ways of working—as long as they still achieve all required **outcomes**.
**Why it matters:**
Supports Agile, DevOps, and modern lightweight delivery approaches, while preserving **governance and traceability**.
**Implications:**
Documentation can take many forms—code comments, pipeline logs, structured markdown, etc.—so long as it meets outcomes and provides clarity if needed later.


## Traceability Through Versioning
**Principle:**
All SDLC artefacts must be traceable to their corresponding release or iteration, using either traditional versioning or modern automated methods.
**Why it matters:**
Traceability ensures transparency and accountability. Teams may use commits, pull request IDs, build numbers, or sprint tags instead of manual versioning provided they clearly link artefacts to specific changes or releases.
**Implications:**
Automation is preferred where possible. Teams must ensure consistent version tracking such as system-generated ids, tags or links as valid evidence.


## Highest Risk Governs the Bundle
**Principle:**
When bundling changes for a release, the highest risk item determines the governance level for the whole bundle.
**Why it matters:**
Bundling is practical—but mixing high and low-risk changes without proper governance can lead to oversight or failure to comply with assurance standards.
**Implications:**
Avoid mixing significantly different risk levels in the same release unless additional governance is applied.


## Risk is Reassessed During Iteration
**Principle:**
Each new iteration may introduce new risks—these must be identified and managed **continuously**, not just up-front.
**Why it matters:**
Modern delivery methods (e.g. Agile sprints, CI/CD) evolve over time. Treating risk as static can result in blind spots.
**Implications:**
Time and resourcing must account for reclassification, especially where risk changes require new controls or approvals.


## Information Classification Evolves Too
**Principle:**
Classification of data must be reviewed when changes affect data models or data use—even mid-project.
**Why it matters:**
What starts as “low sensitivity” may evolve to include personally identifiable information (PII) or sensitive student data. We must adapt.
**Implications:**
Reclassification can affect schedules and delivery. Teams must build this flexibility into planning cycles.



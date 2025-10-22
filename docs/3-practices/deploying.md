## Deploying
*Moving working software into the hands of users—safely, confidently, and often.*
* Makes improvements real—delivery isn’t done until it’s in production
* Encourages **frequent, low-risk releases** instead of high-stakes big-bangs
* Uses **automated pipelines**, feature flags, and progressive rollouts to reduce risk
* Builds **trust in process** through transparency, observability, and rollback readiness
* Streamlines approvals while still upholding quality and oversight


### Desired outcomes vs Anti-patterns
*Desired outcomes:*
* Small, incremental releases that are easy to review, test, and roll back
* Automated deployment pipelines with built-in quality checks
* Environments managed consistently across dev, test, and prod
* Transparent release notes, audit trails, and changelogs
* Approvals that are proportional to risk—not size or ceremony

*Anti-patterns:*
* Delayed deployments due to excessive paperwork and handoffs
* “Production readiness” treated as a static document, not a dynamic state
* Risk increasing with size and frequency of releases
* Environments that drift from each other or require manual workarounds
* Relying on heroics or after-hours “go-lives” to push changes


### When we do it
* Continuously, using automation and triggers (e.g. CI/CD pipeline)
* After a change is tested and approved via pull request or automated checks
* In response to feedback, user need, or hotfixes
* As a learning tool—observing real usage and outcomes
* Even during discovery (via feature flags, internal betas, etc.)


### Tools & Techniques
* CI/CD platforms (e.g. Azure DevOps, GitHub Actions, GitLab, Jenkins)
* Blue/green deployments, canary releases, and rolling updates
* Feature flags and toggles for controlled rollouts
* Deployment dashboards and logs with real-time visibility
* Auto-generated changelogs and release notes
* Infrastructure as code (IaC) and environment consistency tooling
* Automated PR checks, readiness tickets, or policy gates
* Beta programs or internal dogfooding environments
* Lightweight “Certificate Ticket” models replacing heavy PRC docs


### Practice in Action

**“Instead of one large release per quarter, the team moved to weekly deployments using automated pipelines. Each deployment included just a few changes, behind feature flags. Release approvals were based on lightweight risk-assessed 'certificate tickets' tied to automated tests and monitoring. Issues were rare, fast to fix, and entirely visible to stakeholders.”**
— DevOps-enabled team using **CI/CD**, **Feature Flags**, and **Governance-as-Code**



## How to Deploy Safely
Modern deployment isn’t about avoiding risk—it’s about containing and managing it.
When we rely on heavy, infrequent, big-bang releases, the risk grows with each change.
Smaller, more frequent, observable releases—backed by automation and progressive rollout—are safer and more recoverable.

*Common challenges*
- Too many zones create confusion, maintenance burden, and drift
- MPE environments don’t reflect real production use, so issues slip through
- On-prem vs cloud split leads to inconsistent tooling and deployment processes
- Manual deployment or release-by-email increases human error
- Production readiness is treated as a document, not a state

### Safer Deployment Strategies
Feature Flags	- Toggle features on/off without changing code. Allows “shipping dark.”	Deploy incomplete or experimental features safely
Canary Releases - Release to a small % of users first, monitor, then roll out more.	Catch issues early with real usage and rollback control
Blue/Green Deploys - Two mirrored environments. Switch traffic when new version is ready.	Near-zero downtime deployments with instant rollback option
Beta Programs	- Release to invited users (internal/external) for feedback before full launch	Validate functionality and UX before wide release
Feature Branch Deploys - Deploy directly from a feature branch to a non-prod env with full automation	Validate changes in isolation with stakeholder feedback
Dark Launching - Deploy features fully, but hide them behind conditions or flags	Test performance, data flow, or analytics before revealing

*Incremental Change, Not Big Bang*
Safe deployment isn’t about more process. It’s about smarter release architecture.
By embracing these strategies, we reduce pressure on environments like MPE and make deployments faster, safer, and more transparent—for users, devs, testers, and stakeholders alike.


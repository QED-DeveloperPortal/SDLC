# Testing
*Building confidence by embedding quality into everything we do.*
* Ensures we’re delivering safe, usable, accessible, and reliable software
* Catches issues early—when they’re easier and cheaper to fix
* Supports faster delivery by making quality visible and actionable
* Empowers teams to test continuously—not just at the end
* Builds trust in the product, the process, and the team


### Desired outcomes vs Anti-patterns
**Desired outcomes:**
* Automated and manual tests aligned to real user scenarios
* Fast, reliable feedback loops built into the CI/CD pipeline
* Accessibility, security, and performance tested as part of delivery
* Shared responsibility for quality—devs, testers, and designers collaborating
* Testing seen as a learning and risk-reduction activity
**Anti-patterns:**
* Testing left to the end of the project or sprint
* Manual test cases with no automation or reuse
* QA isolated from design, development, and delivery
* Tests focused on “does it work” but ignoring “does it make sense”
* Relying on users or production feedback as the main safety net


### When we do it
* From day one—starting with testable designs and stories
* During development using TDD, unit tests, and integration checks
* At the point of merge or deployment through CI/CD
* Post-release using synthetic monitoring or user analytics
* Any time we need confidence that what we’re building is fit for purpose


### Tools & Techniques
* Unit, integration, and end-to-end (E2E) automated testing
* Test-driven development (TDD) or behaviour-driven development (BDD)
* Manual exploratory testing and usability testing
* Accessibility audits (e.g. axe, WAVE)
* Security testing (e.g. dependency scans, penetration tests)
* Performance and load testing tools (e.g. JMeter, k6)
* CI/CD pipelines with automated test stages
* Feature flags for safe testing in production
* Session-based test management
* Testing personas and real-device testing (e.g. BrowserStack, mobile labs)


### Practice in Action
**“Rather than waiting for the QA cycle, the team wrote test cases alongside their stories. Developers created unit and integration tests in parallel with code. Testers joined refinement sessions and used exploratory testing mid-sprint. Bugs were caught early, risks were surfaced fast, and the team released with confidence—every week.”**
— Cross-functional team using **TDD**, **Exploratory Testing**, and **CI-integrated QA**


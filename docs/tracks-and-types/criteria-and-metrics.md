# Release Acceptability Criteria and Quality Metrics

## Overview

Release readiness is assessed across two complementary dimensions:

* **Release Acceptability Criteria**
  *Extrinsic checks* that confirm governance, approvals, and scope alignment.

* **Release Acceptability Quality Metrics**
  *Intrinsic checks* that measure the quality and robustness of the implemented solution.

Together, these ensure that a release is production-ready and satisfies the correct level of rigour appropriate to its calculated **Release Risk Impact Level** (e.g., Low or High).

A release is considered ready only when:

* all acceptability criteria for its risk level are fulfilled
* all quality metrics fall within the acceptable thresholds for that risk level

This aligns release readiness with DET’s risk-based approach and ensures consistent governance, quality, and assurance practices.



## Acceptability Criteria

The following tables list the governance and approval requirements based on release risk impact level.

### High-Risk Releases

| Acceptability Criteria                                                                         |
| ---------------------------------------------------------------------------------------------- |
| Application governance board approval for bug fixes                                            |
| Application governance board approval for changes of scope                                     |
| Application governance board approval of production readiness for all release scope types      |
| Application governance board approval for all requirements included in all release scope types |



### Low-Risk Releases

| Acceptability Criteria                                                                         |
| ---------------------------------------------------------------------------------------------- |
| Application governance board approval for change of scope for Major and Minor releases         |
| Application governance board approval of production readiness for such releases                |
| Application governance board approval for all requirements included in all release scope types |



## Acceptability Quality Metrics

### High-Risk Releases

| Metric                        | Minimum Threshold      | Maximum Threshold      |
| ----------------------------- | ---------------------- | ---------------------- |
| Unit test coverage            | 65%                    | 100%                   |
| User acceptance test coverage | 180% (performed twice) | 200% (performed twice) |
| Regression test coverage      | 75%                    | 100%                   |



### Low-Risk Releases

| Metric                        | Minimum Threshold | Maximum Threshold |
| ----------------------------- | ----------------- | ----------------- |
| Unit test coverage            | 45%               | 64.99%            |
| User acceptance test coverage | 90%               | 100%              |
| Regression test coverage      | 30%               | 74.99%            |



## Notes

* Any software quality metric from established models (e.g., ISO quality in use, ISO product quality model) may be used to further refine release rigor.
* These criteria support DET’s risk-stratified governance approach, ensuring that high-risk releases undergo deeper scrutiny and higher quality requirements.
* Metrics such as performance benchmarks, accessibility scores, vulnerability scan results, and static analysis findings may be included in future extensions or modernized CI/CD frameworks.
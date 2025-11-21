# Risk assessment process

### Purpose
Evaluates and records the **risk profile** of the system or release to determine the level of rigour, controls, and quality measures required across the SDLC.  
Aligned to **ISO 31000** and **ISO 15288** principles.

### Outcomes
- Release risk level determined and documented.  
- Key business, technical, security, and operational risks identified.  
- Controls and quality metrics tailored to the assessed risk level.  
- Release Risks / Issue Register created and approved by the business owner.

### Artefacts
| **Artefact** | **Description** |
|---------------|----------------|
| Release Risks / Issue Register | Records identified risks, likelihood, impact, and mitigation actions. |



# Release risk impact mapping matrix
This matrix illustrates the combined **overall risk impact level** associated with a release for a single risk aspect (category).

### Risk consequence vs likelihood

| **Highest Determined Risk Likelihood Level ↓** | **Insignificant** | **Minor** | **Moderate** | **Major** | **Critical** |
| ---------------------------------------------- | ----------------- | --------- | ------------ | --------- | ------------ |
| **Almost Certain**                             | Low               | Low       | High         | High      | High         |
| **Likely**                                     | Low               | Low       | High         | High      | High         |
| **Possible**                                   | Low               | Low       | Low          | High      | High         |
| **Unlikely**                                   | Low               | Low       | Low          | High      | High         |
| **Rare**                                       | Low               | Low       | Low          | Low       | High         |


### Notes
- Must be completed at the **start of every development activity**, regardless of release type.  
- Owned and performed by the **business owner** with support from development teams.  
- In iterative models, risk is **reassessed** during **System Analysis** to capture evolving risks.  
- Risk determinations drive the **acceptability criteria and quality metrics** applied across the SDLC.  
- For Agile and CI/CD contexts, incorporate risk gates into **automated workflow checks** or **release readiness dashboards**.
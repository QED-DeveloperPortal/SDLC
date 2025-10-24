---
index: true
---

# Release Categorization Dimensions (Process Viewpoints)
In order to demonstrate how certain goals for certain scenarios (e.g. developing high-risk systems) are achieved through the use of this SDLC process model, the process model can be viewed from different viewpoints. This chapter describes a number of such viewpoints from which different concerns related to systems development activities are addressed. The view seen out of the SDLC process model from each viewpoint will demonstrate how those goals are achieved in such scenarios.
These definitions and their properties have been aligned to ISO 24774:2010 \[3\].
In another perspective, these viewpoints are dimensions in which releases are categorized.


## Release Scope type
### Overview
As a property of a release (or the development activity that delivers the release), scope type is influenced to the amount of work that is involved in the development activity as well as the included items or software changes in the release. In order to cover all scope types, certain “tracks” in the life cycle model can be gone through covering certain stages for each release scope type.
For release scope type categorization, it is recommended for the Information and Technologies Branch (ITB) to partially use the definitions in ITIL \[8\], as follows, however, other areas of the agency may still use their existing labels, which is why a scope type mapping table will be presented later in this handbook to avoid confusion.
-  _Major releases and hardware upgrades_, normally containing large areas of new functionality, some of which may make intervening fixes to problems redundant. A major upgrade or release usually supersedes all preceding minor upgrades, releases and maintenance fixes.
-  _Minor releases_ _and hardware upgrades_, normally containing small enhancements and fixes, some of which may have already been issued as maintenance fixes. A minor upgrade or release usually supersedes all preceding maintenance fixes.
-   _Maintenance releases_, normally containing the corrections to a small number of known problems.


### Process Viewpoint Stakeholders
-  SDLC users (program managers, project managers, systems and software developers, database administrators, solutions architects etc…)
-  Department of Education


### Process Viewpoint Concerns
-  As a process model, the SDLC should be agile enough to allow the development teams perform their routines in a timely fashion with the minimum but most effective level of governance.
-  The SDLC should be able to cover all types of systems development activities, especially business as usual and maintenance-related activities, not just projectized activities.
-  The SDLC should provide controls, rigor, governance and accountability for any releases deployed in the production environment.


### Release Scope Types and Scope Type Mappings
In order to keep the SDLC generic and help it be applicable in different areas of the organization and due to existing release type labels for some areas and to avoid confusion, a generic set of labels (type 1, type 2 and type 3) will be used in this handbook that could be mapped to existing labels in each area, as Table 6 illustrates.

| SDLC Release Scope type Label | Information and Technologies Branch Release Type Label | Finance Branch Release Type Label | Human Resources Branch Release Type Label |
| --- | --- | --- | --- |
| Type 1 | Major | Project | Major |
| Type 2 | Minor | Major, Significant | Minor |
| Type 3 | Maintenance/Bug Fix | Minor, Emergency, Adhoc | Maintenance/Bug Fix |
Table 6 - release scope types and scope type mappings for different areas of the organization

Despite these definitions being subjective, there are a number of criteria that can help the development teams determine which category of release they should choose as it affects the governance model and supporting artefacts applicable.
One distinguishing difference between Type 3 releases as opposed to Type 2 is the fact that for Type 3 releases, the requirements do not change. Consequently, in scenarios where requirements are being changed or there are new requirements, the choices will be limited to either Type 1 or Type 2 releases.
NOTE: The first release of a system that has never existed before is considered a Type 1 release irrespective of its actual size.
Table 7 illustrates a list of criteria to determine the scope type of a release. When using “Table 7”, a single “yes” should be considered enough to determine the release scope type.

| Release Scope type | Being the first-ever release of a new system or solution[2] | Whether the release changes business processes involving other agencies for the first time | Whether the release delivery estimates exceed the business-as-usual capacity, or, the delivery requires new funding arrangements | Whether the release includes new requirements or modifications made to existing requirements |
| --- | --- | --- | --- | --- |
| Type 1 | Yes | Yes | Yes | Yes |
| Type 2 | No | No | No | Yes |
| Type 3 | No | No | No | No |
Table 7 - Release Scope Type Determination Criteria Matrix
You can refer to section “‎7.11.5.2” which explains the release planning and scope type determination process in details.


### Release Versioning Conventions
It is highly recommended to follow a unified versioning convention that is aligned with the release types discussed in this handbook.
Due to a 3-level release scope type categorization scheme, it is recommended to use 3 numbers for each release that could match the _Major.Minor.Maintenance.BuildNumber_ convention.
This identifier should remain the same for a release aimed for the production environment, however, a fourth “build number” will be used to differentiate between different builds of the same release that should remain unique for each release.
NOTE: The SDLC process model aims to deliver an end-to-end “production” release that may go through its own life cycle (Alpha (Dev), Betta (Zone 2), and Release Candidate (MPE)). In that view, the build number can be the only number that may be different in different stages of a release life cycle.   
Example:
Once a release is in its Betta stage (i.e. when it’s being tested in Zone 2 as V1.2.3.200), new issues may be found to be addressed in the next iterations. After they are fixed, a new build will be created (off the same release) with a new build number making the Betta release unique (e,g, V1.2.3.300) which will be deployed in Zone 2 for further tests. Once it’s confirmed the release is production-ready, the same release (V1.2.3.300) may proceed to next stages to be deployed in the production environment.
NOTE: It is recommended to use increasing numbers for the build number to represent a maturing state of the same release that goes through multiple build iterations.


### Release Units
A release unit describes the portion of a service or IT infrastructure that is normally released together according to the organisation’s release policy. The unit may vary, depending on the type(s) or item(s) of service asset or service component such as software and hardware.
The general aim is to decide the most appropriate release unit level for each service asset or component, however, as a general principle, it is highly necessary to avoid bundling releases with high risk profiles with low-risk releases as this will turn the bundle into a high-risk bundle.


## Risk
### Overview
Risk is a characteristic of a release under development and how the SDLC addresses different levels of it is viewed through this viewpoint.
From the risk perspective, irrespective of other perspectives like scope type, the SDLC should apply different levels of control and rigor on pre-production readiness definitions, criteria and examinations.
This viewpoint is another dimension over the SDLC besides others (like scope type) and ensures any change, irrespective of scope type, covering a system, or a module, with high Risk, will go through extra steps while mandating extra artefacts before production readiness is achieved.


### Process Viewpoint Stakeholders
-  SDLC users (program managers, project managers, systems and software developers, database administrators, solutions architects etc…)
-  Department of Education


### Process Viewpoint Concerns
-  The SDLC should remain agile enough for business as usual activities.
-  The SDLC should not create extra red tapes in daily business operations.
-  The SDLC should provide a consistent set of definitions and artifacts for each Risk level.
-  The SDLC should cover all types of systems development activities, especially business as usual and maintenance-related activities, not just projectized activities.
-  The SDLC should provide the optimum and effective level of rigor before a release is deployed in the production environment, especially for systems where there’s a very low levels of tolerance for risk.


## Hosting/Deployment Environment
### Overview
Hosting/deployment environment is another property of a release under development and how the SDLC addresses different environments is viewed through this perspective.


### Process Viewpoint Stakeholders
-  SDLC users (program managers, project managers, systems and software developers, database administrators, solutions architects etc…)
-  Department of Education


### Process Viewpoint Concerns
-  The SDLC should address and cover the different paths needed to be taken for cloud-based development.
-  Since majority of platform-as-a-service environments keep changing frequently without DET’s control, it’s vital that the SDLC remains agile and provides the chance for the development teams to catch up with the demand of an ever-green hosting environment.
The SDLC should ensure that all procedures around development for the cloud remain consistent, clear and documented.

  
* * *

[\[1\]] The original title for the 3rd release type in ITIL is “Emergency” but internal stakeholders in DET agreed upon eliminating the urgency dimension in the title and use “Maintenance” instead. Obviously, urgency may affect priority and timings but it does not affect the size or governance model around releases since maintaining the health of the production environment has the highest priority of all.

[\[2\]]) Non existing systems are the ones that are new as a whole and are not being added to existing systems (e.g. a new game being added to a “game bundle system” does not constitute being the first-ever release of a new system).

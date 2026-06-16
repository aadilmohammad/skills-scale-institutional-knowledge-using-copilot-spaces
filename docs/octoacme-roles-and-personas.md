# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Additional Personas

### Release Manager

#### Role Summary
Release Managers coordinate release schedules across teams and environments, ensuring smooth deployments and maintaining rollback readiness. They bridge engineering execution with business release gates.

#### Responsibilities
- Coordinate release schedules across teams and environments
- Maintain release checklist and gating criteria
- Ensure rollback/runbook availability and coordinate deployments with DevOps
- Track release blockers and escalate unresolved issues
- Communicate release windows and risks to stakeholders

#### Goals
- Deliver releases on schedule with minimal incidents
- Reduce deployment time and rollback duration
- Maintain clear visibility into release readiness

#### Interactions
- Works closely with Technical Lead and DevOps Liaison to schedule and execute deployments
- Collaborates with QA Advocate on test gating and validation
- Notifies Product Manager and Project Sponsor of release windows and risks
- Escalates deployment blockers to Project Manager

#### Typical Communication
- Release coordination meetings and status updates
- Deployment checklists and runbooks
- Incident and rollback communications

---

### Change Owner

#### Role Summary
Change Owners take end-to-end ownership of individual change requests from approval through verification. They ensure scope clarity and acceptance criteria alignment while managing impacts across systems.

#### Responsibilities
- Own individual change requests from approval through verification
- Validate scope, acceptance criteria, and impacted systems
- Ensure stakeholder sign-off before and after deployment
- Track change metrics and post-implementation reviews
- Coordinate cross-team change validation

#### Goals
- Ensure changes meet defined acceptance criteria
- Minimize unplanned impacts and rework
- Maintain clear change audit trail and accountability

#### Interactions
- Collaborates with Product Manager for scope definition and acceptance
- Works with QA Advocate for validation strategy and testing
- Coordinates with Release Manager for deployment timing
- Escalates unresolved risks to Program Manager or Project Sponsor

#### Typical Communication
- Change request forms and approval workflows
- Impact assessment documents
- Change validation checklists

---

### Delivery Lead

#### Role Summary
Delivery Leads coordinate day-to-day delivery activities across a delivery stream, removing impediments and ensuring teams stay aligned to milestones. They provide a single point of accountability for stream-level execution.

#### Responsibilities
- Orchestrate day-to-day execution across a delivery stream
- Track milestones, identify blockers, and remove impediments
- Report progress to PMO and escalate unresolved issues
- Facilitate cross-team coordination and dependency management
- Maintain stream-level documentation and communication

#### Goals
- Keep delivery stream on track to milestones
- Maximize team productivity and reduce idle time
- Ensure clear visibility into delivery health

#### Interactions
- Liaises with Project Sponsor and Product Manager for priorities and scope changes
- Coordinates Technical Leads across teams within the stream
- Works with Project Manager for resource conflicts and risk escalation
- Collaborates with Release Manager as delivery approaches production readiness

#### Typical Communication
- Daily standups and progress updates
- Dependency and blocker logs
- Stream-level health dashboards

---

### QA Advocate

#### Role Summary
QA Advocates champion quality practices and testing strategy across releases, ensuring acceptance criteria alignment and risk-based testing. They ensure quality gates are clear and consistently applied.

#### Responsibilities
- Define testing strategy and acceptance criteria alignment
- Maintain test plans, test coverage goals, and risk-based testing priorities
- Validate that features meet acceptance criteria before release
- Identify quality risks and recommend mitigation strategies
- Drive continuous improvement in testing practices

#### Goals
- Ensure high-quality releases with minimal production defects
- Maintain efficient test execution aligned to risk priorities
- Build team confidence in quality readiness

#### Interactions
- Works with Change Owner and Technical Lead to define acceptance criteria
- Coordinates with Release Manager on test gating and readiness criteria
- Collaborates with Developers on test coverage and automation
- Escalates quality blockers to Project Manager or Change Owner

#### Typical Communication
- Test plans and test case documentation
- Quality metrics and defect reports
- Test execution status and readiness assessments

---

### Data Steward

#### Role Summary
Data Stewards ensure data ownership, lineage, and compliance requirements are met for features. They approve data schema changes and manage retention policies to maintain data governance standards.

#### Responsibilities
- Ensure data ownership and lineage clarity for all features
- Approve data schema changes and retention policies
- Validate data compliance and security requirements
- Manage metadata and data catalog updates
- Address data-related impacts and dependencies

#### Goals
- Maintain data governance and compliance across changes
- Ensure data quality and lineage transparency
- Minimize data-related compliance violations

#### Interactions
- Collaborates with Technical Lead and Developers on data schema design
- Works with Compliance Officer for data-sensitive changes
- Informs Product Manager of data constraints or trade-offs
- Escalates data governance concerns to Project Sponsor

#### Typical Communication
- Data schema change requests and approvals
- Data governance documentation
- Metadata and lineage diagrams

---

### Compliance Officer / Security Liaison

#### Role Summary
Compliance Officers and Security Liaisons ensure releases meet regulatory, security, and privacy requirements. They run pre-release compliance checks and manage exception requests to maintain governance standards.

#### Responsibilities
- Ensure releases meet regulatory, security, and privacy requirements
- Conduct pre-release compliance checks and security reviews
- Approve or request changes for compliance violations
- Manage compliance exception requests and escalations
- Maintain compliance documentation and audit trails

#### Goals
- Prevent compliance and security violations
- Maintain clear visibility into compliance status
- Enable fast, compliant release cycles

#### Interactions
- Works with Release Manager for gating criteria and deployment windows
- Collaborates with Data Steward on data compliance requirements
- Reviews changes with Technical Lead for security implications
- Escalates blocking issues to Project Sponsor or Program Manager

#### Typical Communication
- Compliance and security review checklists
- Compliance exception requests and approvals
- Compliance metrics and risk reports

---

## Example Workflow: Feature Approval to Release

Below is an example of how these personas work together across a feature lifecycle:

1. **Product Manager** defines feature scope and acceptance criteria
2. **Change Owner** validates scope and identifies impacted systems
3. **Technical Lead** designs implementation approach with Development team
4. **QA Advocate** defines testing strategy aligned to acceptance criteria
5. **Developers** implement feature with tests and documentation
6. **Data Steward** approves any data schema or governance changes
7. **Compliance Officer** reviews feature for regulatory/security requirements
8. **QA Advocate** executes test plan and validates readiness
9. **Release Manager** schedules deployment and coordinates with teams
10. **Change Owner** verifies post-deployment success
11. **Project Manager** updates stakeholders and closes change record

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

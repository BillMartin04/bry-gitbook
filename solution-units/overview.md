---
description: >-
  Modular, governed ServiceNow Architecture solutions built for visibility,
  reuse, and long-term value. The foundation of every ServiceNow Solution
  Architecture Unit in the BRY Framework
---

# Overview

### In this article

* Audience
* Goals
* Layers of the Build It the Right Way Framework
* Adopt a phased learning process and improve quality iteratively
* Related links
* Conclusion

### Audience

This article is intended for ServiceNow architects, developers, platform owners, and product managers who design, deliver, or govern solutions using the Build It The Right Way (BRY) Framework. It is also relevant to compliance teams, business stakeholders, and integration partners involved in enterprise ServiceNow delivery. Understanding Solution Units helps unify the vision and execution across these diverse roles.

### Goals

A Solution Unit in the BRY Framework is a complete, service-aligned solution designed on the ServiceNow platform to deliver a defined business outcome. It encapsulates application logic, data structures, integrations, support processes, and governance controls into a modular, composable unit.

Solution Units act as the core delivery and architecture model in BRY. They establish architectural boundaries, enforce ownership, and support service-aware modeling through alignment with the Common Service Data Model (CSDM).

Thinking in terms of Solution Units enables structured ServiceNow implementation and reduces complexity. Teams gain:

* Clear architectural ownership and delivery accountability
* A repeatable design approach aligned to business capabilities
* Scalable governance using modular responsibility boundaries
* Visibility through CMDB service modeling and impact mapping
* A foundation for continuous improvement and lifecycle management

### Layers of the Build It the Right Way Framework

#### Solution Units in the BRY Framework

In the Build It The Right Way (BRY) Framework, a Solution Unit is a complete, modular, service-aligned solution designed and operated on the ServiceNow platform. It represents a purposeful composition of application logic, data structures, integrations, and operational processes aimed at delivering a specific business outcome.

A Solution Unit is not just an application or module. It is a governed architectural entity. It has defined ownership, follows platform standards, aligns with enterprise goals, and is built for continuous improvement. Every Solution Unit adheres to the BRY architectural pillars and is modeled using the Common Service Data Model (CSDM) to ensure service awareness and visibility.

Each unit reinforces the broader BRY architecture by ensuring modularity, traceability, and alignment with the business model. This reinforces the goals of governance and scalability mentioned earlier.

#### What is a Solution Unit?

A Solution Unit is a self-contained ServiceNow implementation that delivers a cohesive business capability. It may include one or more scoped applications, data flows, integrations, and supporting infrastructure. A Solution Unit exists to fulfill a purpose and must be modeled, governed, and evolved intentionally.

Solution Units are designed to be composable. Each one can function independently but contributes to the larger enterprise architecture. Whether you're building an ITSM solution, a custom legal request intake app, or a partner-facing service portal, each is handled as a distinct Solution Unit.

#### Why Solution Units Matter

ServiceNow implementations often grow without structure, leading to inconsistent designs, tech debt, and unclear ownership. The Solution Unit model brings structure and discipline. It enables teams to deliver with intention, track solution boundaries, and apply governance without unnecessary friction.

Solution Units promote the following outcomes:

* Clear ownership and accountability
* Architectural consistency across implementations
* Measurable alignment with business outcomes
* Modularity and reusability
* Scalable governance through shared responsibility

#### Composition of a Solution Unit

Each Solution Unit includes the following components:

* Business context and outcome it supports
* Application logic and configuration
* CSDM-aligned data modeling
* Infrastructure and integration dependencies
* Role-based access and security controls
* Monitoring, observability, and support processes
* Versioning and change management plans

Solution Units must be anchored to real-world business services and capabilities. They include both the functional logic and the underlying technical resources that deliver value. The supporting infrastructure, application services, and integration points must all be explicitly modeled and governed to ensure performance, visibility, and maintainability.

Each of these components directly supports the architectural pillars and platform-wide consistency goals laid out in later sections.

### Adopt a phased learning process and improve quality iteratively

#### BRY Architectural Pillars

All Solution Units must align with the following eight BRY architectural pillars:

**Modularity and Reusability**\
Build once, reuse everywhere. Design utilities and logic that can serve multiple teams and use cases.\
&#xNAN;_&#x52;educes duplication, simplifies maintenance, and accelerates development._

**Security by Design**\
Incorporate access control, data validation, and scoped logic from the beginning.\
&#xNAN;_&#x50;revents breaches, protects data integrity, and ensures trust._

**Scalability and Performance**\
Design for future growth, not just current load. Use async processes, queues, and efficient queries.\
&#xNAN;_&#x53;upports enterprise load, ensures reliability, and future-proofs your solutions._

**Observability and Auditability**\
Build visibility into systems—logging, traceability, and error tracking are essential.\
&#xNAN;_&#x45;nables rapid debugging, compliance support, and better operational control._

**Alignment with the Business Model**\
Reflect business services, owners, and processes in your architecture.\
&#xNAN;_&#x43;reates meaningful data, improves reporting, and links IT to value delivery._

**Upgrade-Safe Architecture**\
Avoid hardcoding and direct modification of out-of-box logic. Use scoped apps and configuration.\
&#xNAN;_&#x53;implifies upgrades, reduces risk, and enables continuous improvement._

**Separation of Concerns**\
Keep validation, processing, and presentation logic in their own domains.\
&#xNAN;_&#x49;mproves clarity, testing, and collaborative development._

**Governance and Control**\
Enforce naming standards, code reviews, and structured deployments.\
&#xNAN;_&#x4D;aintains platform quality, aligns teams, and enables secure scale-out development._

These pillars are what enable the Solution Unit structure to succeed. Every layer, from goals to governance, is reinforced through these principles.

#### CSDM Alignment and Service Modeling

Each Solution Unit must be modeled using CSDM to support platform intelligence, impact analysis, and service awareness. This includes mapping:

* Business Services and Capabilities
* Business Applications and Application Services
* Underlying Technical Resources
* Supporting Infrastructure

CSDM alignment ensures consistency across the CMDB. It allows shared services like AIOps, SLAs, Discovery, and Service Mapping to function effectively. By clearly modeling the business layer and technical foundation, Solution Units become discoverable, observable, and maintainable.

This alignment is also foundational to modularity, reuse, and business-driven architecture—the same principles introduced under Goals and the BRY Pillars.

#### Roles and Responsibility

Each Solution Unit is owned and operated by a cross-functional team responsible for its full lifecycle. Responsibilities include design, development, governance, and support. Performance and reliability metrics should be tracked as part of ongoing ownership.

**Solution Unit Team Roles**

* Product or Solution Owner
* Architect
* Developer(s)
* Quality Assurance / Testing Lead
* Support Analyst
* Business Process Stakeholders

**Centralized Support Teams**

* BRY Architecture Council
* ServiceNow Platform Engineering
* Security and Compliance
* Data Governance
* Infrastructure and DevOps

Documenting responsibilities, support processes, and metrics in solution portfolios or internal knowledge bases ensures transparency and accountability.

This shared ownership model supports the governance and control pillar, and creates alignment across organizational silos.

### Lifecycle and Governance

Solution Units must go through structured lifecycle stages, including:

* Solution design and architectural review
* Security assessment and validation
* Operational readiness checks
* Deployment and change tracking
* Ongoing reviews for improvement and alignment

Lifecycle governance ensures Solution Units remain healthy, relevant, and aligned with evolving business and platform requirements. These stages reinforce the continuous improvement and compliance goals introduced earlier.

#### Enhanced Solution Unit Lifecycle Table

_The following lifecycle table breaks down each Solution Unit phase with examples, BRY applications, measurable outcomes, ServiceNow enablers, and common pitfalls to avoid:_

| **Phase**                                | **Use Case Example**                                     | **BRY Framework Application**                                                                   | **Outcomes**                                                               | **Common Pitfalls to Avoid**                            | **ServiceNow Enablers**                                    | **Sample KPI’s**                                        |
| ---------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | ------------------------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------- |
| 1. Identify the Need                     | Employee offboarding is manual and inconsistent          | Evaluate inefficiencies and business gaps. Gather outcome expectations with stakeholders.       | Clear business problem defined. Alignment with actual capabilities needed. | Vague or undocumented business problems                 | Surveys, Demand Management, Business Case tools            | Process gaps identified, stakeholder alignment score    |
| <p>2. Define the</p><p>Solution Unit</p> | Offboarding workflow needs automation                    | Define scope and ownership. Map dependencies, affected users, and integrations.                 | Solution boundaries, purpose, and ownership clarified.                     | Undefined scope or stakeholder misalignment             | Project Portfolio Management (PPM), APM, Process Workshops | Scope clarity, time-to-plan, % stakeholder coverage     |
| 3. Architect with BRY Pillars            | Roles, tasks, security, and data dependencies identified | Apply modular design, scoped apps, integration guardrails, and compliance requirements.         | Architecture is secure, scalable, and upgrade-safe.                        | Skipping security, scalability, or upgrade planning     | Scoped Apps, Flow Designer, ATF, IntegrationHub            | Architecture approval rate, compliance coverage         |
| 4. Implement the Unit                    | Build workflow, access revocation, notifications         | Develop using scoped apps. Integrate with HR and IT systems. Follow separation of concerns.     | Working service-aware automation.                                          | Tight coupling, hardcoded logic, or ignoring governance | Studio IDE, ACLs, Flow Designer, Custom Apps               | User adoption, task automation %, bug rate              |
| 5. Model with CSDM                       | Map Offboarding to cmdb\_ci\_service and capabilities    | Represent data in CMDB for visibility and impact analysis. Tie services to technical resources. | Enables service mapping, observability, and performance tracking.          | Inconsistent CMDB modeling or lack of service links     | CSDM, CMDB, Service Mapping, App Services                  | CSDM coverage %, CMDB accuracy %, service visibility    |
| 6. Govern & Support                      | Add playbooks, logging, and access reviews               | Document roles, enable monitoring, and define SLAs. Assign platform responsibilities.           | Shared ownership. Continuous monitoring and support.                       | Lack of observability or unclear support boundaries     | Service Level Management, Dashboards, Knowledge            | SLA compliance rate, MTTR, % documented playbooks       |
| 7. Improve Iteratively                   | Adjust based on incidents and SLA breaches               | Conduct retrospectives and architecture reviews. Evolve based on feedback.                      | Solution matures over time. Value grows and risk is reduced.               | Ignoring feedback, metrics, or platform upgrades        | Performance Analytics, AIOps, DevOps Change Velocity       | Cycle time improvement, reduction in repeated incidents |

### Continuous Improvement

Solution Units are not static. They evolve based on performance feedback, changing requirements, and updated platform capabilities. The BRY Framework encourages regular retrospectives, architecture reviews, and performance audits to identify opportunities for optimization or redesign.

Teams are expected to treat Solution Units as living assets—constantly monitored, maintained, and refined. This reinforces the entire phased learning approach of the BRY Framework, connecting design with operations and improvement.

### Related links

* ServiceNow Architect’s Checklist
* ServiceNow Architecture Pattern Library
* Design Decision Principles
* Overview: ServiceNow Build It the Right Way Framework Pillars

### Conclusion

Solution Units are the foundation of the BRY approach to ServiceNow architecture. They provide a disciplined way to define, design, govern, and scale ServiceNow solutions with a strong alignment to business value.

By thinking in Solution Units, you create measurable, supportable, and secure solutions that can grow with the organization. This modular, service-aware approach helps teams deliver faster, govern better, and build on a stronger architectural foundation.

Everything in this framework is connected from audience and goals to design principles, roles, and governance. Solution Units are not just a method; they are the means through which BRY ensures quality, accountability, and enterprise alignment.

This is how we build it the right way.

---
description: >-
  Build It the Right Way is a ServiceNow architecture framework for designing
  scalable, secure, and maintainable solutions through an architecture-led,
  compliance-first approach to the Now Platform.
---

# What is the Build It the Right Way Framework?

{% embed url="https://youtu.be/1Esg-JUhjnE" %}
A twelve-minute walkthrough of the framework, the eight pillars, and how to use this site week-to-week.
{% endembed %}

Build It the Right Way is an architectural guidance model designed specifically for the ServiceNow platform. It exists to close the governance gap that opens when enterprises adopt the Now Platform feature first, standing up ITSM, HRSD, SPM, and ITOM in isolation, by different integrators, on top of a CMDB that was never properly modelled.

The framework moves governance to the front of the design process. Architecture led, compliance first. Every decision is evaluated against a fixed set of pillars before code is written. Governance is not a quarterly review. It is a design gate.

### In this article

* Audience and accountability
* Goals of the framework
* Core pillars
* Architectural blueprint
* Governance control gates
* Roles and ownership
* Implementation roadmap
* Success metrics
* Related links

## Audience and accountability

The framework is for the people who carry architectural accountability on the Now Platform. The ServiceNow architect making design calls every week. The platform owner accountable to executives for outcomes. The developer who needs reusable patterns instead of relearned lessons. The delivery manager bringing discipline to the team. The compliance and risk leader who needs to see the guardrails.

If you influence what gets built on the Now Platform, this framework is written for you. It applies equally to startups, large enterprises, managed service providers, and public sector teams. It pairs naturally with CSDM, APM, and strategic portfolio planning.

## Goals of the framework

The framework helps your ServiceNow workloads remain scalable and resilient through platform upgrades, maintain the security and auditability regulators expect, stay aligned to business needs without sacrificing architectural integrity, support governance and lifecycle efficiency that lets you ship faster instead of slower, and deliver consistent release quality across every deployment.

These outcomes are not aspirational. They are what the framework is engineered to produce when its pillars are applied with discipline.

## Core pillars

The framework is built on eight architectural pillars. Every design decision is evaluated against all eight. No single pillar wins on its own. Balance is the goal.

1. **Platform Governance.** The operating model that defines who decides what gets built, on which scope, with which approval. Prevents shadow customisation.
2. **Configurable over Custom.** Out of the box capability is always evaluated first. Custom code is a last resort, never a default.
3. **Secure by Design.** Access controls, data classification, and audit trails are designed into the solution, not bolted on after a penetration test.
4. **Performance-Aware.** Every table, integration, and workflow is sized for the load it will carry at full enterprise volume, not at pilot scale.
5. **Lifecycle Ready.** The solution can be upgraded, patched, cloned, and retired without surprise. Update sets, application scopes, and release pipelines are first-class concerns.
6. **Service-Oriented.** The architecture reflects the business services you actually deliver, modelled through CSDM, not the org chart you happen to have today.
7. **Extensibility.** APIs, Integration Hub spokes, and connector strategy are designed for a partner ecosystem that will keep growing.
8. **Observability.** You cannot govern what you cannot measure. Health metrics, performance analytics, and operational dashboards are built in from day one.

Each pillar has its own deep-dive page on this site with principles, design goals, recommended approaches, and a self-assessment checklist.

## Architectural blueprint

The framework is organised in three layers. The navigation pattern is **Pillars first, then Solution Units, then Capability Guides.**

#### Pillars

The foundation. Each pillar page presents core principles, design goals, and recommended approaches treated as non-optional. A self-assessment checklist sits at the bottom of every pillar page, with each item linking to implementation guides, reference architectures, and pattern libraries. Design tradeoffs are stated explicitly so teams can balance decisions across performance, maintainability, and business goals.

#### Solution Units

Where the eight pillars get applied to a specific ServiceNow domain. ITSM, IRM, ITOM, HRSD, and Custom Applications each have their own page. Inside every Solution Unit you will find design principles tailored to the domain, the critical design areas where decisions get made, best practice guides for each area, and a maturity assessment to benchmark readiness. Start with the Solution Context, then explore the Design Areas to identify governance gaps.

#### Capability Guides

The most tactical layer. Each guide focuses on a specific Now Platform feature such as Flow Designer, ACLs, Update Sets, or the CSDM model, and explains how to design with that feature in a way that respects all eight pillars. These are not feature tutorials. They tell you when to use the feature, what design patterns apply, and how to keep usage compliant, secure, and extensible.

## Governance control gates

Architectural integrity is enforced through four sequential gates. A build does not advance until the preceding gate is signed off.

1. **Design Intent.** Pillar checklist signed off before build approval. Architect owns sign-off, compliance lead is consulted.
2. **Build Review.** Architecture Review Board validates the design against the relevant Solution Unit design areas.
3. **Pre-Production.** Capability Guide compliance confirmed. The risk log is cleared or each open item is formally accepted.
4. **Post Go-Live Audit.** Maturity assessment re-scored within ninety days of go-live. Findings feed the next quarter's priorities.

## Roles and ownership

The framework only works when accountability is unambiguous.

The **architect** owns pillar interpretation and design-gate sign-off. The **platform owner** is accountable for adoption pace and KPI delivery. **Developers** apply the Capability Guides on the ground and flag pillar conflicts the moment they appear. The **delivery manager** enforces the gates inside the delivery pipeline. The **compliance lead** is consulted at Gate 1 and Gate 3.

## Implementation roadmap

The framework is not intended to be implemented all at once. That is the single most common mistake teams make.

Begin with the pillar that maps to your biggest current risk. Teams facing an audit lead with Secure by Design and Platform Governance. Teams drowning in custom code lead with Configurable over Custom. Teams whose platform is slow lead with Performance-Aware and Observability. Teams with an unreliable CMDB lead with Service-Oriented and Lifecycle Ready.

Get one pillar embedded into how the team operates. Run real design reviews against it for a quarter. Add the next pillar. Run the first full maturity assessment on one Solution Unit by the end of the second quarter. Within twelve to eighteen months, all eight pillars become the default operating model. Not because anyone forced it, but because every pillar proved its value as it was adopted.

## Success metrics

The framework is measured, not declared. Five indicators tell you whether it is working.

The **architectural debt ratio** tracks custom code volume against out-of-the-box capability in use. The **gate pass-through rate** measures the percentage of builds clearing all four gates on the first attempt. The **maturity score trend** is recorded per Solution Unit, quarter over quarter. The **upgrade lead time** is measured in days from one ServiceNow release to adoption of the next. The **audit findings per release** target is zero on Secure by Design controls.

These metrics belong on the platform owner's dashboard. They are the leading indicators that distinguish a healthy ServiceNow practice from one heading toward replatform.

## About the author

Bill Martin. ServiceNow MVP 2026, Certified Technical Architect, seven times CIS certified, Certified Instructor. K26 keynote speaker. This framework is distilled from more than fifty enterprise ServiceNow environments where the wrong decision cost real money.

## Related links

* [ServiceNow Build It the Right Way Architecture Pillars](../pillars/servicenow-architecture-pillars.md)
* [ServiceNow Architecture Pattern Library](../design-patterns/servicenow-architecture-pattern-library.md)
* [Design Decision Principles](../design-decisions/design-decision-principles.md)
* [ServiceNow Architect's Checklist](../design-artifacts/servicenow-architects-checklist.md)
* [Solution Units overview](../solution-units/overview.md)

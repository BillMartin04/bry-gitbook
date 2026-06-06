---
description: >-
  The eight foundational pillars of the Build It The Right Way framework. Each
  pillar defines an architectural principle, the governance discipline that
  enforces it, and the platform outcomes it produces on ServiceNow.
---

# Pillars Overview

The Build It The Right Way (BRY) framework rests on **eight architectural pillars**. Together they form the architecture led, compliance first operating model that governs how we design, build, and evolve solutions on the Now Platform. Each pillar is non negotiable. Each pillar is measurable. Each pillar maps to specific control gates, KPIs, and review artifacts inside this GitBook.

These pillars are not aspirations. They are **design criteria** applied at every change request, **review checkpoints** enforced at every control gate (G0 through G4), and **teaching tools** used to onboard architects, developers, and platform owners into a single shared discipline.

{% hint style="info" %}
**How to use this page.** Treat the pillars as a checklist during design, a scoring rubric during architectural review, and a curriculum spine when training new engineers. Every pillar links to a dedicated chapter with detailed standards, anti patterns, control gates, and assessment tooling.
{% endhint %}

## Anchor Walkthrough

A guided tour of the eight pillars, the reasoning behind their order, and how they reinforce one another in production environments.

{% embed url="https://youtu.be/ZLsy6J94Cp0" %}
Pillars Overview, anchor walkthrough by TechTalk with Bill
{% endembed %}

## The Eight BRY Pillars

| **№** | **Pillar**                | **Architectural Principle**                                                                                                  | **Why It Matters**                                                                                                              |
| ----- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 1     | **Platform Governance**   | Establish authoritative ownership, scope boundaries, naming standards, and a single source of architectural truth.           | Eliminates shadow builds, enforces architectural intent across squads, and gives leadership a defensible control plane.         |
| 2     | **Configurable over Custom** | Prefer configuration, scoped apps, and out of box capability. Custom code is a last resort that requires written justification. | Protects upgrade safety, reduces total cost of ownership, and keeps the platform aligned to vendor roadmap.                     |
| 3     | **Secure by Design**      | Embed access control, data classification, scoped logic, and least privilege from the first design artifact onward.           | Prevents breaches, satisfies regulatory mandates, and removes the cost of retrofitting security after go live.                  |
| 4     | **Performance Aware**     | Design for sustained enterprise load using asynchronous patterns, efficient queries, indexed tables, and queue based scaling. | Supports peak business volume, protects user experience, and prevents architectural debt from surfacing as production incidents.|
| 5     | **Lifecycle Ready**       | Treat every solution as a long lived asset. Plan for upgrade, deprecation, data migration, and ownership succession up front. | Sustains platform health across release cycles and keeps every component recoverable, replaceable, and auditable.               |
| 6     | **Service Oriented**      | Model business services, owners, and capabilities as first class citizens. Architecture must mirror the operating model.      | Produces meaningful CMDB data, enables outcome based reporting, and connects IT delivery to measurable business value.          |
| 7     | **Extensibility**         | Design composable, loosely coupled, API first components. Build once, reuse everywhere, integrate everywhere.                 | Cuts duplication, accelerates delivery, and unlocks safe expansion into adjacent ServiceNow workflows and external systems.     |
| 8     | **Observability**         | Engineer visibility in from day one. Logging, traceability, audit events, and health signals are deliverables, not afterthoughts. | Enables rapid incident response, satisfies audit and compliance evidence requests, and creates the data backbone for AIOps.   |

## How the Pillars Interact

The pillars are **mutually reinforcing**, not independent. A weakness in one pillar will surface as a defect in another.

{% hint style="success" %}
**Platform Governance** is the foundation. Without it, the remaining seven pillars cannot be enforced at scale.
{% endhint %}

{% hint style="success" %}
**Configurable over Custom** and **Lifecycle Ready** together protect upgrade safety. They are reviewed jointly at Control Gate G2.
{% endhint %}

{% hint style="success" %}
**Secure by Design** and **Observability** together produce the audit and compliance evidence trail. They are reviewed jointly at Control Gate G3.
{% endhint %}

{% hint style="success" %}
**Performance Aware**, **Service Oriented**, and **Extensibility** together define the platform's capacity to scale into new workflows without rework. They are reviewed jointly at Control Gate G4.
{% endhint %}

## Pillar Anatomy

Every pillar chapter in this GitBook follows the same structure so reviewers, architects, and engineers can navigate predictably.

1. **Intent.** The architectural principle in one paragraph.
2. **Anchor Video.** A five to seven minute walkthrough hosted on TechTalk with Bill.
3. **Standards.** The non negotiable rules enforced by the pillar.
4. **Anti Patterns.** Documented violations and the production failures they cause.
5. **Control Gates.** The specific G0 through G4 checkpoints where this pillar is evaluated.
6. **KPIs and Metrics.** Quantitative measures used in platform health reviews.
7. **Review Artifacts.** Templates, checklists, and decision records that produce audit evidence.
8. **Capability Guides.** Linked how to material for engineers implementing the pillar in delivery.

## Next Steps

1. Read **Design Decision Principles** to understand the decision discipline that operates across every pillar.
2. Review the **ServiceNow Architects Checklist** to see how the pillars manifest as concrete review questions.
3. Explore the **Architecture Pattern Library** for vetted reference implementations of each pillar in production.
4. Open the **Implementation Roadmap** to plan the Crawl, Walk, Run, Fly progression for your platform.

{% hint style="warning" %}
**This page is normative.** When a pillar described elsewhere in this GitBook conflicts with the table on this page, the table on this page is the source of truth. Submit a change request to reconcile any drift.
{% endhint %}

---
description: >-
  The Build It The Right Way (BRY) Framework — an architecture-led,
  compliance-first governance model for designing scalable, secure, and
  maintainable ServiceNow solutions.
---

# What is the Build It The Right Way Framework?

{% hint style="info" %}
🎥 **Anchor Video** *(to be embedded)*

Title: **Welcome to Build It The Right Way — The ServiceNow Architecture Framework**

Length: ~5 minutes

YouTube URL: *paste embed link here*
{% endhint %}

The **Build It The Right Way (BRY) Framework** is an architectural governance model purpose-built for the ServiceNow platform. It guides teams to design, build, and operate solutions that are **scalable, secure, auditable, and aligned to the strategic intent of the business**.

BRY is inspired by the discipline of the **AWS Well-Architected Framework** and adapted for the realities of enterprise workflow platforms. It establishes a non-negotiable, architecture-led approach to platform delivery: every decision is traceable to a documented principle, every change passes a defined control gate, and every capability advances a measurable business outcome.

## The Problem BRY Solves

Modern enterprises scaling on ServiceNow consistently encounter four governance gaps. BRY is designed to close each one.

1. **Architectural Drift.** Tactical decisions accumulate into structural liabilities that cannot be unwound without disruptive rework.
2. **Compliance Reactivity.** Audit, regulatory, and risk requirements are retrofitted into solutions rather than designed in at inception.
3. **Customization Sprawl.** Out-of-the-box capability is bypassed in favor of bespoke development, eroding upgradeability and inflating total cost of ownership.
4. **Ownership Ambiguity.** Cross-functional decisions stall because authority, accountability, and escalation paths are undefined.

## Audience

BRY is authoritative for any role that influences platform design, build, operation, or ownership.

| Role | How BRY Serves Them |
|------|----------------------|
| **Enterprise Architects** | Codifies the principles, patterns, and decision rights they are accountable for |
| **Solution Architects** | Provides reusable templates, checklists, and trade-off frameworks |
| **Platform Owners** | Establishes the control gates and KPIs that prove platform health |
| **Compliance and Risk Officers** | Anchors security, audit, and regulatory mapping into the design phase |
| **Product Managers** | Aligns business intent with architectural feasibility |
| **Delivery Leads** | Standardizes the path from intake to production readiness |
| **Executive Sponsors** | Provides board-grade visibility into architectural posture |

BRY applies equally to **startups establishing first-time governance**, **large enterprises hardening at scale**, **managed service providers standardizing multi-tenant delivery**, and **public sector teams aligning to regulatory mandates**.

## Goals

The framework exists to drive four outcomes:

1. **Architectural Success.** Well-informed design choices made early, avoiding technical debt.
2. **Platform Confidence.** Decisions grounded in proven principles, validated across finance, healthcare, telecommunications, and public sector deployments.
3. **Risk Awareness.** Architectural trade-offs evaluated early and aligned with governance, security posture, and user experience.
4. **Continuous Improvement.** A benchmark to assess and mature platform capabilities iteratively over time.

## The Eight BRY Pillars

The framework is anchored by **eight architectural pillars**. Each pillar is a non-optional lens applied to every design decision. A solution is considered architecturally sound only when it has been deliberately evaluated and balanced across all eight.

| Pillar | Core Principle |
|--------|----------------|
| **1. Platform Governance** | Authority, standards, and decision rights are defined before code is written |
| **2. Configurable over Custom** | Out-of-the-box capability is exhausted before customization is approved |
| **3. Secure by Design** | Security, privacy, and compliance controls are architectural inputs, not post-delivery additions |
| **4. Performance-Aware** | Performance characteristics are designed, measured, and continuously protected |
| **5. Lifecycle Ready** | Solutions survive upgrades, ownership transitions, and organizational change |
| **6. Service-Oriented** | Capability is exposed and consumed as well-defined services aligned to CSDM |
| **7. Extensibility** | Architectures absorb future capability without breaking current consumers |
| **8. Observability** | What cannot be measured cannot be governed |

{% hint style="warning" %}
**Foundational Rule.** A design that optimizes one pillar at the expense of another is not a balanced architecture. The Technical Governance Council is responsible for explicit, documented trade-off decisions whenever pillars conflict.
{% endhint %}

## The Three Layers of the Framework

BRY is organized into three layers of progressive specificity. Each layer builds on the one below.

| Layer | Purpose | Primary Artifacts |
|-------|---------|-------------------|
| **1. Pillars** | Foundational principles and design goals | Pillar Checklists, Trade-off Registers, Principle Catalog |
| **2. Solution Units** | Application of pillars to specific ServiceNow domains (ITSM, IRM, ITOM, SPM, Custom Applications) | Solution Context, Design Areas, Best Practice Guides, Maturity Assessments |
| **3. Capability Guides** | Architectural usage patterns for individual platform features | Pattern Library, Reference Architectures, Anti-pattern Catalog |

### Layer 1: Pillars

The foundation of the framework. Each pillar page introduces **core principles** and **design goals**, followed by **recommended approaches** that serve as non-optional considerations. A **checklist** evaluates how a solution aligns with each pillar, with links to implementation guides, reference architectures, and pattern libraries.

### Layer 2: Solution Units

Each Solution Unit applies the eight pillars to a specific ServiceNow domain. Every Solution Unit page contains:

1. **Design Principles** tailored to the use case
2. **Design Areas** highlighting critical architectural decisions
3. **Best Practice Guides** per area
4. **Maturity Assessments** to benchmark solution readiness

Start with the **Solution Context**, then explore the **Design Areas** to identify where improvements or governance gaps may exist.

### Layer 3: Capability Guides

Capability Guides explain how to **design with** individual ServiceNow features, not how the features work. Each guide helps determine:

1. **When** to use a feature
2. **What** design patterns apply
3. **How** to keep usage compliant, secure, and extensible

## Adopt a Phased Learning Process

{% hint style="success" %}
**Start small. Learn fast. Scale intentionally.**
{% endhint %}

BRY is designed to evolve with your platform. It is not intended to be implemented all at once. Begin with the highest-priority pillar based on your business goals, compliance obligations, or scalability needs. As your implementation matures, expand to additional pillars. Iterate using checklists, pattern validations, and design reviews. Revisit your architectural alignment every time your platform scales, integrates, or adopts a new capability.

The phased approach works well across:

1. **Initial design and build phases**
2. **Production readiness and go-live**
3. **Scaling to enterprise-level workloads**
4. **Audit, review, and governance checkpoints**

## How BRY Compares to AWS Well-Architected

BRY borrows the **discipline** of AWS Well-Architected and applies it to the **ServiceNow context**.

| AWS Well-Architected | Build It The Right Way |
|----------------------|------------------------|
| 6 Pillars (Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability) | 8 Pillars tuned for enterprise workflow platforms |
| Lenses (Serverless, SaaS, FinServ, ML, Healthcare) | Solution Units (ITSM, IRM, ITOM, SPM, Custom Applications) |
| Well-Architected Labs | Capability Guides |
| Well-Architected Tool | BRY Assessment Toolkit |
| Review Process | BRY Control Gates (G0–G4) |

## The BRY Compact

{% hint style="info" %}
**Seven Governing Principles**

1. **Architecture leads. Delivery follows.**
2. **Configuration is a virtue. Customization is a debt.**
3. **Compliance is designed, not retrofitted.**
4. **Every decision is recorded. Every gate is honored.**
5. **Pillars are balanced. Trade-offs are explicit.**
6. **Measure what you govern. Govern what you measure.**
7. **Start small. Learn fast. Scale intentionally.**
{% endhint %}

## Related Resources

1. ServiceNow BRY Architecture Pillars *(internal — page coming)*
2. Architectural Patterns for ServiceNow *(internal — page coming)*
3. BRY Assessment Toolkit *(internal — page coming)*
4. YouTube: Build It The Right Way Series with Bill *(external link placeholder)*
5. [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/) *(reference inspiration)*
6. [ServiceNow Common Service Data Model (CSDM)](https://www.servicenow.com/community/in-other-news/csdm-service-migration-playbook-and-use-case-examples/ba-p/2977443) *(reference standard)*

---

> **Document Control**
>
> Owner: Office of the Chief Enterprise Architect · Review Cadence: Quarterly · Status: Canonical

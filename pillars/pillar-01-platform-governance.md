---
description: >-
  Pillar 01 of the Build It The Right Way framework. The operating model that
  prevents shadow customisation on ServiceNow. Architecture Review Board, four
  control gates, scope discipline, RACI, maturity
---

# Pillar 01 · Platform Governance

> **Shadow customisation is a governance problem, not a developer problem.** The developers are doing what the operating model permits. Change the operating model, the behaviour changes with it.

{% embed url="https://www.youtube.com/watch?v=3vlwvdOvWZM" %}

**Watch first.** A thirteen-minute walkthrough of this pillar. The page below is the operational reference.

## The scene this pillar prevents

A platform owner gets a call. Production is fine. No incidents. No outage. But there is a new workflow live in ITSM that nobody on the architecture team approved.

Built in three weeks by a developer reporting into operations, on the request of a service desk manager who needed it yesterday. Global scope. Writes directly to the incident table. Bypasses two ACLs. Discovered ninety days later by a regulator's question.

Nobody acted in bad faith. The platform still ended up unmaintainable.

This is **shadow customisation**, the single most expensive failure mode of the ServiceNow platform. Platform Governance is the pillar that prevents it.

## Why this is Pillar One

The framework has eight pillars. Platform Governance is first because every other pillar collapses without it.

> **Configurable over Custom** fails when anyone with developer access can write anything. **Secure by Design** fails when scope is decided in a hurry. **Lifecycle Ready** fails when half the platform was built outside the release process. **Observability** fails when nobody knows what shipped last week.

Platform Governance is not the most exciting pillar. It is the one that makes the others possible.

## The four governance questions

If your platform does not have explicit, documented, enforced answers to these four questions, you do not have governance. You have a wish.

| **Question**                         | **What it means**                                                                                                                        | **Who answers**                                                     |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| **01 · Who decides what gets built** | Not who builds it. Who decides it should be built at all.                                                                                | Architect plus product owner, together, before any story is touched |
| **02 · On what scope**               | Global, scoped application, or new application. Determines upgrade safety, security posture, lifecycle ownership for the next ten years. | Architect, at design time. Not a developer choice.                  |
| **03 · With what approval**          | Every change has a gate. Small, large, or emergency. There is no such thing as an ungoverned change.                                     | The Architecture Review Board                                       |
| **04 · With what consequence**       | If a build ships without passing the gate, what happens. Governance without consequence is a suggestion.                                 | Platform owner, with executive backing                              |

## The Architecture Review Board

An ARB is not a status meeting. It is where you ask **permission to build**.

Three properties make an ARB real. Missing any one of the three, you have a meeting.

### Composition

Five voices at the table.

1. **Architect** · pillar interpretation and design-gate sign off
2. **Platform Owner** · adoption pace, KPI delivery, and executive air cover
3. **Senior Developer** · technical feasibility and Capability Guide application
4. **Compliance Lead** · regulatory exposure
5. **Security** · optional, included when the design touches sensitive data

### Cadence

Matches your release rhythm. Ship every two weeks, the ARB meets every two weeks. Never ad hoc. **Ad hoc ARBs become bypass routes.**

### Authority

Approves or rejects. A rejected design does not ship. A rejected design that ships triggers remediation, owned by the team that shipped it.

## The four control gates

The ARB operates through four gates. Sequential. Mandatory. Documented.

| **Gate**                         | **When**                     | **What clears the gate**                                                                                      |
| -------------------------------- | ---------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Gate 01 · Design Intent**      | Before development starts    | Pillar checklist signed off by the architect. Compliance consulted. No story enters the sprint without it.    |
| **Gate 02 · Build Review**       | Mid build                    | ARB validates implementation against Solution Unit design areas. Catches the design that drifted in practice. |
| **Gate 03 · Pre-Production**     | Before deployment            | Capability Guide compliance confirmed. Risk log cleared or each open risk formally accepted in writing.       |
| **Gate 04 · Post Go-Live Audit** | Ninety days after deployment | Maturity assessment re-scored. Findings feed next quarter's priorities.                                       |

> **Caught at Gate 02, the fix is cheap. Caught at Gate 03, expensive. Caught after go-live, a project.**

## Scope discipline

The governance decision violated most often. Every artefact on the Now Platform lives in a scope. The choice is permanent.

### Global scope · the default, the trap

1. Every change can affect every other team
2. Upgrade conflicts compound silently
3. ACL bypass risk grows with the platform
4. One careless update set ripples everywhere

### Scoped application · a contract in a box

1. Upgrades independently of the platform
2. Uninstalls cleanly when retired
3. Its own ACL model, its own update set hygiene
4. A named owner, a defined lifecycle

The governance question is not _does this need to be scoped_. The question is **what is the cost of putting this in global**. If you cannot answer at design time, you are not ready to ship.

Scope is an architectural decision. Made at Gate 01. Signed off by the architect.

## Roles and ownership

Five roles. Five lanes. No overlap on decision authority.

| **Role**             | **Primary responsibility**                     | **Authority**                                                |
| -------------------- | ---------------------------------------------- | ------------------------------------------------------------ |
| **Architect**        | Pillar interpretation and design-gate sign off | Owns Gate 01 and Gate 02 decisions                           |
| **Platform Owner**   | Adoption pace and KPI delivery                 | Absorbs the political cost of an ARB rejection               |
| **Developer**        | Capability Guide application on the ground     | Raises pillar conflicts the moment they appear               |
| **Delivery Manager** | Gate enforcement inside the delivery pipeline  | Blocks stories from entering the sprint until Gate 01 clears |
| **Compliance Lead**  | Consulted at Gate 01 and Gate 03               | Has authority to escalate any regulatory exposure            |

## Three shadow customisation patterns

Three patterns I have seen on real platforms. Names changed. Architectures intact.

### Pattern 01 · The friendly developer

A capable developer reports into operations and builds workflows on request. No backlog story. No design review. No ARB visibility. The workflows are good. They are also unmaintained, undocumented, in global scope. Developer leaves. Platform owner discovers fourteen Business Rules nobody can explain.

### Pattern 02 · The vendor handoff

A system integrator finishes a project. Internal team starts making changes the SI never expected. The SI's design assumptions are not documented where the internal team would find them. The internal team's changes are not reviewed against those assumptions. Eighteen months later, a hybrid of two architectures and neither one works.

### Pattern 03 · The executive bypass

A senior executive wants a dashboard. Requires a small table extension. Built over a weekend, signed off by the executive, never sees the ARB. Breaks during the next platform upgrade. Blame goes to the upgrade. Actual cause is the bypass.

> **Three patterns. Different surfaces. Same root cause.** Governance authority was unclear, ambiguous, or ignored.

## Maturity ladder

Three levels. Locate yourself honestly.

| **Level**     | **Signal**                                                                                                                                                                                                   | **Typical timeline to next level** |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------- |
| **Reactive**  | No standing ARB. No design gates. Governance happens after the fact, when something breaks.                                                                                                                  | A quarter to reach Managed         |
| **Managed**   | ARB exists. Composition and cadence in place. Gates documented but inconsistently enforced.                                                                                                                  | A year to reach Strategic          |
| **Strategic** | ARB is the centre of how the platform evolves. All four gates run on every build. Maturity assessment re-scored every quarter. Platform Governance is no longer a project, it is a property of the platform. | The goal                           |

Both transitions require executive air cover. Neither happens by accident.

## Implement in ninety days

One pillar. One ARB. Four gates. Twelve weeks.

| **Weeks**    | **Move**        | **What clears the milestone**                                                                             |
| ------------ | --------------- | --------------------------------------------------------------------------------------------------------- |
| **1 to 2**   | Convene the ARB | Five named people. Standing meeting on your release cadence.                                              |
| **3 to 4**   | Adopt Gate 01   | Every new build walks the pillar checklist at design time. Architect signs off in writing. No exceptions. |
| **5 to 6**   | Adopt Gate 02   | Mid-build review running. ARB validates implementation against Solution Unit design areas.                |
| **7 to 10**  | Adopt Gate 03   | Pre-production risk log discipline. Written acceptance of open risks by the platform owner.               |
| **11 to 12** | Adopt Gate 04   | Post go-live audit cadence set. Maturity re-score scheduled in ninety days.                               |

The first ten Gate 01 reviews will be slow. They get faster. By week twelve the team is operating the framework, not having it imposed on them.

## Governance health · architect's self-check

Score your platform on each. Three or more **No** answers and you are on the Reactive side of the ladder.

1. Is there a named ARB with all five roles seated
2. Does the ARB meet on your release cadence, not ad hoc
3. Has the ARB ever rejected a design in the last two quarters
4. Does every new build walk a pillar checklist before entering the sprint
5. Is there a written record of every open risk accepted by the platform owner
6. Was the maturity assessment re-scored in the last ninety days
7. Can you name the scope of every customisation shipped in the last release

## Next in the series

**Pillar 02 · Configurable over Custom.** Why custom code is the last resort, never the default. Coming next in the Build It The Right Way pillar series.

***

_Authored by Bill Martin · ServiceNow MVP 2026 · Certified Technical Architect ·_ [_techtalkwbill_](https://www.youtube.com/@techtalkwbill)

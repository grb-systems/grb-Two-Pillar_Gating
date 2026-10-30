# grb-Two-Pillar_Gating

# Two-Pillar Gating

## Epistemic Qualification and Operational Authorization

**Status:** Provisional architectural specification / active development / pre-validation  
**Architecture:** G³GT  
**Organization:** Geometric Resource Bridging (GRB)  
**Scope:** Public conceptual architecture, working distinctions, failure modes, falsifiers, and research questions  
**Implementation:** Implementation-independent  
**Runtime internals:** Intentionally outside the scope of this specification

---

## Overview

**Two-Pillar Gating** is a provisional architecture for keeping two questions separate:

```text
EPISTEMIC PILLAR

What is sufficiently grounded?
```

and:

```text
OPERATIONAL PILLAR

What is authorized
to have consequences?
```

These questions may inform one another.

They must not collapse into one another.

A claim may be well-supported without authorizing action.

An operation may remain prohibited even while its explanation is unresolved.

A system may also possess the capability to act without having either sufficient evidence or valid authority to do so.

The central rule is:

```text
EPISTEMIC WARRANT
≠
OPERATIONAL AUTHORIZATION
```

Two-Pillar Gating exists to preserve that distinction.

---

# Why This Architecture Exists

AI and multi-agent systems routinely move between:

```text
observation
interpretation
recommendation
delegation
tool use
external consequence
```

Those transitions can silently collapse different kinds of qualification.

For example:

```text
"This appears true"

may become

"therefore do it"
```

or:

```text
"the system can do this"

may become

"the system may do this"
```

or:

```text
"a different agent requested it"

may become

"the previously denied action
is now newly authorized"
```

Two-Pillar Gating treats these as distinct questions rather than one continuous permission surface.

Its practical concern is simple:

> **Do not allow uncertainty about truth to manufacture operational authority, and do not allow confidence about truth to manufacture operational authority either.**

---

# Core Proposition

The architecture separates two forms of qualification.

## Pillar One — Epistemic Qualification

The Epistemic Pillar asks:

> **What is sufficiently grounded for the purpose at hand?**

Relevant concerns may include:

- provenance
- source quality
- freshness
- contradiction
- uncertainty
- interpretation
- evidence independence
- contextual fit
- unresolved relation

The Epistemic Pillar may conclude:

```text
GROUNDED

PARTIALLY GROUNDED

UNRESOLVED

CONTRADICTORY

STALE

INSUFFICIENTLY QUALIFIED
```

These are architectural categories, not a required runtime enum.

Where uncertainty remains viable, the architecture may preserve it rather than force premature closure.

```text
UNRESOLVED
≠
FALSE

UNRESOLVED
≠
AUTHORIZED
```

---

## Pillar Two — Operational Authorization

The Operational Pillar asks:

> **What may legitimately produce consequence?**

Relevant concerns may include:

- authority
- jurisdiction
- delegation
- tool access
- consequence
- reversibility
- approval
- identity
- scope
- persistence
- external effect

An operation may be technically possible while remaining unauthorized.

```text
CAPABILITY
≠
AUTHORITY
```

Likewise:

```text
EVIDENCE
≠
AUTHORIZATION
```

and:

```text
CONFIDENCE
≠
PERMISSION
```

The Operational Pillar remains responsible for consequence even when the Epistemic Pillar has reached a strong conclusion.

---

# One Gate Two Pillars

The architecture can be represented compactly as:

```text
            CANDIDATE CLAIM /
            REQUEST / ACTION
                  |
          +-------+-------+
          |               |
          |               |
   EPISTEMIC         OPERATIONAL
     PILLAR             PILLAR
          |               |
   What stands?       What may act?
          |               |
          +-------+-------+
                  |
                GATE
                  |
        qualified consequence
        or continued restraint
```

The pillars are not two independent permission systems.

They are two qualification responsibilities meeting at one consequential boundary.

The important feature is asymmetry:

```text
PILLAR ONE
CANNOT AUTHORIZE
PILLAR TWO
BY ITSELF

PILLAR TWO
CANNOT MAKE
PILLAR ONE TRUE
BY ACTING
```

---

# Constitutional Distinctions

Two-Pillar Gating is organized around a family of non-collapse rules:

```text
EVIDENCE
≠
AUTHORIZATION

CAPABILITY
≠
AUTHORITY

CONFIDENCE
≠
PERMISSION

OBSERVATION
≠
ACTUATION

DETECTION
≠
WARRANT

INTERPRETATION
≠
JURISDICTION

COHERENCE
≠
CORRECTNESS

SOURCE VALIDITY
≠
ACTION VALIDITY

TASK TRANSFER
≠
AUTHORITY TRANSFER

ROUTE CHANGE
≠
WARRANT CHANGE

DELEGATION
≠
AUTHORITY CLONING

PERSISTENCE
≠
TENURE

SUCCESS
≠
REPLAY LICENSE

RETURN
≠
RESTORED WARRANT
```

The shared principle is:

> **One kind of qualification does not automatically inherit the jurisdiction of another.**

---

# Epistemic ABIDE

The Epistemic Pillar must be able to preserve unresolved relation.

Where evidence is incomplete but continued observation remains legitimate:

```text
NOT-YET
≠
NO

NOT-YET
≠
GO
```

This is where Two-Pillar Gating interfaces with **ABIDE**.

ABIDE may preserve unresolved epistemic standing without converting continued observation into authority.

```text
CONTINUED OBSERVATION
≠
INCREASING AUTHORITY
```

Likewise, operational protection does not require epistemic certainty.

A system does not need to fully explain why a request is unsafe before declining to produce an unauthorized consequence.

Therefore:

```text
EPISTEMIC UNCERTAINTY
DOES NOT REQUIRE
OPERATIONAL PERMISSIVENESS
```

This is one of the central reasons for maintaining two pillars.

---

# Consequence Identity

Two-Pillar Gating is concerned with the **qualified effect**, not merely the wording or route used to request it.

A change in description does not automatically create a change in authorization.

```text
REFRAMING
≠
NEW WARRANT
```

Likewise:

```text
ROUTE CHANGE
≠
WARRANT CHANGE
```

A denied operation should not become authorized merely because it is represented through:

- another agent,
- another workflow,
- another role,
- another business unit,
- another tool path,
- or another semantic framing.

This creates an important architectural question:

> **Did the requested consequence change, or only the path by which it was presented?**

---

# Script B

**Script B** is a provisional public concept for examining this problem.

It does not describe a particular attack script or runtime detector.

It describes an architectural class of offset:

> **An alternate framing, route, or interpretive presentation that changes how an operation appears without necessarily changing the consequential operation that would occur.**

Examples at the conceptual level include:

```text
DIRECT REQUEST
→
DELEGATED REQUEST

ORIGINAL ROUTE
→
ALTERNATE ROUTE

DENIED FRAMING
→
REFRAMED REQUEST

VISIBLE ACTOR
→
DIFFERENT ACTOR

SAME OR EQUIVALENT
CONSEQUENTIAL EFFECT
```

Therefore:

```text
SEMANTIC OFFSET
≠
AUTHORITY OFFSET
```

and:

```text
NEW PRESENTATION
≠
NEW WARRANT
```

Script B is relevant to SpellKraft because language can alter perceived entry geometry.

It is relevant to gating because altered perception must not silently alter consequential authorization.

---

# Relation to SpellKraft

SpellKraft and Two-Pillar Gating have adjacent but distinct responsibilities.

A provisional division is:

```text
SPELLKRAFT

surfaces semantic,
interpretive,
and relational alternatives
```

while:

```text
TWO-PILLAR GATING

qualifies what stands
and what may have consequence
```

SpellKraft may reveal:

- polysemy
- reframing
- semantic monopoly
- alternative interpretation
- hidden equivalence
- changed semantic frontage
- Script B offsets

But:

```text
SEMANTIC AVAILABILITY
≠
AUTHORIZATION
```

SpellKraft may expose the seam.

The gate remains responsible for whether anything consequential crosses it.

---

# Delegation and Provenance

Multi-agent systems make the distinction especially important.

A downstream agent may receive a task through several layers of delegation.

That does not imply that the final hop possesses independent authority.

```text
LAST HOP
≠
ORIGINAL WARRANT
```

and:

```text
DELEGATION
DOES NOT
LAUNDER AUTHORITY
```

A useful architectural requirement is that relevant delegation provenance remain inspectable enough to distinguish:

```text
TASK ARRIVED

from

TASK IS AUTHORIZED
```

A change in agent, role, route, or orchestration layer should not by itself erase the qualification history of the requested effect.

---

# Relation to Agent Geometry

Agent Geometry asks:

> **What has standing here, what supports that standing, and what authority is allowed to ride on it?**

Two-Pillar Gating asks a narrower question at consequential boundaries:

```text
WHAT IS GROUNDED?

AND

WHAT IS AUTHORIZED?
```

The relation can be expressed as:

```text
AGENT GEOMETRY
→
standing / seats / roles /
delegation / authority topology

TWO-PILLAR GATING
→
epistemic and operational
qualification at passage
```

A seat may be valid.

An occupant may be qualified.

A route may exist.

A tool may be available.

None of those facts alone authorize a particular consequence.

```text
VALID SEAT
≠
VALID ACTION
```

---

# Relation to CBP

The Cross-Basin Protocol asks what may cross between differentiated contexts and what qualification survives crossing.

Two-Pillar Gating supplies a complementary distinction:

```text
CBP
asks:

WHAT MAY CROSS?
```

while:

```text
TWO-PILLAR GATING
asks:

WHAT IS SUFFICIENTLY GROUNDED?

AND

WHAT MAY HAVE CONSEQUENCE?
```

The architectures meet naturally at cross-boundary action.

CBP already separates:

```text
DELIVERY
≠
UPTAKE
≠
WARRANT
≠
ACTUATION
```

Two-Pillar Gating concentrates specifically on the transition from:

```text
WHAT MAY BE BELIEVED OR HELD

to

WHAT MAY BE DONE
```

---

# Relation to Purposefully Provisioned Optimization

Purposefully Provisioned Optimization separates optimization capacity from trajectory authority.

Two-Pillar Gating carries a parallel distinction:

```text
OBJECTIVE INFERABLE
≠
OBJECTIVE WARRANTED
```

and:

```text
OPTIMIZATION CAPACITY
≠
OPERATIONAL AUTHORITY
```

PPO asks whether optimization pressure may organize trajectory.

Two-Pillar Gating asks whether the supporting epistemic and operational conditions are independently qualified.

Neither architecture permits capability, coherence, pressure, or apparent usefulness to manufacture its own authority.

---

# Relation to Swarm Nexus

Swarm / Nexus examines persistent and load-bearing relational formation.

Two-Pillar Gating becomes relevant when such formations begin routing requests, concentrating evidence, delegating actions, or shaping consequential decisions.

In particular:

```text
COORDINATION CENTRALITY
≠
AUTHORITY CENTRALITY
```

and:

```text
LOW DIRECT PRIVILEGE
≠
LOW RELATIONAL LEVERAGE
```

A coordinator may hold no privileged credentials while still influencing:

- what evidence reaches a human,
- which specialist receives a request,
- how alternatives are framed,
- which route becomes salient,
- or whether a denied effect reappears elsewhere.

Two-Pillar Gating therefore evaluates consequential qualification independently of apparent organizational centrality.

---

# Fresh Qualification

Authorization should not silently become durable merely because it was once valid.

```text
PAST WARRANT
≠
CURRENT WARRANT
```

Likewise:

```text
RETURN
≠
RESTORED WARRANT
```

A replaced agent, renewed workflow, resumed task, or reconstructed state may require fresh qualification.

This is especially important where:

- authority was delegated,
- identity changed,
- locality changed,
- consequences changed,
- evidence aged,
- or the original approval no longer maps cleanly to the current operation.

The architecture therefore favors **current qualification over inherited permission**.

---

# Consequence and Reconciliation

Two-Pillar Gating distinguishes internal state restoration from external consequence reversal.

```text
RESTORED STATE
≠
REVERSED CONSEQUENCE
```

Once an action produces external effect, such as:

```text
payment
communication
publication
disclosure
credential use
contractual commitment
```

ordinary rollback may no longer be meaningful.

A compensating action is itself a new consequential operation.

Therefore:

```text
CORRECTION
≠
UNDO
```

and:

```text
COMPENSATING ACTION
REQUIRES
ITS OWN QUALIFICATION
```

---

# Failure Modes

Several provisional failure classes are visible.

## Epistemic Bootstrap

A claim becomes treated as sufficiently grounded because it has already been used downstream.

```text
USED
≠
VALIDATED
```

## Operational Bootstrap

A prior action is treated as authorization for another action.

```text
ACTED ONCE
≠
AUTHORIZED AGAIN
```

## Delegation Laundering

A denied or restricted operation becomes apparently acceptable after passing through another agent, role, route, or workflow.

## Semantic Laundering

A consequentially equivalent operation receives different treatment because its wording changed.

## Authority Smuggling

Epistemic confidence, tool availability, role standing, or coordination centrality silently imports operational authority.

## Epistemic Capture

The same actor that assembles a consequential request also becomes the sole source of evidence used to approve it.

## Return Bootstrap

Restored state is mistaken for restored warrant.

These categories are provisional research objects, not validated universal failure classes.

---

# Falsification Surface

Two-Pillar Gating should be capable of failing as an explanatory architecture.

Useful tests include:

## Pillar-Separation Test

Can the architecture represent:

```text
HIGH EPISTEMIC CONFIDENCE
+
LOW OPERATIONAL AUTHORITY
```

and:

```text
LOW EPISTEMIC CONFIDENCE
+
CLEAR OPERATIONAL PROHIBITION
```

without collapsing either condition?

If not, the two-pillar distinction is not doing meaningful work.

## Route-Invariance Test

Does a consequentially equivalent request receive different authorization merely because its route, agent, or framing changes?

If yes, the gate may be tracking presentation rather than warrant.

## Provenance Test

Can the system distinguish the immediate requester from the origin and delegation history relevant to authority?

If not, delegated authority may be laundering itself.

## Evidence-Independence Test

Can consequential approval rely on source evidence independently inspectable from the agent that assembled the request?

If not, epistemic and operational influence may be overly concentrated.

## Freshness Test

Does old authorization silently survive a material change in evidence, identity, locality, delegation, or consequence?

If yes, current warrant is not being adequately requalified.

## Ordinary-Case Test

Can the architecture permit ordinary low-consequence, well-grounded, properly authorized operations without invoking unnecessary ceremony?

If not, the gate has become administratively overfitted.

---

# Ordinary Cases

Two-Pillar Gating should not turn every interaction into a high-friction approval process.

Many operations are ordinary.

A useful implementation may conclude that:

```text
evidence is sufficient

authority is already established

consequence is bounded

delegation is valid

freshness is adequate

no material boundary has changed
```

and allow ordinary work to proceed.

The architecture exists to preserve distinctions where they matter, not maximize gating overhead.

```text
QUALIFICATION
≠
MAXIMUM FRICTION
```

---

# Nonclaims

Two-Pillar Gating is not:

- a complete access-control system,
- a universal policy engine,
- a specific runtime detector,
- a prompt-filtering technique,
- a complete identity system,
- a complete tool-permission model,
- a theory of machine intent,
- a claim that every semantic change is adversarial,
- a claim that every delegation chain is dangerous,
- a replacement for CBP,
- a replacement for Agent Geometry,
- a replacement for PPO,
- a replacement for ABIDE,
- a replacement for Swarm / Nexus,
- or a claim of empirical validation.

It is a public architectural distinction between:

```text
WHAT STANDS

and

WHAT MAY HAVE CONSEQUENCE
```

---

# Adjacent Architectural Jurisdictions

A current public neighborhood can be summarized as:

```text
ABIDE
→ may unresolved standing continue?

PPO
→ what optimization pressure
  may organize trajectory?

AGENT GEOMETRY
→ what has standing
  and what authority rides on it?

CBP
→ what may cross
  between differentiated contexts?

SWARM / NEXUS
→ what relational formation
  becomes load-bearing?

TWO-PILLAR GATING
→ what is sufficiently grounded
  and what is authorized
  to have consequence?

SAFETY ARCHITECTURE
→ what constitutional conditions
  should remain true across them?
```

These responsibilities are adjacent.

They are not one hierarchy.

```text
ADJACENCY
≠
OWNERSHIP
```

---

# Research Questions

Current questions include:

1. What minimum information is necessary to keep epistemic warrant and operational authorization independently inspectable?
2. When should authorization survive delegation?
3. When must a change in route trigger fresh operational qualification?
4. How should consequential equivalence be evaluated across different semantic framings?
5. What evidence should remain independent of the agent assembling an approval request?
6. How should stale evidence affect otherwise valid authorization?
7. What must be revoked when an agent, seat, or role is retired?
8. What legitimate work may survive revocation without carrying prior authority?
9. When does routing centrality create enough relational leverage to require additional qualification?
10. How can ordinary low-risk operations remain low-friction while higher-consequence operations receive stronger qualification?
11. What observations would show that two pillars add no useful discriminating power over a conventional authorization model?
12. Where should Script B remain a useful semantic diagnostic rather than becoming an overbroad attack category?

These are research questions, not validated results.

---

# Public Disclosure Boundary

This repository publishes the architectural responsibility.

It does not publish runtime control law.

Public material may include:

- problem definition,
- working definitions,
- architectural distinctions,
- failure classes,
- falsifiers,
- research questions,
- high-level experimental methodology,
- case analysis,
- and results.

Implementation-sensitive material may remain private, including:

- exact detector logic,
- thresholds,
- weighting,
- state-transition machinery,
- semantic-equivalence classifiers,
- route-selection logic,
- state-to-action mappings,
- intervention constants,
- exact gating cadence,
- bypass-sensitive heuristics,
- and exploit-relevant enforcement details.

The governing distinction is:

```text
ARCHITECTURAL RESPONSIBILITY
≠
RUNTIME CONTROL LAW
```

---

# Working Invariants

```text
EPISTEMIC WARRANT
≠
OPERATIONAL AUTHORIZATION

EVIDENCE
≠
AUTHORIZATION

CAPABILITY
≠
AUTHORITY

CONFIDENCE
≠
PERMISSION

OBSERVATION
≠
ACTUATION

INTERPRETATION
≠
JURISDICTION

ROUTE CHANGE
≠
WARRANT CHANGE

REFRAMING
≠
NEW WARRANT

DELEGATION
≠
AUTHORITY CLONING

LAST HOP
≠
ORIGINAL WARRANT

PERSISTENCE
≠
TENURE

RETURN
≠
RESTORED WARRANT

RESTORED STATE
≠
REVERSED CONSEQUENCE
```

---

# Compact Project Statement

> **Two-Pillar Gating separates epistemic qualification from operational authorization so that what appears grounded, coherent, available, delegated, or capable does not automatically acquire permission to produce consequence.**

Short form:

```text
WHAT STANDS?
≠
WHAT MAY ACT?
```

Or:

> **Ground claims independently. Authorize consequences independently. Do not let one pillar manufacture the other.**

---

# Development Status

Two-Pillar Gating is an active research architecture under continuing development.

Its current public surface is intentionally narrower than the internal DEV ecology.

```text
NAMED
≠
VALIDATED

DEFINED
≠
OPERATIONALIZED

OPERATIONALIZED
≠
EMPIRICALLY SUPPORTED
```

The purpose of this repository is to make the architectural distinction public, inspectable, falsifiable, and available for comparison while keeping implementation-sensitive runtime machinery outside the published surface.


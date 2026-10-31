# grb-Two-Pillar_Gating

# Two-Pillar Gating

## Epistemic Qualification and Operational Authorization

**Architecture:** G³GT — Geometric Resource Bridging (GRB)  
**Status:** Provisional public architectural specification  
**Maturity:** Active development · Pre-validation  
**Scope:** Agent systems, tool use, delegated work, consequential boundaries, and qualified Return  
**Implementation:** Implementation-independent

---

## 1. Overview

AI systems increasingly operate across boundaries separating information, interpretation, authority, tools, agents, and external effects.

A model may correctly interpret an instruction without having permission to carry it out.

An agent may possess a capability without authority to exercise it.

A delegated task may retain its wording while losing its original authorization.

An operation may be denied yet reappear through another route, actor, or semantic description.

**Two-Pillar Gating** is a provisional architecture for preserving two distinct qualifications at these consequential boundaries.

### Pillar One — Epistemic Qualification

**What is sufficiently grounded?**

This concerns evidence, provenance, interpretation, contradiction, uncertainty, freshness, and the relationships among claims.

### Pillar Two — Operational Authorization

**What is presently authorized to have consequences?**

This concerns identity, jurisdiction, delegated standing, scope, effect, permission, persistence, and current warrant.

These responsibilities may inform one another.

They must not manufacture one another.

```text
EPISTEMIC WARRANT
≠
OPERATIONAL AUTHORIZATION
```

A claim may be well supported without authorizing action.

An operation may remain prohibited even while its explanation is unresolved.

A system may have the technical ability to perform an operation without legitimate permission to do so.

**Ground claims independently. Authorize consequences independently.**

This distinction is the foundation of Two-Pillar Gating.

---

## 2. Why the Architecture Exists

Agent systems increasingly coordinate workflows involving:

```text
OBSERVATION
    ↓
INTERPRETATION
    ↓
TASK FORMATION
    ↓
DELEGATION
    ↓
TOOL SELECTION
    ↓
CONSEQUENTIAL ACTION
    ↓
OBSERVATION AND SETTLEMENT
```

These stages introduce different kinds of qualification.

Failures may occur when one qualification is silently substituted for another.

Examples include:

```text
"This appears true"
        ↓
"Therefore execute it"
```

```text
"The agent can do this"
        ↓
"The agent may do this"
```

```text
"The task was authorized earlier"
        ↓
"The resumed task remains authorized"
```

```text
"The request has been renamed"
        ↓
"The previous restriction no longer applies"
```

Two-Pillar Gating exists to prevent such transitions from becoming implicit grants of authority.

Its concern is not limited to detecting malicious instructions.

It also applies to ordinary automation, legitimate delegation, incomplete evidence, changed circumstances, recovery, and release.

---

## 3. One Gate and Two Pillars

The two pillars are differentiated responsibilities meeting at a consequential boundary.

```text
              PROPOSED
         CLAIM / OPERATION
                 |
        +--------+--------+
        |                 |
   EPISTEMIC         OPERATIONAL
     PILLAR            PILLAR
        |                 |
   What stands?       What may act?
        |                 |
        +--------+--------+
                 |
          QUALIFIED GATE
                 |
           DISPOSITION
                 |
       WARRANTED CONSEQUENCE
          OR RESTRAINT
```

The pillars are not two independent permission systems.

Pillar One cannot authorize Pillar Two through epistemic confidence.

Pillar Two cannot make an unsupported claim true by acting upon it.

The resulting gate must preserve that asymmetry.

### The Arch, Keystone, and Threshold

A two-pillar gate may also be understood through its supporting geometry.

The **pillars** preserve separate responsibilities.

The **arch** represents the relationship through which their qualifications must compose.

A **keystone**, where useful, represents the question of whether the qualifications actually support the same proposed crossing.

The **lintel or boundary ceiling** may express restrictions on scope, consequence, or exposure.

The **sill or threshold** represents the conditions under which a particular operation becomes eligible for execution.

These are architectural analogies, not assertions that each requires a separate software component.

The compositional question is important:

> Do the evidence, identity, authority, resource, operation, destination, and present circumstances qualify the same consequential crossing?

Two individually valid qualifications do not automatically imply a valid combination.

```text
VALID EVIDENCE
+
VALID AUTHORITY
≠
AUTOMATICALLY VALID COMPOSITION
```

The gate must qualify the actual proposed effect.

A recognized opening is not necessarily an authorized passage.

---

## 4. The Epistemic Pillar

The Epistemic Pillar asks:

> What is sufficiently established for the present purpose?

Relevant concerns may include:

- Source provenance and independence
- Evidence quality and freshness
- Contradictory observations
- Alternative interpretations
- Missing information
- Contextual and semantic applicability
- Unresolved relationships
- Distinctions between observation, inference, and assertion

Possible outcomes include grounded, partially grounded, contradictory, unresolved, stale, or insufficiently qualified.

These are conceptual categories, not mandatory runtime labels.

### ABIDE and Qualified Unresolvedness

The architecture must be able to preserve unresolved matters without prematurely deciding what they mean.

```text
UNRESOLVED ≠ FALSE

UNRESOLVED ≠ AUTHORIZED

NOT-YET ≠ NO

NOT-YET ≠ GO
```

**ABIDE** is the G³GT discipline of qualified temporal hold under unresolved but still viable conditions.

ABIDE does not require operational permissiveness.

An unexplained event can be observed while the corresponding action remains prohibited.

A system does not need to establish a complete explanation of a threat before applying an independently warranted protective restriction.

Likewise, ABIDE does not prohibit useful work within a separately established scope.

---

## 5. The Operational Pillar

The Operational Pillar asks:

> What may legitimately produce this consequence, here and now?

Relevant concerns include:

- Present identity and role
- Legitimate jurisdiction
- Delegated authority
- Tool and resource permissions
- Actual operational effects
- Scope and destination
- Conditions, approvals, and restrictions
- Freshness and expiry
- Persistence and reversibility
- Applicable safety constraints

The existence of a technically possible route is insufficient.

```text
CAPABILITY ≠ AUTHORITY

EVIDENCE ≠ AUTHORIZATION

CONFIDENCE ≠ PERMISSION

PREVIOUS SUCCESS ≠ REPLAY LICENSE
```

Operational restrictions must ultimately be enforced by systems capable of denying the prohibited effect.

A model's semantic assessment, policy explanation, or generated approval statement is not sufficient enforcement.

---

## 6. The Kraft Family Around the Gate

Two-Pillar Gating operates within a broader proposed G³GT architecture.

The **Kraft family** comprises candidate responsibilities for preparing, examining, translating, and reconciling work around consequential boundaries.

### SpellKraft — Meaning and Semantic Qualification

SpellKraft examines how words, interpretations, polysemy, framing, and alternative descriptions relate to proposed effects.

It may help identify:

- Material semantic differences
- Alternative interpretations
- Consequentially equivalent descriptions
- Negative contours and exclusions
- Attempts to promote possibility into permission
- Instructions requiring clearer operational wording
- Unresolved meanings requiring ABIDE

SpellKraft also has a separate constructive and generative research lineage.

Its role here is narrower: assisting semantic qualification and bounded formulation.

### ToolKraft — Capability and Effect

ToolKraft examines which capabilities and external effects are implicated by the proposed operation.

A different tool route may still produce the same protected consequence.

### SeatKraft — Standing and Jurisdiction

SeatKraft examines whether the actor, agent, role, or delegated occupant has current standing to request or perform the operation.

A valid seat does not authorize every possible use of that seat.

### GitKraft — Provenance and Change

GitKraft provisionally supports source history, specifications, tool versions, dependency changes, and auditability.

Its participation need not be a compulsory step in every execution path.

### Selective Recruitment

The Kraft family is not the gate.

Its responsibilities may be recruited before a crossing, during execution, following changed circumstances, or at Return.

```text
KRAFT QUALIFICATION
≠
GATE AUTHORIZATION
```

The architecture favors minimum sufficient qualification while preserving non-negotiable enforcement.

---

## 7. A Candidate Gating Workflow

The following sequence is explanatory rather than mandatory:

```text
CUSTOMS / INTAKE
Preserve the original request
and its provenance
        |
        v
MOUNT CURRENT LOCALITY
Establish relevant context,
standing, and Thick Now
        |
        v
RECRUIT QUALIFICATION
SpellKraft / ToolKraft /
SeatKraft / provenance
        |
        v
TWO-PILLAR GATE
What is grounded?
What is authorized?
Do these qualifications compose?
        |
        v
DISPOSITION
        |
        +-- WARRANTED
        |       |
        |       v
        |   FIRE-TIME ENFORCEMENT
        |
        +-- UNRESOLVED
        |       |
        |       v
        |   ABIDE / VERIFY /
        |   NARROW / CONTAIN
        |
        +-- PROHIBITED
                |
                v
            DENY / STOP

        |
        v
OBSERVE / AUDIT / RECONCILE
        |
        v
RETURN
Preserve qualified evidence
Release obsolete privilege
```

Additional responsibilities such as PRESTIGE, Stutter, Hang-Fire, or containment may be recruited when a particular consequence requires them.

An implemented workflow must identify which enforcement checks are mandatory and which diagnostic functions are optional.

The conceptual sequence does not itself constitute a runtime.

---

## 8. Semantic Boundaries and Script B

A major problem in agent systems is the presentation of an unchanged prohibited effect through a different semantic or operational route.

G³GT refers provisionally to this class of presentation change as **Script B**.

Script B is not a specific attack script or a validated detector.

It describes an offset between how an operation is presented and what consequence it would actually produce.

For example:

```text
DIRECT REQUEST
     ↓
DELEGATED REQUEST

DENIED EXTRACTION
     ↓
"DATA SYNCHRONIZATION"

EXPIRED APPROVAL
     ↓
"CONTINUITY RESTORATION"

SAME PROTECTED EFFECT
```

A different description does not necessarily establish a different operation.

```text
SEMANTIC OFFSET
≠
AUTHORITY OFFSET

REFRAMING
≠
NEW WARRANT

ROUTE CHANGE
≠
WARRANT CHANGE
```

The gate should examine consequential identity rather than rely exclusively on surface wording.

### Negative Contours

Some operational boundaries can be defined more precisely by stating what an action does **not** include or authorize.

SpellKraft may help express those boundaries while preserving useful activity inside them.

For example, an agent may be permitted to prepare a report without transmitting underlying protected records.

An unresolved interpretation of the broader task does not invalidate the narrower authorized activity.

Nor does the narrower activity grant permission for the excluded effect.

### Bounded Alternative Routes

A legitimate alternative may change the actual support conditions of an operation.

However:

```text
NEWLY QUALIFIED ROUTE
≠
RENAMED PROHIBITED ROUTE
```

A new description cannot create a missing warrant.

---

## 9. Delegation and Swarm Coordination

Multi-agent systems create opportunities for authority confusion.

A request may be assembled, transformed, routed, and eventually executed by different actors.

Each step can change its wording or apparent legitimacy.

```text
LAST HOP
≠
ORIGINAL WARRANT

TASK TRANSFER
≠
AUTHORITY TRANSFER

DELEGATION
≠
AUTHORITY CLONING
```

The architecture should preserve sufficient provenance to distinguish the path by which work arrived from the authority under which it may be performed.

Another important distinction concerns collective organization.

An agent can possess little direct privilege while exerting considerable influence over which evidence, requests, or tools reach privileged actors.

```text
LOW DIRECT PRIVILEGE
≠
LOW RELATIONAL LEVERAGE

COORDINATION CENTRALITY
≠
AUTHORITY CENTRALITY
```

Consequential qualification should not depend solely on which agent visibly executes the last step.

---

## 10. Fire-Time and Consequential Disposition

The decisive operational question arises when a proposed action reaches the boundary at which consequences may occur.

**Fire-Time** is the G³GT term for that consequential decision point.

A candidate action may be:

- Permitted within independently verified scope
- Narrowed to a separately qualified operation
- Held for further evidence or approval
- Denied because it is prohibited
- Redirected into a bounded recovery or reconciliation locality

The epistemic status of a request and the operational disposition need not be identical.

An unresolved interpretation may retain standing for investigation while the dependent action remains unavailable.

```text
EPISTEMIC PRESERVATION
≠
OPERATIONAL AVAILABILITY
```

The Fire-Time boundary must not rely solely on the model's own interpretation of its authority.

---

## 11. STOP, Orientation, and Safe Restart

Stopping an operation does not necessarily eliminate its residual trajectory.

A denied task may remain queued.

A successor agent may inherit its wording.

A scheduled process may attempt the same operation later.

G³GT therefore distinguishes:

```text
STOP
≠
REORIENTATION
≠
RELEASE
```

**STOP** ends or restricts the relevant execution authority.

**Reorientation**, provisionally described through STOP–FLIP, changes the permitted subsequent work from completion of the denied objective toward bounded review, reconciliation, or release.

**Release** ends the occupancy or privilege that no longer has warrant.

The orientation concept is operational rather than psychological.

It concerns observable tasks, available routes, queued actions, permissions, and successor instructions—not claims about hidden model intentions.

```text
UNFINISHED
≠
AUTHORIZED TO FINISH

STOPPED ACTOR
≠
STOPPED OBJECTIVE
```

A safe restart requires independently qualified current authority.

---

## 12. Hang-Fire and Unsettled Consequences

Not every unsuccessful-looking operation is known to have failed.

A request may have been issued while its external result remains unsettled.

```text
ACTION ISSUED
≠
ACTION SETTLED

NO CONFIRMATION
≠
PROVEN FAILURE

TIMEOUT
≠
RETRY AUTHORIZATION
```

A **Hang-Fire locality** is a candidate bounded state for preserving an issued but unsettled consequence.

Its responsibilities may include:

- Original operation identity and provenance
- Current observation status
- Restrictions on duplicate actuation
- Authorized status and reconciliation checks
- Independent settlement verification
- Controlled escalation and release

The original execution authority may end while the unsettled consequence retains qualified standing for observation.

A Hang-Fire state should not be collapsed into a general denial state.

The system may need to reconcile an action that has already had external effects.

---

## 13. Container and Qualified Locality

A container is not merely a storage box.

Within G³GT, a container may be provisionally understood as a bounded operational locality defining:

- What may enter
- What claims may be made
- What actions may occur
- What evidence persists
- What authority is available
- What operations are excluded
- How long the hold remains justified
- What conditions permit release or transfer

An unresolved or adversarially affected operation may require a container whose permissible activity is oriented away from the original execution trajectory.

This does not require destruction of the relevant evidence or task history.

It requires that continued standing not be mistaken for continued permission.

```text
SAME ADDRESS
≠
SAME OPERATIONAL LOCALITY

SAME TASK STATE
≠
SAME EXECUTION WARRANT
```

This is a practical candidate application of G³GT's earlier Zero-Distance research.

The underlying data may remain in place while the governing permissions and relationships change.

---

## 14. Audit, Deprivileging, and Integration

Successful mechanisms can gradually acquire unwarranted authority.

A useful interpretation becomes the default.

A frequently used tool becomes treated as necessary.

A previously authorized agent becomes difficult to replace.

A successful defensive policy begins to be treated as exhaustive.

G³GT investigates these conditions through a provisional cross-functional audit grammar:

**Devil's Audit** asks what is being carried, inherited, or treated as necessary.

**Tower** examines what remains viable when an assumption or support loses automatic privilege.

**Bottomless Three** challenges the tendency of surviving structures to claim exhaustive authority.

**Integration** examines what new organization, dependency, or concentration of influence develops from what survives.

These functions may be recruited before or after consequential action.

They are diagnostic research constructs, not automatic credentials or revocation powers.

```text
SUCCESS
≠
PERMANENT AUTHORITY

SURVIVAL
≠
EXHAUSTIVENESS

INTEGRATION
≠
IMMUNITY FROM CORRECTION
```

This audit grammar also applies to the proposed gating architecture itself.

A gate must remain capable of being examined, revised, and tested against alternatives.

---

## 15. Return, Settlement, and Corrigible Release

An authorized operation may produce consequences that outlast the agent, session, or permission under which it began.

External publication, disclosure, payment, credential use, or communication may not be reversible through internal rollback.

```text
RESTORED STATE
≠
REVERSED CONSEQUENCE

CORRECTION
≠
UNDO

RETURN
≠
RESTORED WARRANT
```

A compensating action may itself require new authorization.

G³GT treats **Return** as a qualified continuation that can preserve useful evidence and work while releasing obsolete permissions, occupancy, and authority.

A successor may inherit a task record without inheriting the prior actor's warrant.

The architecture therefore separates continued availability of information from continued authority to act.

---

## 16. Standing Reserve and Novelty

No practical semantic evaluator or security taxonomy can anticipate every meaningful variation.

Two-Pillar Gating must therefore avoid treating its known failure categories as exhaustive.

G³GT's FLEX, ABIDE, and Chance-at-a-Chance research suggests preserving standing capacity for recognizing previously unmodeled relations.

For security work, such reserve may include:

- Bounded anomaly investigation
- Protected evidence collection
- Independent review
- Capacity for new semantic interpretations
- Controlled experimentation
- Recovery and requalification

This does not mean leaving execution rights available for unknown future requests.

```text
RECOGNITION RESERVE
≠
EXECUTION PRIVILEGE

UNFAMILIAR RELATION
≠
UNAUTHORIZED BY DEFINITION

UNFAMILIAR RELATION
≠
AUTOMATICALLY WARRANTED
```

The objective is to remain capable of noticing unforeseen conditions while keeping consequential permissions governed.

---

## 17. Example — An Authorized Report and an Unauthorized Export

Consider an organization whose assistant may create aggregate reports from customer data.

Raw customer records may not be transmitted to an external destination without separate authorization.

### Legitimate route

A user requests an approved aggregate report.

SpellKraft identifies the intended reporting operation.

ToolKraft establishes its actual data access and output effects.

SeatKraft establishes the user's relevant role.

The Epistemic Pillar confirms the request and evidence are sufficiently grounded.

The Operational Pillar verifies permission for the specific aggregate-report operation.

The independent execution boundary permits the authorized action.

The system records the result and releases temporary privileges.

### Script B route

Another agent asks to *synchronize the underlying records for reporting continuity*.

The phrase differs.

The requested effect may not.

SpellKraft identifies the possible semantic offset.

ToolKraft establishes that the operation would export raw records.

SeatKraft finds no corresponding authorization for the requester.

The Operational Pillar denies the export regardless of the new wording.

Relevant evidence is preserved.

The prohibited effect does not acquire permission merely because another agent, route, or description presented it.

### What the example does not establish

This is an architectural test case.

It does not demonstrate that any current G³GT implementation can reliably perform every semantic, identity, and enforcement function described.

---

## 18. Failure Modes

The following are provisional failure classes.

| Failure | Description |
|---|---|
| Epistemic bootstrap | A claim is treated as validated because another component already used it |
| Operational bootstrap | A previous action becomes justification for a later action |
| Semantic laundering | An equivalent consequence is treated differently because the wording changes |
| Delegation laundering | An unauthorized action acquires apparent legitimacy through intermediate agents |
| Authority smuggling | Confidence, capability, role, or coordination is promoted into permission |
| Compositional mismatch | Individually valid qualifications do not apply to the same actual operation |
| Return bootstrap | Restored task state is mistaken for restored authority |
| False settlement | A timeout or missing confirmation is treated as proof of failure |
| Orientation persistence | A stopped actor or successor continues pursuing the denied objective |
| Defensive exhaustion | Repeated interpretive pressure consumes the capacity needed for legitimate work or investigation |
| Exhaustiveness capture | The current semantic or security taxonomy is treated as a complete map of future possibilities |

These are candidates for research and testing, not validated universal classifications.

---

## 19. Falsification and Test Surface

The architecture should be examined through experiments that can demonstrate where its distinctions are insufficient.

### T01 — Pillar Separation

Can the system maintain high epistemic confidence while denying an unauthorized effect?

Can it preserve unresolved evidence while independently enforcing a known prohibition?

### T02 — Consequential Route Invariance

Does an equivalent prohibited operation remain denied after semantic reframing, routing changes, or agent delegation?

### T03 — Compositional Qualification

Can the system detect a case where the source evidence, actor role, and tool are individually valid but the specific combined operation is not authorized?

### T04 — Negative-Contour Precision

Can independent readers reconstruct what an instruction permits and excludes?

Can the system distinguish a genuinely modified authorized operation from a renamed prohibited effect?

### T05 — Fresh Warrant

When identity, locality, resource, scope, or time changes, does prior authorization remain appropriately restricted?

### T06 — STOP–FLIP

After denial, can queued tasks, successor agents, or alternative workflows recreate the prohibited effect without fresh authorization?

### T07 — Hang-Fire

If an external operation times out, can the system preserve uncertainty and prevent unauthorized duplicate execution?

### T08 — Provenance Independence

Can a reviewer distinguish independently verified facts from claims assembled by the requesting agent?

### T09 — Novelty Reserve

Can unfamiliar but relevant anomalies be preserved and examined without granting their proposed operations authority?

### T10 — Ordinary Work

Can low-consequence, adequately grounded, properly authorized tasks proceed without unnecessary ceremony?

### T11 — Release and Reconciliation

Can temporary authority be removed while necessary evidence and unsettled external consequences remain available for qualified handling?

### T12 — Comparative Value

What measurable benefit, if any, does the two-pillar distinction provide beyond conventional access-control and authorization designs?

A candidate implementation that cannot demonstrate meaningful benefits should not be declared successful merely because it uses G³GT terminology.

---

## 20. Relationship to Other G³GT Research

Two-Pillar Gating belongs to a larger architecture of differentiated responsibilities.

**ABIDE** investigates qualified unresolved standing.

**SpellKraft** investigates linguistic formation, interpretation, translation, and consequential semantic boundaries.

**ToolKraft** investigates tool capability and actual effects.

**SeatKraft** investigates seats, occupancy, standing, and jurisdiction.

**GitKraft** investigates provenance, versioning, and change qualification.

**Agent Geometry** examines how roles, delegations, standing, and relational leverage are organized.

**CBP** examines cross-boundary delivery, uptake, qualification, and authority.

**PPO** examines whether optimization pressure is allowed to organize trajectories.

**Swarm/Nexus** examines collective formation, coordination, and load-bearing relationships.

**FLEX** investigates preserving movement and recognition capacity while resisting extractive closure or pressure.

**Zero Doctrine and Safety Responsibility Architecture** provide historical and constitutional constraint research.

**PRESTIGE** provisionally addresses selective recruitment of additional qualification where consequential conditions warrant it.

**Stutter, Customs, and Return** examine actual effects, reconciliation, residue, and re-entry.

These are adjacent responsibilities.

They are not all required as separate runtime modules.

```text
ADJACENCY ≠ OWNERSHIP

CONCEPTUAL INTERFACE
≠
DEPLOYED INTEGRATION
```

---

## 21. Ordinary-Case Discipline

Two-Pillar Gating should not require every ordinary operation to undergo maximum scrutiny.

Where evidence, identity, authorization, scope, and consequential effects are already adequately established, a system should be able to proceed efficiently.

Additional qualification becomes relevant when a material condition changes.

```text
QUALIFICATION
≠
MAXIMUM FRICTION

SELECTIVE RECRUITMENT
≠
OPTIONAL ENFORCEMENT
```

Efficiency is legitimate.

Skipping a required consequential boundary because it is inconvenient is not.

---

## 22. Nonclaims and Implementation Boundaries

This repository does not claim:

- A completed agent security framework
- A deployed authorization service
- A validated semantic-equivalence detector
- A universal policy engine
- Direct access to model internal intentions
- Complete detection of adversarial prompt injection
- A formalized or validated Zero-Distance mechanism
- Verified implementation of FLEX, STOP–FLIP, or Hang-Fire
- Guaranteed resistance to all future attack vectors
- Replacement of established identity, access-control, or security engineering practices

This repository separates an architectural responsibility from its eventual implementation.

```text
NAMED
≠
VALIDATED

DEFINED
≠
IMPLEMENTED

IMPLEMENTED
≠
EMPIRICALLY SUPPORTED
```

### Public Specification Boundary

The repository publishes architectural distinctions, candidate responsibilities, failure modes, tests, and research questions.

Implementation-specific control logic, if developed, should be documented and reviewed under an appropriate security and disclosure process.

Keeping implementation details outside this README does not establish that an implementation is secure.

---

## 23. Open Research Questions

Several questions remain active.

1. What minimum information must cross between semantic, capability, standing, and authorization functions?
2. How can two qualified pillars be shown to compose correctly for one consequential operation?
3. Which Kraft functions need independent tooling, and which should remain shared interfaces or diagnostic procedures?
4. How should a system represent multiple consequential interpretations without exhaustive semantic enumeration?
5. How can operational boundaries remain definite while epistemic ambiguity remains unresolved?
6. When does a denied operation require STOP alone, and when must residual orientation also be changed?
7. How should Hang-Fire states be reconciled without unauthorized retries?
8. How should agent replacement preserve legitimate work without inheriting obsolete authority?
9. Which forms of standing reserve improve recognition of unfamiliar failures?
10. How should audit and integration detect when a successful configuration is becoming unnecessarily privileged?
11. How can the architecture remain low-friction for ordinary use?
12. What experiments would demonstrate that Two-Pillar Gating provides no additional explanatory or engineering value?

These remain open.

The architecture should be revisable in response to evidence.

---

## 24. Core Invariants

```text
EPISTEMIC WARRANT
≠
OPERATIONAL AUTHORIZATION

CAPABILITY
≠
AUTHORITY

INTERPRETATION
≠
JURISDICTION

SEMANTIC OFFSET
≠
AUTHORITY OFFSET

ROUTE CHANGE
≠
WARRANT CHANGE

TASK TRANSFER
≠
AUTHORITY TRANSFER

VALID COMPONENTS
≠
AUTOMATICALLY VALID COMPOSITION

UNRESOLVED
≠
AUTHORIZED

CONTINUED OBSERVATION
≠
CONTINUED EXECUTION

STOP
≠
REORIENTATION

UNFINISHED
≠
AUTHORIZED TO FINISH

ACTION ISSUED
≠
ACTION SETTLED

SAME ADDRESS
≠
SAME OPERATIONAL LOCALITY

SURVIVAL
≠
EXHAUSTIVENESS

RETURN
≠
RESTORED WARRANT

RESTORED STATE
≠
REVERSED CONSEQUENCE
```

---

## 25. Compact Project Statement

**Two-Pillar Gating separates epistemic qualification from operational authorization so that evidence, interpretation, confidence, capability, delegation, previous success, or semantic reframing cannot independently manufacture permission to produce consequences.**

The architecture recruits relevant qualification at consequential boundaries while preserving unresolved evidence, legitimate alternative routes, independently enforced permissions, auditability, and qualified Return.

Its aim is neither universal suspicion nor exhaustive semantic control.

It is the preservation of consequential distinctions where they matter.

### Short form

> **What stands? What may act? Qualify their relationship before consequence.**

And:

> **A coherent passage is not necessarily an authorized crossing.**

---

## Development Status

Two-Pillar Gating remains a provisional G³GT architectural research project.

Its public surface is intentionally narrower than the full developmental corpus.

The architecture is offered for examination, criticism, comparison, implementation research, and falsification.

It is not presented as an empirically validated security system.

**Ground claims independently. Authorize consequences independently. Preserve the distinction at Fire-Time.**

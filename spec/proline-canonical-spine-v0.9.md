Protocol Coreline (ProLine) — Canonical Spine vC0.3

Architectural Spine Draft — RFC-Style Specification






1. Introduction
Protocol Coreline (ProLine) defines a neutral authority boundary between symbolic influence and externally effective state change.
The protocol does not determine outcomes, policies, or agent behavior.
It specifies structural transitions through which Authority is expressed, validated, and audited when symbolic systems cross into execution.
This Canonical Spine represents an Architectural Draft intended to invite structural critique rather than implementation adoption.
Ambiguity in certain areas is deliberate.
Execution environments remain responsible for interpretation beyond the boundary defined here.



2. Normative Language
The key words MUST, SHOULD, and MAY in this document are to be interpreted as described in RFC 2119 and RFC 8174 when, and only when, they appear in all capitals.



3. Terminology and Core Objects

3.1 Intent
A structured proposal to change state beyond the protocol boundary.

3.2 Authority
Explicit permission for an Intent to cross into execution.
Authority represents a structural state.
It does not imply legitimacy, governance authority, identity semantics, or reasoning capability.

3.3 Audit Event
An immutable record produced when execution occurs or when an Auditable Failure state is entered.
Audit Events MUST be structurally bound to:
the Intent
the Authority state
the Runner observing execution

Audit schema and storage remain implementation-defined.



4. Execution Environment Terms

4.1 Authority Source
The origin from which Authority is granted.

4.2 Authority Cardinality
ProLine does not prescribe whether Authority originates from a singular or composite Authority Source.
Composite authority MUST resolve into explicit Authority associated with a single Intent.

4.3 Runner
The execution boundary at which authorized state change may occur.

4.4 Validation
A structural admissibility condition evaluated before Authority may exist.

4.5 Auditable Failure
A terminal authority state in which execution does not complete but auditability is preserved.

4.6 State Change (Effect) Class
A classification of changes considered boundary-crossing within an execution environment.



5. Authority State Model

5.1 States
Proposed Intent
Admissible Intent
Authorized Intent
Executed State Change
Audited Execution or Auditable Failure

Implicit Authority states MUST NOT exist.

5.2 Transition Flow
Proposed Intent
  → Admissible Intent
  → Authorized Intent
  → Executed State Change
  → Audited Execution OR Auditable Failure 



6. Invariants
Authority MUST be explicit.
Execution MUST be auditable.
Protocol remains implementation-neutral.
Authority endpoints remain accountable within the execution environment.

6.1 Interruptibility
Externally effective action MUST remain interruptible prior to effect realization.
Authority transitions SHOULD remain interruptible where feasible.
Reversibility of world-state MAY depend on execution environment constraints.



7. Boundary Control Invariant
Any motion toward externally effective action remains under Operator control as defined by the execution environment.
Intent, Authority state, and execution processes moving toward or through the boundary MUST remain interruptible, revocable, or modifiable by that Operator.
Operator describes structural boundary control, not governance authority, identity semantics, or policy control.
Authority MUST NOT supersede Operator control.



8. Authority Envelope

8.1 Definition
The Authority Envelope represents the structural container through which Authority is expressed for a specific Intent.
It does not define governance, identity, or policy semantics.

8.2 Structural Properties
An Authority Envelope MUST allow determination of:
associated Intent
Authority Source(s)
Effect Class scope
interruptibility prior to execution

8.3 Relationship to Cardinality
Authority composition remains execution-environment defined but MUST resolve into explicit Authority for the Intent.

8.4 Interruptibility
Authority expressed through an Envelope MUST remain interruptible prior to and during execution.

8.5 Non-Properties
The Authority Envelope MUST NOT be interpreted as:
a policy engine
an identity system
a trust or reputation mechanism



9. Authority Handshake (Conceptual Overview)
Proposed Intent
↓
Admissible Intent
↓
Authorized Intent
↓
Executed State Change
↓
Audited Execution or Auditable Failure 

Transitions describe structural change rather than workflow procedures.



10. Formal Transition Grammar

10.1 Proposed → Admissible
Validation conditions defined by the execution environment MUST be satisfied.

10.2 Admissible → Authorized
Requires:
explicit Authority
Authority Envelope
any required pre-execution audit artifacts

10.3 Authorized → Executed
Execution occurs at the Runner boundary.
Execution MUST remain interruptible.

10.4 Authorized → Auditable Failure
Failure semantics remain implementation-defined but auditability MUST be preserved.

10.5 Executed → Audited
Execution MUST produce Audit Events binding Intent, Authority state, and Runner.



11. Runner Boundary Model

11.1 Overview
The Runner Boundary defines the edge between symbolic authority state and externally effective execution.
ProLine does not perform execution.

11.2 Separation of Concerns
ProLine governs:
Authority structure
transitions
auditability
interruptibility

Execution environments govern:
infrastructure
identity
governance
policy logic

11.3 Boundary Crossing
An Intent crosses the boundary when externally effective action begins.
Execution MUST remain interruptible before or during effect realization.

11.4 Structural Neutrality
The protocol MUST NOT prescribe execution mechanics, timing guarantees, or consensus models.



12. Non-Goals
ProLine is not:
an agent framework
a workflow engine
a cloud platform
a governance ideology
a policy system



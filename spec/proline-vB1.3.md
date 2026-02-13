# Protocol Coreline (ProLine) — Draft vB1.3    

## 1. Purpose  

Protocol Coreline (ProLine) defines a neutral authority boundary
between symbolic influence and externally effective state change.

The protocol does not determine outcomes or policies.
It specifies the structure through which authority is expressed,
validated, and audited.

Boundary crossing depends on explicit authority rather than implicit
trust, reputation, or emergent social signals. 

---

## 2. Core Concepts (Protocol Primitives) 

Intent 
A structured proposal to change state beyond the protocol boundary.

Authority
Explicit permission for an Intent to cross into execution.

Audit Event
An immutable record produced when execution occurs.   


## 2.1 Authority Cardinality

ProLine does not prescribe whether Authority originates from a
singular or composite Authority Source.
Authority composition, delegation, and aggregation are defined
by the execution environment.  
   
---   
   
## 3. Execution Environment Terms

Authority Source
The origin from which Authority is granted.

Runner
The execution boundary at which authorized state change may occur.

Validation
A structural admissibility condition evaluated before Authority may exist.

Auditable Failure
A terminal authority state in which execution does not complete but
auditability is preserved.

State Change (Effect) Class
A classification of changes considered boundary-crossing within a
given execution environment.
 
---

## 4. Authority Handshake  

Proposed Intent
↓ (validation condition satisfied)
Admissible Intent
↓ (Authority granted by Authority Source AND required Pre-Execution
   Audit Events produced)  
Authorized Intent 
↓ (state change occurs at Runner boundary)  
Executed State Change    
↓ (Post-Execution Audit Events produced OR Auditable Failure State  
   entered)
Audited Execution

The protocol defines transitions between authority states rather than 
procedural steps.  
   
---

## 5. Invariants

- Authority must be explicit.
- Execution must be auditable.
- Actions must remain interruptible.
- Protocol remains implementation-neutral.
- Authority endpoints remain accountable within the execution environment. 
-Authority transitions must remain interruptible; reversibility of world-state 
is implementation-and domain-dependent.


---

## 6. Non-Goals

ProLine is not:

- an agent framework
- a cloud platform
- a workflow engine
- a policy engine

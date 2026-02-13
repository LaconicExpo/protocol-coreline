# Protocol Coreline (ProLine) — Draft vA1.3   

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
   
---   
   
## 3. Execution Environment Terms 
   
Authority Source 
The origin from which Authority is granted. 

Runner
The execution boundary at which authorized state change may occur.

Validation 
A structural admissibility evaluation that must be satisfied before 
Authority may be granted.   

Auditable Failure   
A terminal authority state in which execution does not complete but auditability 
is preserved  
   
State Change (Effect) Class 
A classification of changes that are considered boundary-crossing in a given 
environment 
   
---   

## 4. Authority Handshake  

Proposed Intent
↓ (validation condition satisfied)
Admissible Intent
↓ (Authority granted AND required Pre-Execution Audit Events present)  
Authorized Intent 
↓ (state change occurs at Runner boundary)  
Executed State Change    
↓ (Post-Execution Audit Events produced OR Auditable Failure State entered)
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
is implementation - and domain-dependent.
-Authority Model (vA1.3 Scope) 
ProLine v1.2 models Authority as originating from a single Authority Source per Intent.    
Composed or multi-source authority models may be implemented but are not defined by this 
version.   

---

## 6. Non-Goals

ProLine is not:

- an agent framework
- a cloud platform
- a workflow engine
- a policy engine

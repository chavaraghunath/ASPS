# Reference Architecture

The ASPS reference architecture is **vendor-neutral**. It can be implemented through any combination of cloud platforms, AI model providers, CI/CD stacks, repositories, observability platforms, GRC systems, and evidence stores.

> The architecture is defined by **control responsibilities, not by specific products.** Swap any vendor; the responsibilities remain.

---

## The layers

| Layer | Core Capability |
|-------|-----------------|
| **Experience Layer** | Conversational intake, intent negotiation, risk clarification, executive and engineering views |
| **Intent Layer** | Intent Contracts, assumptions, exclusions, risk classification, success-telemetry definition |
| **Governance Layer** | Policy-as-code, agent trust classes, compliance controls, legal triggers, approval thresholds |
| **Context Layer** | Production Knowledge Graph, context lifecycle, source trust, memory partitions, retrieval policies |
| **Orchestration Layer** | Cell routing, task decomposition, sub-agent spawning, escalation |

---

## Layer responsibilities in depth

### 🗣️ Experience Layer
The human interface to autonomous production. Where intent is **captured and negotiated**, risk is clarified in conversation, and both executives and engineers get role-appropriate views. This is where ambiguity is resolved *before* it becomes autonomous action.

### 📜 Intent Layer
Turns negotiated intent into a **machine-actionable, bounded contract**: what's wanted, what's excluded, what assumptions hold, the risk class, and how success will be measured in telemetry. The Intent Contract becomes the reference against which everything downstream is judged.

### 🏛️ Governance Layer
The control plane. **Policy-as-code** decides what agents may do; **agent trust classes** bound their authority; **compliance controls** and **legal triggers** fire when thresholds are crossed; **approval thresholds** route high-consequence actions to humans. This layer is where ASPS's governance becomes executable.

### 🧠 Context Layer
The memory and knowledge substrate. The **Production Knowledge Graph** holds trusted production reality; **context lifecycle** and **source trust** keep it fresh and attributed; **memory partitions** and **retrieval policies** prevent context poisoning and leakage. Agents are only as trustworthy as the context they act on.

### 🎛️ Orchestration Layer
The execution fabric. Routes work to **production cells**, decomposes tasks, spawns **sub-agents**, and **escalates** when confidence or authority is exceeded. This is where autonomous work is actually coordinated and run — under the constraints set by the layers above.

---

## Mapping layers to the domains

The five layers **host** the [eleven governance domains](eleven-governance-domains.md):

| Layer | Primary domains it carries |
|-------|----------------------------|
| Experience | Intent Governance *(intake side)* |
| Intent | Intent Governance |
| Governance | Cyber Security · Compliance · Legal · Reversibility · Economics |
| Context | Context Integrity · Evidence Ledger |
| Orchestration | Agent Engineering · Verification Factory · Runtime Truth |

The **layers** are *where things run*; the **domains** are *what must be governed*. ASPS specifies both so an enterprise can implement it on any technology stack without losing the control guarantees.

---

## Standards alignment

ASPS is designed to **align with**, not replace, existing enterprise frameworks:

| Standard / Framework | Relevance to ASPS |
|----------------------|-------------------|
| **NIST SSDF** | Secure software development direction for Cyber Production Security |
| **COBIT / ITIL** | Enterprise governance and service-management alignment for operating-model integration |

This lets ASPS slot into an organization's existing governance estate rather than demanding a greenfield.

---

**Next:** **[Differentiation from Existing Paradigms](differentiation.md)** → why ASPS is not just "DevOps for AI."

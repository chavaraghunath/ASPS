# Adoption Roadmap

ASPS is adopted **incrementally**, climbing the **[Maturity Model](maturity-model.md)** one level at a time. You do not need the whole framework on day one — you need the *next* control that closes your most dangerous gap.

> Principle: **adopt governance just ahead of autonomy.** Never let agent authority outrun the controls that bound it.

---

## Phase 0 → 1 — Establish the baseline

**Goal:** know how production changes are proven today.

- Inventory where AI/agents already touch your pipeline (often more than you think)
- Establish telemetry linkage between *change* and *outcome*
- Name an accountable owner for autonomous-production risk

**Exit criterion:** you can answer *"do we know how production changes are proven?"*

---

## Phase 1 → 2 — Govern the agents

**Goal:** move from ungoverned productivity to **governed agent workflows**.

- Stand up **Agent Engineering**: an agent registry, skill catalog, and **tool-trust registry**
- Assign **agent trust classes** and scope tool access (least privilege)
- Enforce branch isolation and require evidence outputs from agent runs

**Exit criterion:** you can answer *"which agents can affect production?"*

→ Activates: Agent Engineering, parts of the Governance Layer.

---

## Phase 2 → 3 — Make promotion evidence-led

**Goal:** promotion depends on **signed evidence**, not assertion.

- Stand up the **Evidence Ledger** (why a change exists, who produced it, what verified it)
- Build the **Verification Factory** with risk-weighted gates
- Introduce **Intent Contracts** so every change has a bounded, testable origin

**Exit criterion:** you can answer *"can we audit why a change was promoted?"*

→ Activates: Intent Governance, Verification Factory, Evidence Ledger.

---

## Phase 3 → 4 — Close the loop with runtime truth

**Goal:** production **validates** the claims made about it.

- Instrument **Runtime Truth**: telemetry that proves or disproves delivery claims
- Feed runtime signals back into policies and controls
- Strengthen **Context Integrity** (Production Knowledge Graph, source trust)

**Exit criterion:** you can answer *"does production prove or disprove delivery claims?"*

→ Activates: Runtime Truth, Context Integrity.

---

## Phase 4 → 5 — Integrate the full control plane

**Goal:** **trustworthy, reversible autonomous production** at scale.

- Integrate **Cyber Production Security**, **Autonomous Compliance**, **Legal Governance**
- Make **Production Economics** ([CTQOST-R](ctqost-r.md)) visible and optimizable
- Enforce **[Reversibility by Design](reversibility-by-design.md)** as a hard promotion gate across all changes

**Exit criterion:** you can answer *"can the enterprise safely scale autonomous production?"*

→ Activates: the remaining [governance domains](eleven-governance-domains.md).

---

## Sequencing principles

1. **Reversibility early.** Even before full maturity, require a defined recovery path for any autonomous action — it is the cheapest insurance you will buy.
2. **Risk-weight everything.** Don't gate low-risk changes heavily; concentrate controls where blast radius justifies them.
3. **Evidence before scale.** Do not widen agent authority until promotion is evidence-led (Level 3). Scaling ungoverned autonomy is the **[AI code factory](anti-patterns.md)** trap.
4. **Vendor-neutral.** Implement each control as a *responsibility* (see **[Reference Architecture](reference-architecture.md)**), so you can change tools without losing guarantees.

---

## A note on pace

ASPS maturity is **not** a race to Level 5. It is about ensuring **governance stays one step ahead of autonomy** at every phase. An organization at Level 3 with disciplined evidence is far safer than one at Level 1 scaling agents blindly.

---

**Next:** **[Anti-Patterns](anti-patterns.md)** → the failure modes to avoid on the way up.

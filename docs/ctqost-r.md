# CTQOST-R Optimization Model

CTQOST-R is the **objective function of ASPS** — the model that defines what "good" means when autonomous agents produce software. It extends classic delivery thinking (Cost, Time, Quality) with the constraints that autonomous production makes non-negotiable.

> ASPS does not optimize speed alone. It optimizes **production-correct outcomes** under economic, operational, security, trust, and reversal constraints.

---

## The seven dimensions

| | Dimension | What it governs |
|---|-----------|-----------------|
| **C** | **Cost** | Total economic cost of producing and operating the change |
| **T** | **Time** | Velocity to a *production-proven* outcome (not just merged code) |
| **Q** | **Quality** | Correctness, architectural integrity, defect resistance |
| **O** | **Operability** | Observability, SLOs, incident readiness, scaling behavior |
| **S** | **Security** | Cyber resilience across the autonomous attack surface |
| **T** | **Trust** | Evidence, accountability, and governance assurance |
| **R** | **Reversibility** | The ability to undo, compensate, contain, or safely degrade |

The first three (**C, T, Q**) are familiar from traditional delivery. The last four (**O, S, T, R**) are the dimensions that autonomy makes mandatory — the ones existing paradigms under-serve.

---

## Why the extra dimensions matter

When a **human** ships a change, organizational judgment implicitly covers operability, security, trust, and reversibility. When an **autonomous agent** ships at machine speed and scale, those implicit checks vanish. CTQOST-R makes them **explicit, weighted, and optimizable**.

| Without it | With CTQOST-R |
|------------|---------------|
| "Ship faster" | "Ship *production-correct* outcomes per unit cost and time" |
| Reversibility is luck | Reversibility is a scored dimension |
| Security is a later gate | Security is part of the objective |
| Trust is assumed | Trust is measured and evidenced |

---

## CTQOST-R as a constraint system

CTQOST-R is best read as **correctness under constraint**:

```
maximize   Production Correctness (Q)
per unit   Cost (C) × Time (T)
subject to Operability (O), Security (S), Trust (T), Reversibility (R)
           meeting their required thresholds for the change's risk class
```

A change that is fast and cheap but **irreversible**, **insecure**, or **unevidenced** does not score well in ASPS — it fails the constraints regardless of velocity.

---

## Risk-weighting (the practical core)

CTQOST-R is **not applied uniformly**. ASPS insists verification and control be **risk-weighted**:

> Low-risk changes should not be smothered by unnecessary controls. High-risk changes must not pass through light gates.

The model optimizes verification and control **cost against blast radius**, data sensitivity, security exposure, regulatory exposure, and **reversibility class**. This keeps ASPS economical — heavy governance is spent only where consequence justifies it.

→ See the **Verification Factory** in **[The Eleven Governance Domains](eleven-governance-domains.md)** and **[Reversibility by Design](reversibility-by-design.md)** (reversibility classes).

---

## How CTQOST-R connects to the rest of ASPS

- **[Reversibility by Design](reversibility-by-design.md)** operationalizes the **R** dimension.
- **Production Economics** (a governance domain) instruments **C** and **T**.
- The **Verification Factory** and **Runtime Truth** measure **Q** and **O**.
- **Cyber Production Security** and the **Evidence Ledger** underwrite **S** and **T**.

CTQOST-R is the lens; **[The Eleven Governance Domains](eleven-governance-domains.md)** are the machinery that satisfies it.

---

**Next:** **[Reversibility by Design](reversibility-by-design.md)** → the invariant behind the *R* dimension.

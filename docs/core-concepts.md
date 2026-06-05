# Core Concepts

ASPS rests on a small set of foundational ideas. Understand these five, and the rest of the framework follows naturally.

---

## 1. Production correctness, not code output

Traditional delivery optimizes for **velocity** — how fast can we ship code? ASPS rejects this as the goal.

> **The objective is not more code. The objective is *production correctness per unit cost and time*, under explicit constraints of security, trust, legal, compliance, operability, and reversibility.**

Autonomous agents can generate unlimited code. Volume is no longer scarce — **trustworthy, correct, reversible production** is. ASPS reorients the entire production system around that scarce resource.

→ Formalized in the **[CTQOST-R Optimization Model](ctqost-r.md)**.

---

## 2. Governed transformation of intent

ASPS reframes software production as a pipeline that **transforms human intent into governed system behavior**:

```
Human Intent  →  Intent Contract  →  Governed Production  →  Production-Proven Behavior
                      (negotiated,         (policy, agents,        (verified by runtime
                       risk-classified)     evidence, controls)     truth, reversible)
```

Intent is never executed blindly. It is **negotiated, bounded, risk-classified, and contracted** before any autonomous action occurs.

→ See **[Reference Architecture](reference-architecture.md)** (Intent Layer) and the *Intent Contracts* section of the thesis.

---

## 3. Production trust as the unifying objective

Every part of ASPS exists to produce one thing: **production trust** — justified confidence that what autonomy put into production is correct, accountable, secure, compliant, and reversible.

Trust is not a feeling; in ASPS it is an **engineered, evidenced property**. It is assembled from eleven interdependent domains, and a single weak domain lowers the trustworthiness of the whole system.

→ See **[The Eleven Governance Domains](eleven-governance-domains.md)**.

---

## 4. Reversibility as a first-class invariant

Most paradigms treat rollback as an operational afterthought. ASPS elevates it to a **non-negotiable production invariant**:

> **No autonomous action is promotable to production unless its reversal, compensation, containment, or safe-degradation path is defined in advance.**

If you cannot describe how to undo it, you cannot ship it.

→ Detailed in **[Reversibility by Design](reversibility-by-design.md)**.

---

## 5. Evidence over assertion

In ASPS, claims are not trusted — **evidence is**. A change is promoted not because someone says it works, but because **signed evidence** proves *why it exists, who produced it, what governed it, what verified it, what risks were accepted, and how it can be reversed*.

This evidence is durable and auditable, recorded in the **Evidence Ledger**, and continuously validated against **Runtime Truth** — the telemetry that proves or disproves delivery claims after release.

→ See **[The Eleven Governance Domains](eleven-governance-domains.md)** (Evidence Ledger, Runtime Truth).

---

## How the concepts connect

| Concept | Answers the question |
|---------|----------------------|
| Production correctness | *What are we optimizing for?* |
| Governed transformation of intent | *How does work enter the system?* |
| Production trust | *What is the end goal?* |
| Reversibility-by-design | *What must be true before we ship?* |
| Evidence over assertion | *How do we know it's real?* |

Together they define a production system fit for **autonomous actors operating at enterprise scale and consequence**.

---

**Next:** **[CTQOST-R Optimization Model](ctqost-r.md)** → how ASPS turns these principles into a measurable objective function.

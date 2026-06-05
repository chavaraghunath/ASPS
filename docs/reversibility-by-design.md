# Reversibility by Design

Reversibility-by-Design is the **defining safety principle of ASPS** — the one idea that most distinguishes it from every prior delivery paradigm. It elevates "can we roll this back?" from an operational afterthought to a **production invariant** that gates promotion.

---

## The invariant

> **No autonomous action is promotable to production unless its reversal, compensation, containment, or safe-degradation path is defined in advance.**

Read literally: **if you cannot describe how to undo it, you cannot ship it.** This applies to every autonomous change, at every scale.

---

## Why autonomy demands it

A human operator carries implicit judgment about consequence and recovery. An **autonomous agent** acting at machine speed does not — and the blast radius of an un-reversible automated action can be enormous and immediate. Reversibility-by-Design forces the recovery path to be **designed up front**, not discovered during an incident.

---

## The four reversal modes

ASPS recognizes that not everything can be perfectly "undone." It defines **four acceptable recovery paths** — at least one must exist before promotion:

| Mode | Meaning | Example |
|------|---------|---------|
| **Reversal** | Cleanly undo the change, restoring prior state | Roll back a deployment; revert a migration |
| **Compensation** | Apply a counter-action that offsets the effect | Issue a corrective transaction; refund |
| **Containment** | Limit the blast radius so damage cannot spread | Circuit-break; quarantine; feature-flag off |
| **Safe degradation** | Fall back to a reduced but safe mode of operation | Serve cached/read-only; graceful downgrade |

A change with **none** of these defined is, by ASPS definition, **not promotable**.

---

## Reversibility class

Every change carries a **reversibility class** — how recoverable it is — which feeds directly into [CTQOST-R](ctqost-r.md) risk-weighting:

- **Highly reversible** → lighter gates, faster promotion
- **Hard to reverse / irreversible** → heavier verification, stronger approval, more evidence

This makes reversibility an **economic lever**, not just a safety one: the easier something is to undo, the cheaper it is to ship safely.

---

## How reversibility is verified

Reversibility is not asserted — it is **tested**, as part of the Verification Factory's *reversibility verification*:

- **Rollback simulation** — prove the reversal actually works before you need it
- **Compensation testing** — validate counter-actions produce the intended offset
- **Snapshot validation** — confirm restorable state exists and is consistent
- **Forensic replay** — reconstruct what happened for audit and recovery
- **Safe-degradation checks** — verify the system fails into a safe mode

→ See **Verification Factory** and **Evidence Ledger** in **[The Eleven Governance Domains](eleven-governance-domains.md)**.

---

## Reversibility as a domain *and* a dimension

Reversibility appears twice in ASPS — deliberately:

1. As the **R** in **[CTQOST-R](ctqost-r.md)** (a scored optimization dimension)
2. As a **governance domain** producing the *release decision, rollback contract, and approval trail*

This dual role signals its importance: it is both *something you measure* and *something you govern*.

---

## The cultural shift

| Traditional thinking | Reversibility-by-Design |
|----------------------|-------------------------|
| "We'll figure out rollback if needed" | Rollback path defined **before** promotion |
| Reversibility = ops concern | Reversibility = production invariant |
| Optimize for forward speed | Optimize for **recoverable** forward speed |
| Incident → scramble | Incident → execute the pre-defined path |

---

**Next:** **[The Eleven Governance Domains](eleven-governance-domains.md)** → the full machinery that produces production trust.

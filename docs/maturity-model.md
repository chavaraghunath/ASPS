# Maturity Model

The ASPS Maturity Model is a **six-level self-assessment ladder** for organizations adopting autonomous software production. Each level is paired with **the question a board should be able to answer** at that stage — making maturity a governance conversation, not just a technical one.

---

## The six levels

| Level | Name | Description | The Board Question |
|:---:|------|-------------|--------------------|
| **0** | Manual / fragmented delivery | Human-driven SDLC, weak telemetry linkage, disconnected evidence | *Do we know how production changes are proven?* |
| **1** | AI-assisted engineering | Copilots and AI tools improve local productivity, but governance remains manual | *Are we creating faster, unmanaged risk?* |
| **2** | Governed agent workflows | Agents have policies, scoped tools, branch isolation, and evidence outputs | *Which agents can affect production?* |
| **3** | Evidence-led production | Promotion depends on signed evidence, verification, compliance, security, and rollback readiness | *Can we audit why a change was promoted?* |
| **4** | Runtime-truth adaptive production | Runtime telemetry validates intent and feeds learning back into controls | *Does production prove or disprove delivery claims?* |
| **5** | Trustworthy reversible autonomous production | Cyber, compliance, legal, economic, and reversibility controls are integrated into autonomous production | *Can the enterprise safely scale autonomous production?* |

---

## Reading the ladder

The levels trace a deliberate progression:

```
0  Fragmented        →  no linkage between change and proof
1  AI-assisted       →  speed up, governance unchanged  (the danger zone)
2  Governed agents   →  autonomy gains policies + scope
3  Evidence-led      →  promotion requires signed evidence
4  Runtime-truth     →  production validates the claims
5  Trustworthy       →  full reversible, governed autonomy at scale
```

### ⚠️ The Level 1 trap
Most organizations adopting AI coding tools jump to **Level 1** — productivity rises, but governance stays manual. The board question makes the risk explicit: *are we creating faster, unmanaged risk?* ASPS exists to move organizations **past** Level 1 deliberately, rather than accumulating autonomous risk by default.

### The Level 3 inflection
**Evidence-led production** is the pivotal step: promotion stops depending on assertion and starts depending on **signed evidence** (verification, compliance, security, rollback readiness). This is where [the Evidence Ledger](eleven-governance-domains.md) becomes load-bearing.

### The Level 5 goal
**Trustworthy reversible autonomous production** integrates every control domain — cyber, compliance, legal, economic, and [reversibility](reversibility-by-design.md) — so the enterprise can scale autonomy *safely*. This is the target state ASPS is designed to reach.

---

## How to use it

1. **Locate yourself.** Answer each board question honestly. Your level is the **highest** one where you can answer affirmatively *with evidence*.
2. **Find the gap.** The next level's board question is your near-term objective.
3. **Map to domains.** Each climb activates specific [governance domains](eleven-governance-domains.md) — e.g., reaching Level 3 means standing up the Evidence Ledger and Verification Factory.
4. **Sequence the work.** Use the **[Adoption Roadmap](adoption-roadmap.md)** to plan the climb.

> Maturity is not measured by how much AI you use (Level 1) — it is measured by how *provably, reversibly, and accountably* autonomy operates in production (Levels 3–5).

---

**Next:** **[Adoption Roadmap](adoption-roadmap.md)** → how to climb the ladder in practice.

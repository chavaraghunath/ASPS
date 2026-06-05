# Anti-Patterns

ASPS is defined as much by what it **prohibits** as by what it prescribes. These are the failure modes that autonomous production invites — each one trades short-term velocity for unmanaged, autonomous-scale risk.

> If you recognize your organization in several of these, you are likely stalled at **[Level 1](maturity-model.md)** — fast, but ungoverned.

---

## 🏭 1. The AI code factory without verification

**The pattern:** maximize agent output — lines, PRs, features — while verification, architecture review, and evidence lag behind.

**Why it fails:** it hides defects and architecture drift behind a wall of volume. Output looks like progress; correctness quietly erodes. This is the **canonical ASPS anti-pattern** — speed mistaken for production.

**The ASPS counter:** [CTQOST-R](ctqost-r.md) optimizes *production correctness*, not output; the Verification Factory gates promotion.

---

## ↩️ 2. Autonomous action without a reversal path

**The pattern:** agents ship changes with no defined way to undo, compensate, contain, or safely degrade.

**Why it fails:** the first serious incident has no pre-designed recovery — you improvise during the outage, at machine-scale blast radius.

**The ASPS counter:** **[Reversibility by Design](reversibility-by-design.md)** — no promotion without a defined recovery path.

---

## 🔓 3. Unscoped tool access

**The pattern:** agents are granted broad tool and system access "to be productive," without least-privilege scoping or trust classes.

**Why it fails:** every over-privileged agent is an expanded attack surface and an expanded blast radius. Prompt injection or context poisoning becomes catastrophic rather than contained.

**The ASPS counter:** Agent Engineering's **tool-trust registry** and **agent trust classes**; Cyber Production Security.

---

## 🧪 4. Promotion without signed evidence

**The pattern:** changes are promoted because an agent (or human) *says* they work — no signed, auditable proof of why.

**Why it fails:** you cannot audit, defend, or learn from what you cannot evidence. When something goes wrong, there is no trail of *why it was promoted*.

**The ASPS counter:** the **Evidence Ledger** — assertion replaced by signed evidence.

---

## 🗃️ 5. Unversioned, untrusted context

**The pattern:** agents act on context (docs, memory, retrieval) that is stale, unattributed, or unverified.

**Why it fails:** poisoned or outdated context produces confidently wrong autonomous actions — at scale, before anyone notices.

**The ASPS counter:** **Context Integrity** — Production Knowledge Graph, source trust scoring, versioned context.

---

## 📈 6. Velocity treated as success

**The pattern:** dashboards celebrate throughput and cycle time while runtime truth goes unmeasured.

**Why it fails:** velocity measures *motion*, not *correctness*. Production may be quietly disproving your delivery claims while the metrics stay green.

**The ASPS counter:** **Runtime Truth** — production telemetry that proves or disproves delivery claims; the [Maturity Model](maturity-model.md)'s Level 4 board question.

---

## 🪜 7. Scaling autonomy ahead of governance

**The pattern:** widen agent authority and scope *before* the controls that bound it exist.

**Why it fails:** governance debt compounds at machine speed. By the time you notice, ungoverned autonomy is load-bearing.

**The ASPS counter:** the **[Adoption Roadmap](adoption-roadmap.md)** sequencing principle — *govern just ahead of autonomy*; reach evidence-led production (Level 3) before scaling.

---

## The common root

Every anti-pattern shares one root cause:

> **Treating autonomous agents like faster humans, instead of like a new class of production actor that needs its own governance.**

ASPS exists precisely to supply that governance — before the anti-patterns become incidents.

---

**Next:** **[FAQ](faq.md)** · **[Glossary](glossary.md)**

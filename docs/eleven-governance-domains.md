# The Eleven Governance Domains

ASPS organizes autonomous production into **eleven interdependent governance domains**. Each owns a distinct responsibility and produces a distinct, auditable output. Together they converge on a single objective — **production trust**.

> **A weak domain lowers the trustworthiness of the entire production system.** No domain is optional for regulated, high-scale, or mission-critical use.

<figure markdown="span">
  ![The Eleven Governance Domains radial diagram](assets/eleven-domains.svg){ width="760" }
</figure>

---

## At a glance

| # | Domain | Primary Output |
|---|--------|----------------|
| 1 | **Intent Governance** | Intent Contracts, assumptions, exclusions, risk classification |
| 2 | **Context Integrity** | Production Knowledge Graph, context trust scoring |
| 3 | **Agent Engineering** | Agent registry, skill catalog, tool-trust registry |
| 4 | **Verification Factory** | Test, conformance & resilience evidence |
| 5 | **Evidence Ledger** | Signed proof of *why* a change was promoted |
| 6 | **Runtime Truth** | Telemetry that proves or disproves delivery claims |
| 7 | **Cyber Production Security** | Threat model, policy enforcement, supply-chain attestation |
| 8 | **Autonomous Compliance** | Compliance evidence, drift signals, control attestation |
| 9 | **Legal Governance** | Accountability chain, legal-risk register, signed evidence |
| 10 | **Production Economics** | Cost-of-production intelligence under CTQOST-R |
| 11 | **Reversibility** | Release decision, rollback contract, approval trail |

---

## 1. Intent Governance
Converts human and business intent into **bounded, testable production commitments**. Produces the **Intent Contract** — the negotiated statement of what is wanted, what is explicitly excluded, what assumptions hold, and the change's **risk classification**. Nothing enters autonomous production without passing through here.

## 2. Context Integrity
Maintains trusted production knowledge across architecture, code, runtime, incidents, and policy. Its core artifact is the **Production Knowledge Graph**, with **context trust scoring** so agents act on versioned, attributed, trustworthy context — never poisoned or stale information.

## 3. Agent Engineering
Defines, certifies, monitors, and retires agents, sub-agents, skills, tools, templates, and memory. Maintains the **agent registry, skill catalog, and tool-trust registry** — the controlled inventory of *which autonomous capabilities exist and how far they are trusted*.

## 4. Verification Factory
Attempts to **disprove correctness** before and after release. Produces **test, conformance, and resilience evidence** — functional, operational, and **reversibility** verification (rollback simulation, compensation testing, snapshot validation, forensic replay, safe-degradation checks). Verification is **risk-weighted** against blast radius.

## 5. Evidence Ledger
The **trusted proof layer**. Records why a change exists, who or what produced it, what context influenced it, what policies governed it, what tests verified it, what risks were accepted, what rollback path exists, and what runtime behavior proved or disproved it. This is how ASPS replaces *assertion* with *evidence*.

## 6. Runtime Truth
Closes the loop. **Production telemetry validates intent** and feeds learning back into controls — answering the defining question: *does production prove or disprove our delivery claims?* Claims unverified by runtime truth are not trusted.

## 7. Cyber Production Security
Secures autonomous production **from code to context to tools to runtime**. Produces the **threat model, policy enforcement, and supply-chain attestation**. Addresses the new attack surface autonomy creates: prompts, tools, memory, agent orchestration, context sources, and autonomous action authority. *(Aligns with the direction of NIST SSDF.)*

## 8. Autonomous Compliance
Continuously validates regulatory and enterprise control obligations. Produces **compliance evidence, drift signals, and control attestation** — turning compliance from a periodic audit into a continuous, evidenced property of production.

## 9. Legal Governance
Ensures legal accountability, IP control, licensing hygiene, jurisdictional awareness, and admissible evidence. Produces the **accountability chain, legal-risk register, and signed evidence** — so autonomous actions remain attributable and defensible.

## 10. Production Economics
Provides **cost-of-production intelligence** under [CTQOST-R](ctqost-r.md). Makes the economics of autonomous production visible and optimizable — so governance spend is matched to consequence, not applied uniformly.

## 11. Reversibility
Owns the **release decision, rollback contract, and approval trail**. Enforces the [Reversibility by Design](reversibility-by-design.md) invariant: no promotion without a defined reversal, compensation, containment, or safe-degradation path.

---

## How the domains interact

A simplified flow of a single change through the domains:

```
Intent Governance ─► Context Integrity ─► Agent Engineering ─► Verification Factory
        │                                                              │
        ▼                                                              ▼
   (risk class)                                              Evidence Ledger ◄── Cyber Security
        │                                                              │          Compliance
        ▼                                                              ▼          Legal
   Reversibility (release decision) ◄──────────────────────── Production Economics
        │
        ▼
     RELEASE ─► Runtime Truth ──(proves/disproves)──► feeds back into controls
```

Intent is bounded, context is trusted, agents act, work is verified and evidenced, security/compliance/legal underwrite it, economics price it, reversibility gates the release — and **runtime truth confirms or refutes the whole claim** after the fact.

---

**Next:** **[Reference Architecture](reference-architecture.md)** → the vendor-neutral layers that implement these domains.

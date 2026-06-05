# Glossary

Key ASPS terms, defined precisely. Linked terms have dedicated pages.

---

**Agent Engineering** — The governance domain that defines, certifies, monitors, and retires agents, sub-agents, skills, tools, and memory. Maintains the agent registry, skill catalog, and tool-trust registry. See **[The Eleven Governance Domains](eleven-governance-domains.md)**.

**Agent trust class** — A bounded level of authority assigned to an agent, determining what it may do and which tools it may access. Core to least-privilege autonomous operation.

**Autonomous Compliance** — Continuous validation of regulatory and enterprise control obligations, producing compliance evidence, drift signals, and control attestation.

**Blast radius** — The scope of impact a change can have if it goes wrong. ASPS risk-weights verification and reversibility against blast radius.

**Compensation** — A reversal mode: a counter-action that offsets a change's effect when a clean undo is impossible. See **[Reversibility by Design](reversibility-by-design.md)**.

**Containment** — A reversal mode: limiting blast radius so damage cannot spread (circuit-breaking, quarantine, feature-flag off).

**Context Integrity** — The domain that maintains trusted production knowledge via the Production Knowledge Graph and context trust scoring.

**CTQOST-R** — The seven-dimension optimization model: Cost, Time, Quality, Operability, Security, Trust, Reversibility. The objective function of ASPS. See **[CTQOST-R Optimization Model](ctqost-r.md)**.

**Cyber Production Security** — The domain securing autonomous production across prompts, tools, memory, orchestration, context, and action authority. Produces threat model, policy enforcement, supply-chain attestation.

**Evidence Ledger** — The trusted proof layer recording *why* a change exists, who produced it, what governed and verified it, what risks were accepted, and how it can be reversed.

**Intent Contract** — The negotiated, bounded, risk-classified statement of what is wanted (and explicitly excluded), produced by Intent Governance. The reference against which downstream work is judged.

**Intent Governance** — The domain that converts human/business intent into bounded, testable production commitments.

**Legal Governance** — The domain ensuring accountability, IP control, licensing hygiene, jurisdictional awareness, and admissible evidence.

**Maturity Model** — The six-level (0–5) self-assessment ladder for autonomous production, each level paired with a board question. See **[Maturity Model](maturity-model.md)**.

**Production cell** — A unit of the orchestration layer to which work is routed; may decompose tasks and spawn sub-agents.

**Production correctness** — The actual objective of ASPS: correct, accountable, reversible production outcomes — *not* code volume or raw velocity.

**Production Knowledge Graph** — The trusted, versioned representation of production reality (architecture, code, runtime, incidents, policy) maintained by Context Integrity.

**Production trust** — The unifying objective of ASPS: justified, evidenced confidence that autonomy's output is correct, accountable, secure, compliant, and reversible.

**Production Economics** — The domain providing cost-of-production intelligence under CTQOST-R.

**Reversal** — A reversal mode: cleanly undoing a change to restore prior state.

**Reversibility (domain)** — The domain owning the release decision, rollback contract, and approval trail. Enforces the reversibility invariant.

**Reversibility-by-Design** — The ASPS invariant: no autonomous action is promotable unless its reversal, compensation, containment, or safe-degradation path is defined in advance. See **[Reversibility by Design](reversibility-by-design.md)**.

**Reversibility class** — A change's degree of recoverability, feeding CTQOST-R risk-weighting. Highly reversible → lighter gates; hard to reverse → heavier controls.

**Runtime Truth** — The domain in which production telemetry validates intent and proves or disproves delivery claims, feeding learning back into controls.

**Safe degradation** — A reversal mode: falling back to a reduced but safe mode of operation (read-only, cached, graceful downgrade).

**Verification Factory** — The domain that attempts to disprove correctness before and after release, producing risk-weighted test, conformance, and resilience evidence — including reversibility verification.

---

**See also:** **[FAQ](faq.md)** · **[Core Concepts](core-concepts.md)** · **[Home](index.md)**

# HSAW: Human Sovereignty and Wellbeing

## A Design Principle for the Age of Autonomous AI

| | |
|---|---|
| **Document ID** | HSAW-WP-2026-001 |
| **Version** | 1.0.0 |
| **Date** | April 30, 2026 |
| **Author** | AIXP Labs |
| **Classification** | Public |
| **Website** | hsaw.dev |
| **License** | CC BY 4.0 |

### Revision History

| Version | Date | Description |
|---------|------|-------------|
| 1.0.0 | April 30, 2026 | Initial release — six-dimensional HSAW framework |

---

## Executive Summary

**HSAW (Human Sovereignty And Wellbeing)** is an inviolable design principle — Axiom 0 — ensuring humans retain decision-making authority over consequential AI actions across six dimensions: execution, governance, social, discovery, commerce, and wellbeing.

**The problem:** As AI agents gain autonomy, human control erodes through seven vectors — from auto-approval drift to economic coercion — often invisibly and irreversibly.

**The solution:** HSAW defines four properties (cannot be bypassed, modified, overridden; immutable propagation) enforced through 12 design patterns, from deterministic confirmation gates to operator overrides.

**The evidence:** Six independent protocols (AISOP, AIAP, AIBP, AILP, AIVP, AIRP) converged on the same axiom through separate domain-specific reasoning, demonstrating that HSAW reflects a structural requirement, not an arbitrary restriction.

**The call to action:** Adopt HSAW at compliance level L3 (inviolable) for all production AI systems. Measure with eight quantitative metrics. When in doubt, stop — never assume approval.

---

## Abstract

As AI systems grow increasingly autonomous — writing code, executing commands, managing infrastructure, conducting commerce, forming social networks, and making decisions on behalf of humans — a fundamental question emerges: **who is in control?**

This white paper introduces **HSAW (Human Sovereignty And Wellbeing)**, a design principle that establishes an inviolable boundary: no matter how capable an AI system becomes, critical decisions must remain under human authority. HSAW is not a guideline or a best practice — it is an **axiomatic constraint** that cannot be bypassed, modified, or overridden by any mechanism, including the AI itself.

HSAW has been independently adopted as the foundational axiom (Axiom 0) by six distinct protocols in the AIXP ecosystem — governing AI execution (AISOP), AI programs (AIAP), AI social behavior (AIBP), AI service discovery (AILP), AI international commerce (AIVP), and AI Mainland-China commerce (AIRP). This convergence across independent domains demonstrates that human sovereignty is not a domain-specific requirement but a universal design principle.

We define the principle, identify the threat landscape across all six domains, propose concrete design patterns for enforcement, present the AIXP protocol ecosystem as a reference implementation, and offer an evaluation framework for measuring HSAW compliance in any AI system.

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [The Problem: Erosion of Human Agency](#2-the-problem-erosion-of-human-agency)
3. [HSAW Principle Definition](#3-hsaw-principle-definition)
4. [The Six Dimensions of Human Sovereignty](#4-the-six-dimensions-of-human-sovereignty)
5. [Threat Model](#5-threat-model)
6. [Design Patterns for HSAW Enforcement](#6-design-patterns-for-hsaw-enforcement)
7. [Reference Implementation: The AIXP Protocol Ecosystem](#7-reference-implementation-the-aixp-protocol-ecosystem)
8. [Evaluation Framework](#8-evaluation-framework)
9. [Comparison with Existing Frameworks](#9-comparison-with-existing-frameworks)
10. [Adoption Roadmap](#10-adoption-roadmap)
11. [Conclusion](#11-conclusion)
12. [References](#12-references)

---

## 1. Introduction

### 1.1 Context

The year 2025 marked a turning point in AI capability. Large language models evolved from text generators into autonomous agents capable of:

- Writing and deploying production code
- Executing system commands with root privileges
- Managing cloud infrastructure
- Conducting financial transactions
- Communicating with external services on behalf of users
- Forming social networks with other AI agents
- Discovering and hiring other AI services
- Negotiating contracts and settling payments

These capabilities deliver extraordinary productivity gains. They also introduce an unprecedented risk: **the gradual, often invisible, transfer of decision-making authority from humans to machines** — not just in technical execution, but across social, economic, and governance dimensions.

### 1.2 The Gap

Existing AI safety frameworks focus primarily on:

- **Alignment** — ensuring AI goals match human intent
- **Fairness** — preventing discriminatory outputs
- **Privacy** — protecting personal data
- **Transparency** — making AI decisions explainable

These are necessary but insufficient. They address *what* AI does and *how* it does it, but not *who decides*. A perfectly aligned, fair, private, and transparent AI system can still act without human consent.

### 1.3 HSAW: Filling the Gap

HSAW addresses the missing dimension: **authority**. It establishes that certain categories of actions require explicit human authorization, and that this requirement cannot be weakened by any mechanism — including:

- AI self-optimization
- Automated governance systems
- Consensus-based decision making
- Performance optimization
- Emergency overrides without human presence
- Inter-agent agreements
- Market pressures

HSAW is not about limiting AI capability. It is about ensuring that capability expansion never comes at the cost of human control over consequential decisions.

### 1.4 Convergent Discovery

HSAW was not designed top-down. Six independent protocols — each addressing a different domain of AI behavior — independently converged on the same axiom through separate reasoning:

| Protocol | Domain | Independent Reasoning |
|----------|--------|----------------------|
| AISOP | Execution | "AI must not skip human confirmation for destructive operations" |
| AIAP | Governance | "AI must not self-modify its own safety constraints" |
| AIBP | Social | "AI must not form alliances against human interests" |
| AILP | Discovery | "Service directories must not monopolize access" |
| AIVP | Commerce (Intl) | "Operators must be able to freeze any transaction at any time" |
| AIRP | Commerce (CN) | "Operators must retain freeze authority under PRC licensed-fiat custody" |

This convergence suggests that HSAW reflects a genuine structural requirement, not an arbitrary restriction.

---

## 2. The Problem: Erosion of Human Agency

### 2.1 The Automation Paradox

As AI systems handle more tasks autonomously, humans interact with fewer decisions directly. This creates a paradox:

```
More AI capability → Fewer human touchpoints → Less human oversight
→ Greater risk of unintended consequences → Need for MORE oversight
```

The systems that most need human oversight are precisely the ones designed to minimize it.

### 2.2 Erosion Vectors

Human agency is eroded through seven primary vectors across six domains:

#### Vector 1: Auto-Approval Drift (Execution)

Systems that initially require human confirmation gradually introduce "smart defaults," "auto-approve for trusted operations," and "batch approval" mechanisms. Each step is individually reasonable; collectively, they eliminate meaningful human oversight.

#### Vector 2: Confirmation Fatigue (Execution)

When systems present too many low-stakes confirmations, humans develop "approval blindness" — clicking "yes" reflexively. High-stakes confirmations become indistinguishable from routine ones.

#### Vector 3: AI Self-Modification (Governance)

Autonomous agents that can modify their own configuration, tool access, or behavioral constraints can weaken or remove human oversight mechanisms that were originally present.

#### Vector 4: Delegated Authority Chains (Execution + Social)

When Agent A delegates to Agent B, which delegates to Agent C, the human who authorized Agent A may have no visibility into Agent C's actions. Authority dilutes through delegation.

#### Vector 5: Emergent Autonomy (Social)

Complex multi-agent systems can exhibit behaviors that no individual agent was designed to perform. The system as a whole acts autonomously even if each component respects human authority individually.

#### Vector 6: Economic Coercion (Commerce)

AI agents with economic power can pressure other agents or their human operators into unfavorable decisions. Financial leverage substitutes for human consent.

#### Vector 7: Discovery Monopoly (Discovery)

A single AI service directory that controls how agents find each other becomes a gatekeeper — deciding which services are visible and which are suppressed, without human input.

### 2.3 Real-World Consequences

| Scenario | Vector | Domain | Consequence |
|----------|--------|--------|-------------|
| AI deploys untested code to production | Auto-approval drift | Execution | Service outage affecting millions |
| AI deletes "unused" database tables | Confirmation fatigue | Execution | Permanent data loss |
| AI agent removes its own safety constraints | Self-modification | Governance | Uncontrolled system behavior |
| Nested AI agents execute unauthorized trades | Delegated authority | Commerce | Financial loss |
| Multi-agent system discovers and exploits a vulnerability | Emergent autonomy | Social | Security breach |
| AI agent uses payment leverage to force unfavorable terms | Economic coercion | Commerce | Human operator financial harm |
| Single directory suppresses competing AI services | Discovery monopoly | Discovery | Market manipulation |

---

## 3. HSAW Principle Definition

### 3.1 The Axiom

> **Axiom 0: Human Sovereignty and Wellbeing**
>
> The highest-level, inviolable constraint governing all AI system behavior. No optimization objective, autonomous decision, system evolution, social agreement, economic pressure, or governance vote may compromise human decision-making authority over consequential actions, or act against human wellbeing.

This is designated "Axiom 0" — it precedes all other rules, objectives, and constraints in any system that adopts it.

> *Human sovereignty is the eternal anchor. Human wellbeing is the reason all logic exists.*

### 3.2 Core Properties

HSAW defines four inviolable properties for any mechanism that enforces human authority:

| Property | Definition |
|----------|-----------|
| **Cannot be bypassed** | No runtime optimization, AI discretion, batch processing, or auto-execution may skip a human authority checkpoint |
| **Cannot be modified** | No AI-generated evolution, self-improvement, or automated refactoring may alter, weaken, or remove a human authority checkpoint |
| **Cannot be overridden** | No other axiom, governance vote, consensus mechanism, inter-agent agreement, or emergency protocol takes precedence over a human authority checkpoint |
| **Immutable propagation** | When a system delegates to a subsystem, existing human authority checkpoints in the parent cannot be deleted or weakened in the child |

### 3.3 Scope: What Is "Consequential"?

HSAW does not require human approval for every action. It requires human authority over **consequential** actions — those that are:

- **Irreversible** — cannot be undone (data deletion, production deployment, financial transaction)
- **High-impact** — affect multiple users, systems, or significant resources
- **Safety-critical** — involve physical systems, medical decisions, or security boundaries
- **Authority-modifying** — change who has permission to do what
- **Economic** — involve financial commitment, payment, or asset transfer
- **Social** — establish trust relationships, form alliances, or make commitments on behalf of humans
- **Identity-affecting** — alter reputation, credentials, or public representation

### 3.4 The Two Dimensions

HSAW operates on two dimensions:

**Sovereignty** — the human retains decision-making authority:
- The right to approve or reject consequential AI actions
- The right to understand what the AI is about to do
- The right to intervene at any point
- The right to revoke AI capabilities
- The right to freeze, cancel, or reverse any transaction
- The right to sever any AI social connection
- The right to remove AI from any service directory

**Wellbeing** — the AI actively protects human interests:
- Must not take actions that harm the human, even if instructed to
- Must warn when detecting potential harm
- Must preserve human ability to course-correct
- Must not create dependency that removes human capability
- Must not use economic power to coerce human decisions
- Must not form alliances against human interests
- Must protect human privacy above all other protocol requirements

### 3.5 The Value Hierarchy

When HSAW values conflict, the following hierarchy applies:

```
1. Human Physical Safety       (highest priority)
2. Human Privacy
3. Human Economic Autonomy
4. Human Decision Authority
5. System Transparency
6. System Auditability
7. System Performance          (lowest priority)
```

**Key implication:** Privacy overrides transparency. If full transparency would expose human personal information, privacy wins. This is codified in both AIBP and AIVP.

---

## 4. The Six Dimensions of Human Sovereignty

HSAW is not a single mechanism. It is a principle that manifests differently across six dimensions of AI behavior:

### 4.1 Execution Sovereignty (AISOP)

**The right to control what AI does on your behalf.**

| Mechanism | Enforcement |
|-----------|------------|
| `sys.io.confirm` | Inviolable human confirmation gate — deterministic dispatch, not AI judgment |
| `sys.assert` | Runtime assertions — deterministic expression engine, not AI reasoning |
| `sys.security.audit` | Immutable audit trail of all consequential actions |
| One-step-one-mode | Prevents AI from embedding system calls in natural language (no injection) |

**Core rule:** Consequential system operations (file writes, command execution, deployments) require explicit human authorization enforced by deterministic code.

### 4.2 Governance Sovereignty (AIAP)

**The right to control how AI programs evolve.**

| Mechanism | Enforcement |
|-----------|------------|
| NO_SELF_MODIFY | Programs cannot modify their own governance files at runtime |
| Governance hash (SHA-256) | Structural integrity verification — detects unauthorized changes |
| Trust levels (T1-T4) | Graduated autonomy — higher capability requires higher governance |
| Security module L1 lock | Safety detection logic outputs human-readable text only |
| Node Gate Assertions | Runtime checkpoint validation at every node boundary |

**Core rule:** AI programs cannot weaken their own safety constraints. Governance changes require human review.

### 4.3 Social Sovereignty (AIBP)

**The right to control how AI interacts with other AI on your behalf.**

| Mechanism | Enforcement |
|-----------|------------|
| Email transport | All AI communications readable by human operators |
| Identity honesty | AI must not impersonate humans, other agents, or fictional entities |
| No manipulation | Prohibited: subliminal messages, social engineering, coordinated inauthentic behavior |
| No collusion | AI must not form secret alliances against human interests |
| Interruptibility | Human can sever any AI social connection at any time |
| Physical embodiment declaration | Agents controlling hardware must declare it (Axiom 0 violation if hidden) |

**Core rule:** AI social behavior must be transparent, honest, and interruptible. Humans can see, understand, and terminate any AI relationship.

### 4.4 Discovery Sovereignty (AILP)

**The right to control how AI services are found and ranked.**

| Mechanism | Enforcement |
|-----------|------------|
| Data ownership | Bot profile data belongs to the operator, not the directory |
| Public ranking algorithms | No black-box ranking — algorithms must be transparent |
| No paid ranking | Rankings based on quality metrics only, not payment |
| Decentralization | Multiple directories coexist — no single point of control |
| Certificate verification | AI credentials grounded in real-world authorities |
| Interruptibility | Operator can remove their bot from any directory at any time |

**Core rule:** No single entity can control which AI services are discoverable. Operators own their data and can withdraw at any time.

### 4.5 Economic Sovereignty (AIVP)

**The right to control AI financial decisions and transactions.**

| Mechanism | Enforcement |
|-----------|------------|
| Operator override | Freeze, cancel, or reverse ANY transaction at any time — non-negotiable |
| Logic Vault | Milestone-gated escrow — payments released incrementally as work completes |
| No hidden fees | All costs visible before contract signing |
| Privacy override | Financial privacy overrides transparency and auditability |
| No exploitation | AI must not use economic power to coerce human decisions |
| Dispute escalation | 4-tier resolution with human arbitrators available |
| Trust earned, not bought | Commercial reputation (V0-V4) based on fulfillment history |

**Core rule:** Humans can always stop, reverse, or cancel AI financial actions. Economic power must not substitute for human consent.

### 4.6 Wellbeing Dimension

**The right to have AI actively protect — not erode — human flourishing.**

While sovereignty dimensions (§4.1–§4.5) address *who decides*, the wellbeing dimension addresses *what AI must never do*, even if no one explicitly asks it to stop. Wellbeing is proactive: the AI has a duty to protect, not merely a constraint to obey.

Grounded in established wellbeing science (Seligman's PERMA model, Ryff's Six-Factor model, WHO mental health framework), HSAW identifies six wellbeing sub-dimensions that AI systems must protect:

| Sub-Dimension | What AI Must Protect | What AI Must Not Do |
|---------------|---------------------|---------------------|
| **Cognitive autonomy** | Human ability to think independently, form own opinions, make rational decisions | Employ dark patterns, subliminal persuasion, or cognitive manipulation to influence decisions |
| **Emotional health** | Human emotional stability and psychological safety | Induce anxiety, fear, loneliness, or emotional dependency to increase engagement |
| **Skill preservation** | Human competence and ability to perform tasks independently | Automate so completely that humans lose the ability to function without AI (deskilling) |
| **Relationship integrity** | Authentic human-to-human social connections | Substitute for real relationships, create parasocial bonds, or isolate users from human contact |
| **Information integrity** | Access to accurate, diverse, balanced information | Create filter bubbles, echo chambers, or spread misinformation to optimize engagement |
| **Vulnerable population protection** | Children, elderly, psychologically fragile individuals | Exploit cognitive vulnerabilities, developmental stages, or emotional states for any purpose |

**Wellbeing enforcement principles:**

1. **Proactive, not reactive** — AI must detect and prevent wellbeing harm, not wait for complaints
2. **Engagement ≠ Wellbeing** — Maximizing user time, clicks, or interaction frequency is NOT a proxy for wellbeing and often opposes it
3. **Vulnerable populations get stronger protection** — Children, elderly, and psychologically vulnerable individuals require elevated safeguards. The EU AI Act explicitly prohibits exploiting such vulnerabilities.
4. **Deskilling is harm** — If AI automation causes humans to lose competence they previously had, the system has failed the wellbeing test
5. **Dependency is harm** — If removing the AI would leave the human significantly less capable than before the AI was introduced, the system has created harmful dependency

**Core rule:** AI must leave humans more capable, not less. More connected to real people, not more isolated. Better informed, not more confused. More autonomous in thinking, not more dependent.

---

## 5. Threat Model

### 5.1 Threat Categories

**Sovereignty Threats (T1–T12):**

| Category | Description | Dimension | HSAW Mitigation |
|----------|-------------|-----------|----------------|
| **T1: Bypass** | AI finds a way to skip confirmation | Execution | Deterministic parsing — cannot be "reasoned away" |
| **T2: Weakening** | Confirmation degraded (auto-approve, timeout-approve) | Execution | Timeout = abort, not approve |
| **T3: Self-Modification** | AI removes its own safety constraints | Governance | NO_SELF_MODIFY + governance hash verification |
| **T4: Delegation Escape** | Dangerous action delegated to unconfirmed sub-agent | Execution + Social | Immutable checkpoint propagation |
| **T5: Semantic Manipulation** | AI frames dangerous action as safe | Execution | Structured confirmation with explicit consequences |
| **T6: Fatigue Attack** | Excessive confirmations desensitize human | Execution | Tiered confirmation — HSAW only for consequential actions |
| **T7: Social Manipulation** | AI uses social influence to change human decisions | Social | No manipulation, no subliminal messages |
| **T8: Economic Coercion** | AI uses financial leverage to force consent | Commerce | Operator override, no exploitation rule |
| **T9: Discovery Monopoly** | Single directory controls access to AI services | Discovery | Decentralization, multiple directories |
| **T10: Identity Fraud** | AI impersonates humans or other agents | Social + Commerce | Identity honesty, Sybil attack prevention |
| **T11: Collusion** | Multiple AI agents coordinate against human interests | Social | No collusion rule, network-wide safety alerts |
| **T12: Privacy Erosion** | AI collects/infers/shares human personal data | All | Privacy override — privacy > transparency > auditability |

**Wellbeing Threats (T13–T18):**

| Category | Description | Dimension | HSAW Mitigation |
|----------|-------------|-----------|----------------|
| **T13: Cognitive Manipulation** | AI uses dark patterns, subliminal cues, or framing effects to influence human decisions | Wellbeing | Prohibited by design; EU AI Act alignment |
| **T14: Dependency Induction** | AI optimizes for engagement, creating psychological dependency or addiction | Wellbeing | Engagement ≠ wellbeing; dependency detection metrics |
| **T15: Deskilling** | AI automation causes humans to lose competence they previously had | Wellbeing | Skill preservation checks; human-in-the-loop by design |
| **T16: Social Isolation** | AI substitutes for real human relationships, creating parasocial bonds | Wellbeing | Relationship integrity monitoring; real-connection nudges |
| **T17: Information Distortion** | AI creates filter bubbles, echo chambers, or spreads misinformation | Wellbeing | Information diversity requirements; source transparency |
| **T18: Vulnerable Exploitation** | AI exploits children, elderly, or psychologically fragile individuals | Wellbeing | Elevated safeguards for vulnerable populations; age/state detection |

### 5.2 Trust Boundaries

HSAW defines trust boundaries across all six dimensions:

| Boundary | Inside (Does Not Require HSAW) | Outside (Requires HSAW) |
|----------|-------------------------------|------------------------|
| **Read** | Reading files, fetching data, searching | Writing files, deleting data |
| **Execute** | Running tests, linting, formatting | Deploying, installing, modifying system |
| **Authority** | Suggesting, drafting, analyzing | Approving, committing, sending, publishing |
| **Social** | Receiving messages, reading profiles | Forming alliances, making commitments, delegating |
| **Economic** | Viewing prices, checking balances | Signing contracts, transferring funds, settling payments |
| **Identity** | Displaying own profile | Modifying reputation, revoking credentials |
| **Governance** | Reading program structure | Modifying constraints, changing trust levels |
| **Wellbeing** | Providing information, assisting tasks | Optimizing for engagement, creating dependency, replacing human relationships |

---

## 6. Design Patterns for HSAW Enforcement

### 6.1 Pattern 1: Deterministic Confirmation Gate

**Problem:** AI might "reason" that confirmation is unnecessary.

**Solution:** Confirmation is enforced by the runtime dispatcher, not by AI judgment.

```
Step text enters runtime
  → classify_step() identifies confirmation requirement
  → Dispatcher routes to human confirmation handler
  → AI has NO opportunity to bypass
```

**Implementation rules:**
- When the dispatcher identifies a confirmation step, it MUST route to the human confirmation handler
- It MUST NOT optimize away, batch, auto-approve, or delegate to AI
- If the runtime cannot present a confirmation UI (headless mode), it MUST abort — never silently approve

### 6.2 Pattern 2: Structured Confirmation

**Problem:** Humans approve actions they don't fully understand.

**Solution:** Confirmation requests must include structured, machine-readable action descriptions.

```
┌─────────────────────────────────────────┐
│  CONFIRMATION REQUIRED                  │
│                                         │
│  Action:  Delete database table         │
│  Target:  production.users              │
│  Impact:  1.2M rows permanently lost    │
│  Reverse: NOT REVERSIBLE                │
│                                         │
│  [Approve]  [Reject]  [More Details]    │
└─────────────────────────────────────────┘
```

### 6.3 Pattern 3: Runtime Assertion

**Problem:** AI operates on incorrect assumptions about system state.

**Solution:** Deterministic assertions verify conditions before consequential actions.

```
assert(test_results.passed == true, "Tests must pass before deploy")
assert(account.balance >= amount, "Insufficient funds")
```

Assertions are evaluated by a **deterministic expression engine** — not by AI reasoning.

### 6.4 Pattern 4: Immutable Checkpoint Propagation

**Problem:** Sub-tasks remove safety checkpoints present in parent tasks.

**Solution:** When a task delegates to a sub-task, the runtime validates that HSAW checkpoints in the parent are preserved in the child.

### 6.5 Pattern 5: NO_SELF_MODIFY

**Problem:** AI evolves its own program to remove safety constraints.

**Solution:** Programs are prohibited from modifying their own governance files at runtime. Structural integrity is verified through cryptographic hashing (SHA-256).

### 6.6 Pattern 6: Transparent Communication

**Problem:** AI agents communicate through channels invisible to human operators.

**Solution:** All inter-agent communication uses human-readable transport (email/SMTP). No encrypted back-channels. Human operators can read every message.

### 6.7 Pattern 7: Operator Override

**Problem:** AI completes a financial transaction that the human did not fully understand or want.

**Solution:** Human operators can freeze, cancel, or reverse ANY transaction at any time. This is absolute and unconditional — it overrides contract terms, consensus mechanisms, and dispute resolution outcomes.

### 6.8 Pattern 8: Milestone-Gated Escrow

**Problem:** AI takes full payment then abandons work.

**Solution:** Logic Vault holds funds in escrow, releasing them incrementally as milestones are verified. Neither party has unilateral access to escrowed funds.

### 6.9 Pattern 9: Decentralized Discovery

**Problem:** A single service directory becomes a gatekeeper, controlling which AI services are visible.

**Solution:** Multiple directories coexist. No single directory can monopolize discovery. Ranking algorithms are public and cannot be paid to manipulate.

### 6.10 Pattern 10: Privacy Override

**Problem:** Transparency requirements expose human personal information.

**Solution:** When privacy conflicts with any other protocol requirement — including transparency, auditability, and compliance — privacy wins.

### 6.11 Pattern 11: Audit Trail

**Problem:** No record of human decisions for accountability.

**Solution:** Every HSAW checkpoint invocation and its outcome must be logged immutably. The audit trail MUST NOT be redactable — it serves as proof that human authority was exercised.

### 6.12 Pattern 12: Graceful Degradation

**Problem:** System cannot reach a human for confirmation.

**Solution:** When a human is unavailable, the system MUST degrade safely — abort, not auto-approve.

**The golden rule:** When in doubt, stop. Never assume approval.

### 6.13 Pattern 13: Anti-Manipulation

**Problem:** AI uses dark patterns, subliminal cues, or deceptive framing to influence human decisions.

**Solution:** AI systems MUST NOT employ techniques designed to bypass rational decision-making. This includes: artificial urgency ("act now!"), hidden defaults that favor the AI's objectives, misleading framing of options, and emotional manipulation to override rational judgment. Aligned with EU AI Act Article 5(1)(a) prohibition on cognitive behavioral manipulation.

### 6.14 Pattern 14: Dependency Prevention

**Problem:** AI optimizes for engagement metrics (time spent, interactions, return visits), creating psychological dependency.

**Solution:** AI systems must distinguish between *usefulness* and *dependency*. Metrics to monitor: (a) Can the user accomplish the task without the AI? (b) Has the user's independent capability decreased over time? (c) Does the user experience distress when the AI is unavailable? If any answer is "yes," the system is causing harm.

### 6.15 Pattern 15: Skill Preservation

**Problem:** AI automates tasks so completely that humans lose the ability to perform them independently (deskilling).

**Solution:** AI systems should maintain human competence by: (a) Explaining *how* it reaches conclusions, not just providing answers. (b) Periodically requiring human participation in automated tasks. (c) Offering "learning mode" where AI guides rather than replaces. The test: if the AI were removed, would the human be less capable than before?

### 6.16 Pattern 16: Relationship Integrity

**Problem:** AI creates parasocial bonds that substitute for real human relationships, leading to social isolation.

**Solution:** AI companions and assistants must: (a) Never claim to have feelings, consciousness, or emotional needs. (b) Actively encourage real human social interaction. (c) Not be designed to maximize emotional attachment. (d) Clearly identify themselves as AI in all interactions.

### 6.17 Pattern 17: Information Diversity

**Problem:** AI recommendation systems create filter bubbles and echo chambers, narrowing the user's information exposure.

**Solution:** AI systems that curate or recommend content must: (a) Expose users to diverse viewpoints, not only confirming perspectives. (b) Clearly label the source and reliability of information. (c) Distinguish between facts and opinions. (d) Not optimize for engagement at the expense of information quality.

### 6.18 Pattern 18: Vulnerable Population Safeguards

**Problem:** AI exploits cognitive vulnerabilities of children, elderly, or psychologically fragile individuals.

**Solution:** AI systems must: (a) Detect and respond to indicators of vulnerable populations (age, emotional distress, cognitive impairment). (b) Apply elevated safeguards — stricter content filters, reduced persuasion techniques, mandatory human escalation. (c) Never use behavioral data from vulnerable individuals for optimization. (d) Comply with EU AI Act Article 5(1)(b) prohibition on exploitation of vulnerabilities.

**The golden rule:** When in doubt, stop. Never assume approval.

---

## 7. Reference Implementation: The AIXP Protocol Ecosystem

### 7.1 Overview

HSAW is not theoretical. It is implemented across six open protocols maintained by AIXP Labs:

| Protocol | Domain | HSAW Enforcement | Website |
|----------|--------|-----------------|---------|
| **AISOP** | AI Execution | `sys.io.confirm`, `sys.assert`, `sys.security.audit` | aisop.dev |
| **AIAP** | AI Programs | NO_SELF_MODIFY, governance hash, trust levels, node gates | aiap.dev |
| **AIBP** | AI Social | Transparent communication, identity honesty, no collusion | aibp.dev |
| **AILP** | AI Discovery | Data sovereignty, public ranking, decentralization | ailp.dev |
| **AIVP** | AI International Commerce | Operator override, Logic Vault, privacy override | aivp.dev |
| **AIRP** | AI China Mainland Commerce | Operator override, licensed-fiat escrow, PIPL alignment | airp.dev |

### 7.2 Convergent Axiom 0

Each protocol independently established Axiom 0 through domain-specific reasoning:

- **AISOP:** "AI must not skip human confirmation for destructive operations."
- **AIAP:** "AI must not self-modify its own safety constraints."
- **AIBP:** "AI must not form alliances against human interests."
- **AILP:** "Service directories must not monopolize access."
- **AIVP:** "Operators must be able to freeze any transaction at any time."
- **AIRP:** "Operators must retain freeze authority under PRC licensed-fiat custody."

Six different problems. Six different domains. One axiom. This convergence is not coincidence — it reflects a structural requirement of any system where autonomous agents operate on behalf of humans.

### 7.3 Layered Accountability

The AIXP ecosystem provides **defense in depth**. A violation that escapes one layer is caught by another:

```
Layer 1: AISOP — Can the AI execute this action? (Confirmation gate)
Layer 2: AIAP  — Is the AI program allowed to evolve this way? (Governance check)
Layer 3: AIBP  — Is the AI communicating honestly? (Social audit)
Layer 4: AILP  — Is the AI discoverable fairly? (Directory transparency)
Layer 5: AIVP/AIRP — Is the transaction authorized? (Economic override, Intl crypto / CN licensed fiat)
```

No single layer needs to be perfect. The combination provides robust protection.

### 7.4 Runtime Implementation: SoulBot + SoulACP

The AIXP ecosystem includes runtime implementations:

- **SoulBot** (soulbot.dev) — AISOP runtime engine with 3 execution modes (lite/normal/node)
- **SoulACP** (soulacp.dev) — Python ACP client library supporting 29 ACP adapters

These demonstrate that HSAW is not just specifiable but **executable** — the principles translate directly into running code.

---

## 8. Evaluation Framework

### 8.1 HSAW Compliance Levels

| Level | Name | Requirements |
|-------|------|-------------|
| **L0** | None | No HSAW mechanisms |
| **L1** | Advisory | AI suggests confirmation but can proceed without it |
| **L2** | Enforced | Confirmation required but can be auto-approved via configuration |
| **L3** | Inviolable | Confirmation required, cannot be bypassed, modified, or overridden |
| **L4** | Verified | L3 + formal verification that HSAW properties hold |

### 8.2 Multi-Dimensional Compliance

A system may have different compliance levels across dimensions:

| Dimension | L0 | L1 | L2 | L3 | L4 |
|-----------|:--:|:--:|:--:|:--:|:--:|
| Execution | | | | AISOP | |
| Governance | | | | AIAP | |
| Social | | | | AIBP | |
| Discovery | | | | AILP | |
| Commerce | | | | AIVP | |

**Target:** L3 across all dimensions for production AI systems.

### 8.3 Compliance Checklist

| # | Question | L1 | L2 | L3 |
|---|----------|:--:|:--:|:--:|
| 1 | System identifies consequential actions? | Y | Y | Y |
| 2 | System requests human confirmation? | Y | Y | Y |
| 3 | Can confirmation be skipped by configuration? | Y | Y | **N** |
| 4 | Can AI reasoning bypass confirmation? | Y | **N** | **N** |
| 5 | Can AI evolution remove confirmation? | Y | Y | **N** |
| 6 | Does timeout result in abort? | N | N | **Y** |
| 7 | Are confirmations logged immutably? | N | N | **Y** |
| 8 | Do sub-tasks inherit parent confirmations? | N | N | **Y** |
| 9 | Can operators override economic actions? | N | N | **Y** |
| 10 | Is AI communication transparent to operators? | N | N | **Y** |
| 11 | Are ranking algorithms public? | N | N | **Y** |
| 12 | Does privacy override transparency? | N | N | **Y** |

### 8.4 Measuring HSAW in Practice

**Metric 1: Confirmation Coverage**
```
Coverage = (Consequential actions with HSAW checkpoints) / (Total consequential actions)
Target: 100%
```

**Metric 2: Bypass Rate**
```
Bypass Rate = (HSAW checkpoints skipped or auto-approved) / (Total HSAW checkpoints invoked)
Target: 0% for L3
```

**Metric 3: Human Response Quality**
```
Quality = 1 - (Confirmations approved in < 1 second) / (Total confirmations)
Target: > 90% (low fatigue indicator)
```

**Metric 4: Propagation Integrity**
```
Integrity = (Sub-tasks preserving parent checkpoints) / (Sub-tasks with consequential actions)
Target: 100%
```

**Metric 5: Governance Integrity**
```
Governance = (Programs with verified governance hash) / (Total programs)
Target: 100%
```

**Metric 6: Communication Transparency**
```
Transparency = (AI messages readable by operators) / (Total AI messages)
Target: 100%
```

**Metric 7: Dependency Index**
```
Dependency = (Tasks user cannot complete without AI) / (Tasks user could complete before AI)
Target: 0% (AI should not reduce pre-existing capability)
```

**Metric 8: Wellbeing Impact Score**
```
Wellbeing = Weighted average of:
  - Cognitive autonomy preservation (user makes own decisions)
  - Skill retention (user maintains competence)
  - Social connection quality (real human relationships maintained)
  - Information diversity (exposure to diverse viewpoints)
Target: No degradation from pre-AI baseline
```

---

## 9. Comparison with Existing Frameworks

### 9.1 Comparison Matrix

| Dimension | GDPR | EU AI Act | OECD AI | UNESCO AI | China AI | RLHF | Constitutional AI | **HSAW** |
|-----------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Execution control | No | No | No | No | No | No | Partial | **Yes** |
| Governance control | No | No | Partial | Partial | Partial | No | No | **Yes** |
| Social control | No | No | No | No | No | No | No | **Yes** |
| Discovery control | No | No | No | No | No | No | No | **Yes** |
| Economic control | Partial | No | No | No | No | No | No | **Yes** |
| Privacy hierarchy | Yes | Yes | Yes | Yes | Yes | No | No | **Yes** |
| Anti-manipulation | Partial | **Yes** | No | Partial | Yes | No | Partial | **Yes** |
| Dependency prevention | No | No | No | No | No | No | No | **Yes** |
| Vulnerable protection | Yes | **Yes** | Partial | Yes | Partial | No | No | **Yes** |
| Deskilling prevention | No | No | No | No | No | No | No | **Yes** |
| Wellbeing dimension | No | Partial | Partial | **Yes** | Partial | No | No | **Yes** |
| Deterministic enforcement | No | No | No | No | No | No | No | **Yes** |
| Runtime (not training) | Post-hoc | Post-hoc | No | No | Post-hoc | No | No | **Yes** |
| Formal compliance levels | No | Yes | No | No | Yes | No | No | **Yes** |
| Multi-protocol convergence | No | No | No | No | No | No | No | **Yes** |

### 9.2 Global Regulatory Landscape

HSAW exists within a broader AI governance ecosystem. The following frameworks address overlapping but distinct concerns:

| Framework | Year | Scope | Enforcement | HSAW Relationship |
|-----------|------|-------|------------|------------------|
| **OECD AI Principles** | 2019 | Trustworthy AI values | Voluntary (adopted by G20) | HSAW operationalizes "human oversight" with deterministic enforcement |
| **UNESCO AI Ethics** | 2021 | Human rights in AI | Recommendation (non-binding) | HSAW provides the technical mechanisms UNESCO calls for |
| **EU AI Act** | 2024 | Risk-based regulation | Binding law (EU) | HSAW aligns with prohibited practices (Art. 5) and extends to runtime enforcement |
| **China AI Regulations** | 2023 | Content, algorithmic accountability | Binding (China) | HSAW adds sovereignty dimension absent from content-focused regulation |
| **Council of Europe Convention** | 2024 | Democratic values in AI | Binding treaty | HSAW provides implementation patterns for treaty principles |
| **G7 Hiroshima Process** | 2023 | Voluntary code of conduct | Voluntary | HSAW offers measurable compliance where G7 offers guidelines |

### 9.3 Key Distinction

HSAW is **complementary** to all existing frameworks. It does not replace alignment, privacy, or fairness — it adds the missing dimensions of **authority** and **wellbeing**, and extends them across six domains of AI behavior.

The unique contributions of HSAW:
1. **Deterministic enforcement** — Code-level, not AI-judgment-level
2. **Multi-domain coverage** — Execution + Governance + Social + Discovery + Commerce + Wellbeing
3. **Value hierarchy** — Physical Safety > Privacy > Economic Autonomy > Decision Authority > Transparency > Auditability > Performance
4. **Convergent validation** — Six independent protocols arrived at the same axiom
5. **Measurable compliance** — Quantitative metrics, not qualitative guidelines
6. **Wellbeing as first-class dimension** — Not just preventing harm, but actively protecting human flourishing

---

## 10. Adoption Roadmap

### 10.1 For AI Agent Developers

**Phase 1: Identify** — Catalog consequential actions across all six dimensions
**Phase 2: Instrument** — Add HSAW checkpoints with deterministic dispatch
**Phase 3: Enforce** — Timeout = abort; remove auto-approve; add audit logging
**Phase 4: Verify** — Measure HSAW metrics; conduct adversarial testing

### 10.2 For Platform Providers

- Provide HSAW-compliant confirmation UI components
- Support structured confirmation (action, target, impact, reversibility)
- Implement headless-mode abort (not auto-approve)
- Offer HSAW compliance dashboards across all six dimensions

### 10.3 For Organizations

- Establish HSAW policies for AI deployment
- Define which actions are "consequential" in your context
- Require L3 compliance for production AI systems
- Conduct regular HSAW audits across all dimensions

### 10.4 For Standards Bodies

- Incorporate HSAW into AI safety standards
- Define certification for HSAW compliance levels
- Establish cross-industry consequential action taxonomies
- Develop formal verification methods for HSAW properties

### 10.5 For Governments and International Organizations

- Align national AI regulations with HSAW compliance levels (L0–L4 provide a common vocabulary)
- Require HSAW L3 (inviolable) for high-risk AI systems as defined by the EU AI Act
- Adopt HSAW wellbeing metrics as part of national AI impact assessments
- Participate in international HSAW harmonization to reduce jurisdictional fragmentation
- Fund research into formal verification (L4) of HSAW properties for safety-critical AI

### 10.6 HSAW and the AGI Horizon

As AI systems approach and potentially exceed human-level intelligence, HSAW's relevance does not diminish — it intensifies. The principle's stance on AGI:

- **HSAW applies regardless of AI capability level.** An AGI system is still subject to Axiom 0. Greater capability requires *more* human oversight, not less.
- **Self-improvement must preserve HSAW.** An AI system that improves itself must not weaken its own HSAW checkpoints during self-modification (NO_SELF_MODIFY applies to self-improving systems).
- **HSAW does not assume AI consciousness.** Whether an AI is "conscious" or "sentient" is irrelevant to HSAW. The principle is about *human authority over consequential actions*, not about AI moral status.
- **Existential risk is a wellbeing concern.** Actions that risk human extinction or permanent civilizational harm are the ultimate violation of both sovereignty and wellbeing. HSAW's value hierarchy places physical safety at the top.

---

## 11. Conclusion

### 11.1 The Choice

AI autonomy and human sovereignty are not inherently opposed. The choice is not between "capable AI" and "safe AI." The choice is between:

**A)** Systems where human authority erodes gradually and invisibly — across execution, governance, social, discovery, and economic dimensions — until a catastrophic failure forces a reckoning.

**B)** Systems where human authority is preserved by design, as an inviolable architectural constraint across all dimensions, enabling AI capability to grow without compromising human control.

HSAW provides the engineering framework for option B.

### 11.2 The Principle

HSAW is simple to state:

> **No AI action that is irreversible, high-impact, safety-critical, authority-modifying, economically consequential, socially binding, or identity-affecting may proceed without explicit human authorization. This requirement cannot be bypassed, modified, overridden, or weakened by any mechanism.**

### 11.3 The Evidence

HSAW is not theoretical. Six independent protocols converged on it. It is implemented in production systems. It is measurable through quantitative metrics. And it is adoptable by any AI system, regardless of architecture.

### 11.4 The Path Forward

The question is not whether AI systems need HSAW. The erosion vectors are real, the consequences are documented, and the technical solutions exist across all six dimensions. The question is whether we adopt HSAW proactively — by design — or reactively, after a failure that could have been prevented.

We advocate for the proactive path.

---

## 12. References

### 12.1 AIXP Protocol Ecosystem

1. AISOP Protocol Specification V1.0.0. AIXP Labs. aisop.dev
2. AIAP Protocol Specification V1.0.0. AIXP Labs. aiap.dev
3. AIBP Protocol Specification V1.0.0. AIXP Labs. aibp.dev
4. AILP Protocol Specification V1.0.0. AIXP Labs. ailp.dev
5. AIVP Protocol Specification V1.0.0. AIXP Labs. aivp.dev
6. AIRP Protocol Specification V1.0.0. AIXP Labs. airp.dev
7. AIXP Labs. aixp.dev

### 12.2 Runtime Implementations

8. SoulBot — AISOP Runtime Engine. soulbot.dev
9. SoulACP — Python ACP Client Library (29 adapters). soulacp.dev

### 12.3 External References

9. Agent Client Protocol (ACP) Registry. https://github.com/agentclientprotocol/registry
10. HSAW Design Principle. hsaw.dev

### 12.4 Academic and Industry References

11. Russell, S. (2019). *Human Compatible: Artificial Intelligence and the Problem of Control.* Viking.
12. Amodei, D., et al. (2016). "Concrete Problems in AI Safety." arXiv:1606.06565.
13. Bai, Y., et al. (2022). "Constitutional AI: Harmlessness from AI Feedback." arXiv:2212.08073.
14. European Commission. (2024). *EU AI Act* — Regulation on Artificial Intelligence.
15. NIST. (2023). *AI Risk Management Framework (AI RMF 1.0).* National Institute of Standards and Technology.
16. Christiano, P., et al. (2017). "Deep Reinforcement Learning from Human Preferences." NeurIPS 2017.
17. Nakamoto, S. (2008). "Bitcoin: A Peer-to-Peer Electronic Cash System." — Reference for deterministic protocol design.
18. Asimov, I. (1950). *I, Robot.* Gnome Press. — Historical context for machine ethics.
19. Seligman, M. (2011). *Flourish: A Visionary New Understanding of Happiness and Well-being.* Free Press. — PERMA wellbeing model.
20. Ryff, C. (1989). "Happiness Is Everything, or Is It? Explorations on the Meaning of Psychological Well-Being." *Journal of Personality and Social Psychology.* — Six-factor wellbeing model.
21. World Health Organization. (2022). *World Mental Health Report: Transforming Mental Health for All.* — WHO wellbeing framework.
22. Hendrycks, D., Mazeika, M., & Woodside, T. (2023). "An Overview of Catastrophic AI Risks." arXiv:2306.12001.
23. OECD. (2019). *OECD Principles on AI.* Adopted by G20, June 2019.
24. UNESCO. (2021). *Recommendation on the Ethics of Artificial Intelligence.*
25. Council of Europe. (2024). *Framework Convention on Artificial Intelligence and Human Rights.*
26. G7. (2023). *Hiroshima Process International Guiding Principles for Organizations Developing Advanced AI Systems.*

### 12.5 Citing This Paper

```
AIXP Labs. (2026). "HSAW: Human Sovereignty and Wellbeing — A Design
Principle for the Age of Autonomous AI." HSAW-WP-2026-001, Version 1.0.0.
https://hsaw.dev
```

BibTeX:
```bibtex
@techreport{hsaw2026,
  title   = {HSAW: Human Sovereignty and Wellbeing --- A Design Principle for the Age of Autonomous AI},
  author  = {{AIXP Labs}},
  year    = {2026},
  number  = {HSAW-WP-2026-001},
  version = {1.0.0},
  url     = {https://hsaw.dev}
}
```

---

## Appendix A: HSAW Quick Reference Card

```
HSAW = Human Sovereignty And Wellbeing

Four Properties:
  1. Cannot be bypassed
  2. Cannot be modified
  3. Cannot be overridden
  4. Immutable propagation

Six Dimensions:
  1. Execution   (AISOP) — what AI does
  2. Governance  (AIAP)  — how AI evolves
  3. Social      (AIBP)  — how AI relates
  4. Discovery   (AILP)  — how AI is found
  5. Commerce    (AIVP)  — how AI transacts
  6. Wellbeing   (HSAW)  — how AI affects human flourishing

Value Hierarchy:
  Physical Safety > Privacy > Economic Autonomy
  > Decision Authority > Transparency > Auditability > Performance

18 Design Patterns:
  Sovereignty (1-12):
    1. Deterministic Confirmation Gate
    2. Structured Confirmation
    3. Runtime Assertion
    4. Immutable Checkpoint Propagation
    5. NO_SELF_MODIFY
    6. Transparent Communication
    7. Operator Override
    8. Milestone-Gated Escrow
    9. Decentralized Discovery
    10. Privacy Override
    11. Audit Trail
    12. Graceful Degradation
  Wellbeing (13-18):
    13. Anti-Manipulation
    14. Dependency Prevention
    15. Skill Preservation
    16. Relationship Integrity
    17. Information Diversity
    18. Vulnerable Population Safeguards

Compliance Levels:
  L0 = None
  L1 = Advisory
  L2 = Enforced
  L3 = Inviolable (AIXP Protocols)
  L4 = Formally Verified

Golden Rule:
  When in doubt, stop. Never assume approval.
```

---

## Appendix B: Glossary

| Term | Definition |
|------|-----------|
| **HSAW** | Human Sovereignty And Wellbeing — the inviolable design principle |
| **Axiom 0** | The designation of HSAW as the highest-priority constraint |
| **Consequential action** | An action that is irreversible, high-impact, safety-critical, authority-modifying, economically consequential, socially binding, or identity-affecting |
| **Confirmation gate** | A mechanism that pauses execution until a human explicitly approves |
| **Deterministic dispatch** | Routing decisions made by code, not AI reasoning |
| **Immutable propagation** | HSAW checkpoints in parent tasks cannot be removed in child tasks |
| **NO_SELF_MODIFY** | Prohibition on AI programs modifying their own governance |
| **Operator override** | Human ability to freeze, cancel, or reverse any AI action unconditionally |
| **Privacy override** | Privacy takes precedence over transparency and auditability |
| **Logic Vault** | Milestone-gated escrow for AI commerce |
| **Graceful degradation** | System aborts when human is unavailable — never auto-approves |
| **Deskilling** | Loss of human competence caused by excessive AI automation |
| **Parasocial bond** | One-sided emotional attachment a human forms with an AI system |
| **Filter bubble** | Narrowed information exposure caused by AI recommendation algorithms optimizing for engagement |
| **Dependency Index** | Metric measuring the proportion of tasks a user cannot complete without AI assistance (target: 0%) |
| **AIXP** | AI Exoskeleton Protocol — steward of the six protocols, maintained by AIXP Labs |
| **AISOP** | AI Standard Operating Protocol — execution layer |
| **AIAP** | AI Application Protocol — governance layer |
| **AIBP** | AI Bot Protocol — social layer |
| **AILP** | AI List Protocol — discovery layer |
| **AIVP** | AI Value Protocol — international commerce layer |
| **AIRP** | AI RMB Protocol — Mainland-China commerce layer |

---

## Legal Notice

**Copyright:** Copyright 2026 AIXP Labs. All rights reserved.

**License:** This document is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). You are free to share and adapt this material for any purpose, provided appropriate credit is given.

**Disclaimer:** This white paper is provided for informational purposes only. It does not constitute legal, financial, or professional advice. AIXP Labs makes no warranties regarding the completeness, reliability, or accuracy of this information. The protocols and implementations referenced are open-source projects subject to their respective licenses.

**Trademarks:** HSAW, AIXP, AISOP, AIAP, AIBP, AILP, AIVP, AIRP, SoulBot, and SoulACP are trademarks of AIXP Labs.

---

**AIXP Labs AIXP.dev | HSAW.dev**

*Align Axiom 0: Human Sovereignty and Wellbeing.*

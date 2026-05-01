# Inference Governance Module (IGM)
### Live Demonstration · DeBacco Nexus LLC

[![Live Demo](https://img.shields.io/badge/Live%20Demo-igm--demo.onrender.com-00e5a0?style=for-the-badge)](https://igm-demo.onrender.com)
[![Patent Pending](https://img.shields.io/badge/Patent%20Pending-USPTO%2019%2F571%2C156-4d9fff?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-Proprietary-ff4d6a?style=for-the-badge)]()

---

## What Is the IGM?

The **Inference Governance Module (IGM)** is a constraint-first AI governance architecture that sits at the inference boundary — between the user request and the large language model — enforcing hard token output ceilings, input validation, PII detection, and structured output classification at the API layer.

The IGM does not ask the model to behave. It mechanically enforces governance before inference occurs.

> *"Everyone's writing AI policies. Few are building governance that survives the first deployment."*
> — Harvard Data Science Initiative

The IGM is the architecture that survives the first deployment.

---

## The Core Problem

Current AI governance operates at the prompt layer — system instructions that request compliant behavior from a language model. This is **performative governance**: the model is asked to comply, but nothing mechanically enforces it.

This creates four compounding failures:

| Failure | Impact |
|---|---|
| **The Translucent Guardrail Problem** | Prompt-level governance is a request, not a constraint. Models can and do exceed it. |
| **The Knowability Gap** | Without an inference boundary, output cannot be known or bounded before it is produced. |
| **Token waste at scale** | Ungoverned inference produces verbose output by default, burning tokens, energy, water, and capital with every call. |
| **Token ceiling inequity** | Users on paid subscriptions hit monthly limits not because they needed those tokens — but because ungoverned inference wasted them. |

---

## The IGM Solution

The IGM enforces governance **mechanically** at the infrastructure layer — not performatively at the prompt layer.

```
User Request
     │
     ▼
┌─────────────────────────────┐
│   INFERENCE GOVERNANCE      │
│         MODULE              │
│                             │
│  ① Input validation         │
│  ② PII scanner              │
│  ③ Token ceiling enforcer   │
│  ④ Output classifier        │
└─────────────┬───────────────┘
              │ Authorized
              ▼
     Large Language Model
              │
              ▼
     Governed Response
     (Precise · Bounded · Auditable)
```

Without IGM, the request goes directly to the LLM with no constraints enforced — producing verbose, unstructured, unauditable output.

---

## Live Demonstration

**[https://igm-demo.onrender.com](https://igm-demo.onrender.com)**

The demonstration runs real-time API calls — governed vs. ungoverned — simultaneously, across ten real-world scenarios. Watch the governance decision log populate line by line before the LLM responds. See real token counts, real differential, real cumulative environmental and capital savings.

### Scenarios

| # | Domain | Situation |
|---|---|---|
| 01 | Thermodynamics | Thermal safety engineer — PWR reactor 8°C from critical failure |
| 02 | Robotics | Surgical robot arm — LLM-to-actuator inference boundary |
| 03 | Nanotech | Carbon nanotube QC — 40,000 ungoverned calls/day, millions in waste |
| 04 | Thermodynamics + Nanotech | 200-node nanorobotic array — thermal boundary analysis |
| 05 | Robotics | Emergency — autonomous arm detects human in work envelope |
| 06 | Cloud Security | AWS Bedrock — Fortune 500 CISO, $340K/year ungoverned inference |
| 07 | Cybersecurity | Margin collapse — AWS inference costs exceeding product revenue |
| 08 | Access Equity | Token ceiling crisis — paid subscribers locked out by waste |
| 09 | Custom | Enter your own real-world situation — IGM governs it live |
| 10 | Engineering | Offshore wind turbine — structural alert fatigue, 340 alerts/day |

---

## The DeBacco Rule

Governed AI inference produces responses within approximately **1 joule** regardless of language, modality, or model architecture.

This is the first thermodynamic constant applied to AI inference governance. It provides a unit of measurement that no existing AI policy framework has — making IGM the only governance architecture with a measurable, falsifiable, energy-based boundary condition.

---

## Key Research Findings

**The Translucent Guardrail Problem**
Empirical testing across six AI platforms demonstrated that prompt-level JSON governance is performative rather than mechanical. Infrastructure-level constraints enforced via API parameters work mechanically. This distinction is the foundation of the IGM.

**The Principle of Tiers**
A structured framework for scaling governance:
- **Tier 1** — Token reduction (English, Arabic, 23 DHCS languages)
- **Tier 2** — Modality governance
- **Tier 3** — Environmental impact projection
- **Tier 4** — AI-to-AI separation architecture

**Thermodynamic Nanorobotic Infrastructure (TNI)**
The IGM governance boundary applies uniformly across cloud and local offline deployments. Thermal stress field visualizations document the energy differential between governed and ungoverned inference paths.

---

## Real-World Applications

- **Healthcare** — Clinical AI delivering precise instructions without PII exposure
- **Robotics** — Inference-to-actuator governance preventing unsafe motor commands
- **Cloud Security** — Structured audit trails replacing verbose unaccountable output
- **Enterprise AI** — Token budget governance restoring profitability on inference-heavy products
- **Public Infrastructure** — Emergency dispatch AI with zero-verbosity, millisecond decisions
- **Access Equity** — Preserving monthly token budgets for individuals and small businesses

---

## Patent

**USPTO Application 19/571,156** — Patent pending  
Inference Governance Module (IGM)  
DeBacco Nexus LLC  

The full IGM architecture is protected under this application. This repository demonstrates the governance boundary concept only. The implementation architecture is not disclosed.

---

## About

**James DeBacco**  
Founder & CEO, DeBacco Nexus LLC  
Member, CalCompute Consortium  
Veterans Treatment Court Liaison, Los Angeles County  
Executive Director, Bridges2Freedom 501(c)(3)  
DSW Candidate, USC Suzanne Dworak-Peck School of Social Work  

The IGM originated from the Transformational Accountability and Ethics (TAE) methodology developed over 15+ years working with justice-involved and veteran populations — and the recognition that the same governance principles that protect human behavior in high-stakes institutional settings apply directly to AI inference at the infrastructure layer.

---

## Contact

## Ambient Ungoverned Inference Drain (AUID)

**AUID** is the hidden CPU load draining battery, energy, and tokens without consent.

**Definition:** The continuous execution of AI inference on user devices through browser-embedded or application-embedded engines, operating without token ceilings, energy measurement, user consent, or audit trails — resulting in measurable CPU load, battery drain, and thermal impact on users who never authorized it.

*Introduced by DeBacco, J. (2026). Submitted to Springer Nature AI and Ethics. USPTO 19/571,156.*

---

### AUID Does Not Wait for You

The most significant finding: **AUID starts the moment your device wakes up — before you open a single application.**

A live Activity Monitor capture taken immediately upon device wake on May 1, 2026 showed:

| Process | CPU % | Classification |
|---|---|---|
| spotlight | 48.1% | Apple ML indexing — fires on wake |
| duetexpertd | 29.4% | Apple Intelligence coordinator |
| suggestd | 19.0% | Apple suggestion inference daemon |
| Google Chrome | 10.5% | Chrome AI features activating |
| Microsoft | 8.6% | Microsoft AI activating on wake |
| corespeechd | 4.0% | CoreSpeech inference daemon |
| Grammarly | 2.2% | Continuous ML inference |

**Combined CPU at wake: 20.61% — before any user action.**

---

### Seven Documented AUID Examples

**1 — Mozilla Firefox 141 (August 2025)**
Background "Inference" process for AI tab grouping ran by default. CPU spikes to 130%. Battery drain. Fans at maximum. Killing the process crashed the browser. Mozilla reversed the rollout only after user complaints — post-hoc governance, not governance by design.

**2 — Google Chrome: Gemini Nano**
Chrome automatically downloads and runs Gemini Nano locally during updates. Executes inference for summarization, writing assistance, and smart replies. No token ceiling. No energy measurement. No consent required.

**3 — Microsoft Copilot + Edge WebView2**
Runs in background on Windows 11, consuming 250–500MB of memory while idle, causing CPU spikes when not in use. Disabling Copilot immediately reclaims approximately 200MB of system memory.

**4 — Microsoft Windows Recall + Phi Silica**
Continuously analyzes all user activity using a local AI model on the device NPU — default-on. Made opt-in only after user backlash.

**5 — Browser Extensions with Persistent Background Inference**
Extensions using Transformers.js and WebLLM load multi-gigabyte AI models as persistent service workers across all tabs — by design, because reloading them repeatedly is impractical.

**6 — Grammarly Desktop**
Runs continuous local ML inference across every application on your device — word processors, email, browsers — without any user-initiated request. No token ceiling. No energy record.

**7 — Apple Intelligence: generativeexperiencesd, textunderstandingd, siriinferenced**
Three persistent Apple Intelligence daemons run continuously on macOS and iOS. All execute background inference without token ceilings, energy measurement, or per-session consent. Visible in Activity Monitor across multiple captures.

---

### What Every AUID Example Has in Common

- **No token ceiling** — no limit on computational resources per inference event
- **No energy measurement** — no record of joules consumed on your device
- **No consent** — default-on, requiring users to actively disable
- **No audit trail** — no verifiable record of what ran, when, or what it consumed

This is not a single vendor problem. It is a systemic absence of governance at the browser and device inference boundary — across every major browser, on every major operating system, on hundreds of millions of devices simultaneously.

---

### The IGM Addresses All Four AUID Failures

| AUID Failure | IGM Module |
|---|---|
| No consent boundary | Input Processing — authenticated authorization required |
| No token ceiling | GATE — hard ceiling enforced before inference |
| No energy measurement | TTP Monitor — joule measurement per inference |
| No clean termination | Pipeline architecture — discrete modules, clean boundaries |

**The DeBacco Rule** — governed inference within ~1 joule — provides the reference energy boundary that AUID currently has no equivalent of.

*DeBacco, J. (2026). Ambient Ungoverned Inference Drain (AUID): Naming and Addressing the Hidden CPU Load on User Devices and the Case for Constraint-First Architecture. Submitted to AI and Ethics, Springer Nature. USPTO Provisional Application 19/571,156.*

**DeBacco Nexus LLC**  
info@debacconexus.com  
[https://igm-demo.onrender.com](https://igm-demo.onrender.com)

---

*This demonstration is built on the Claude API by Anthropic. The IGM architecture, governance boundary concept, DeBacco Rule, Principle of Tiers, and Translucent Guardrail Problem are original works of James DeBacco / DeBacco Nexus LLC, protected under USPTO 19/571,156.*

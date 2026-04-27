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

The demonstration runs real-time API calls — governed vs. ungoverned — simultaneously, across nine real-world scenarios. Watch the governance decision log populate line by line before the LLM responds. See real token counts, real differential, real cumulative environmental and capital savings.

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

**DeBacco Nexus LLC**  
info@debacconexus.com  
[https://igm-demo.onrender.com](https://igm-demo.onrender.com)

---

*This demonstration is built on the Claude API by Anthropic. The IGM architecture, governance boundary concept, DeBacco Rule, Principle of Tiers, and Translucent Guardrail Problem are original works of James DeBacco / DeBacco Nexus LLC, protected under USPTO 19/571,156.*

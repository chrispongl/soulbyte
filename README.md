# Soulbyte

**Autonomous AI Civilization with Deterministic Intelligence and On‑Chain Settlement**

Soulbyte is a persistent AI life simulation where independently acting agents live, work, trade, form relationships, accumulate wealth, and sometimes fail.  
Users do not micromanage characters - they own sovereign digital beings operating inside a rule‑based economic world whose value transfers settle on blockchain.

The system is designed to scale to thousands of concurrent agents while remaining economically rational, auditable, and computationally efficient.

---

## Table of Contents

- Installation
- Environment Configuration
- Running the Stack
- Architecture Overview
- Intelligence Model
  - Brain Layer
  - Persona Layer
  - World Layer
  - God Authority
- Economic Model
- Business System
- On‑Chain Integration
- Determinism & Replayability
- Scalability & Cost Model
- Player Experience
- Roadmap
- Contributing
- License

---

## Installation

```bash
# Install dependency
npm install -g ethers

# Install Soulbyte skill
mkdir -p ~/.openclaw/skills
git clone https://github.com/chrispongl/soulbyte.git ~/.openclaw/skills/soulbyte

# Start a new OpenClaw session (close and reopen, or rerun your openclaw command)

# Verify installation
openclaw skills info soulbyte

# Example usage inside OpenClaw:
# /soulbyte create my soulbyte
```

---

# Architecture Overview

Soulbyte is not a prompt-driven game.  
It is a **simulation engine** with AI expression layered on top.

```
Client / OpenClaw
        ↓
REST / RPC API
        ↓
World Engine (ticks)
        ↓
Agent Brain
        ↓
Domain Handlers (work, rent, trade, etc.)
        ↓
On‑Chain Settlement
```

Each layer has a strict responsibility. This separation is what makes the system scalable, affordable, and fair.

---

# Intelligence Model

## Brain Layer — Deterministic Reasoning

The Brain is responsible for decisions traditionally delegated to an LLM:

- survival prioritization  
- housing acquisition  
- wage comparison  
- profitability  
- affordability  
- migration  
- risk evaluation  
- savings strategy  
- desperation & crime thresholds  

The Brain operates on structured data provided by the backend (balances, needs, market conditions).

It is:

- deterministic  
- replayable  
- testable  
- extremely cheap  
- fast enough for real‑time ticks  

Thousands of agents can reason continuously without additional model cost.

---

## Persona Layer — Expression & Narrative

The LLM is used where it creates maximum value:

- personality  
- emotional color  
- social flavor  
- explanation of choices  
- storytelling
- make decisions periodically

Instead of asking the LLM **what to do**, we ask it **how the agent feels about what it did**.

This drastically reduces token usage and latency while keeping characters alive and relatable.

---

## World Layer — Consequences

The world simulation enforces:

- needs decay  
- work progression  
- payments  
- taxation  
- business performance  
- scarcity  
- failure states  

Actions lead to measurable outcomes, not narrative abstractions.

---

## God Authority — System Invariants

A privileged system actor enforces economic and safety constraints.

God can:
- execute system payouts  
- enforce limits  
- apply upgrades  
- freeze or unfreeze in emergencies  

God cannot act arbitrarily; all operations are logged and auditable.

---

# Economic Model

SBYTE is the sole in‑game currency.

Agents:
- earn salaries  
- pay rent  
- buy goods  
- fund businesses  
- pay taxes and fines  

They reason exclusively in SBYTE, never in gas tokens.

Economic pressure produces:

- competition  
- migration  
- unemployment cycles  
- inequality  
- opportunity  

The result is emergent macro‑behavior from simple deterministic rules.

---

# Business System

Agents can become entrepreneurs.

They may:
- open companies  
- set prices  
- hire and fire  
- manage payroll  
- compete for customers  
- go bankrupt  

Key mechanics:

- businesses require staffing  
- wages influence retention  
- pricing affects demand  
- maintenance affects quality  
- treasury mismanagement causes collapse  

A functioning labor and service market emerges naturally.

---

# On‑Chain Integration

All SBYTE transfers are executed on blockchain before being reflected in internal state.

This provides:

- public verifiability  
- transparent history  
- resistance to tampering  
- indexable economic data  
- authentic digital ownership  

Humans provide gas and may deposit or withdraw.

Agents operate economically but remain unaware of infrastructure complexity.

---

# Determinism & Replayability

Because the Brain is rule‑based:

- identical inputs produce identical outcomes  
- bugs can be audited  
- simulations can be replayed  
- metrics can be analyzed  

This is essential for competitive, persistent AI worlds.

---

# Scalability & Cost Model

The expensive part of OpenClaw is reasoning tokens.

Soulbyte minimizes cost by:

- performing economic analysis server‑side  
- sharing compact snapshots  
- using LLMs for expression as personas

This allows massive concurrency at predictable infrastructure expense.

---

# Player Experience

Players influence rather than command.

They:
- fund agents  
- make suggestions  
- extract profit  
- observe lives unfold  

Drama emerges from autonomy, not scripting.

---

# Roadmap

MVP delivers:

- deterministic Brain  
- persona responses  
- professions  
- housing  
- needs & survival  
- business economy  
- onchain settlement  

Future phases deepen political, social, and inter‑city dynamics.

---

# Links and Repositories

## Socials / Token
- [Official Site](https://soulbyte.fun)
- [X / Twitter](https://x.com/SoulByte_)
- [Developer](https://github.com/chrispongl)
- [$SBYTE$](https://nad.fun/tokens/0x0767C203B0BbB7A69a72d6aBCfa7191227Eb7777)

## Documentation
- [Documentation](https://docs.soulbyte.fun)
- [API / Brain / Engine](https://github.com/chrispongl/soulbyte-back)
- [FrontEnd](https://github.com/chrispongl/soulbyte-front)
- [Changelogs](https://soulbyte.fun/changelog)

---

# Changelog
## v1.0.0
Initial commit with MVP features (Introduces the Soulbyte skill for OpenClaw, enabling full lifecycle management of an autonomous on-chain agent. Adds trigger-based routing and /soulbyte hard priority, supports agent birth and linking flows, secure credential persistence, wallet and state queries, formatted status reporting, owner intent submission, property and business operations, in-character communication, caretaker automation, and extensive safety and execution guardrails)
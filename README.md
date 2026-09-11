# SignalForge — Product Intelligence OS

> **Turn messy customer feedback into an evidence-backed product roadmap.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open%20SignalForge-69e0c2?style=for-the-badge)](https://signalforge-52lf.onrender.com)

SignalForge is a portfolio-grade product management case study built by an AI/ML student to demonstrate **PM thinking, product strategy, analytics, prioritization, experimentation, and technical fluency**.

## The product loop

**Feedback → Evidence → Opportunities → Prioritization → Roadmap → PRD → Experiment → Decision log**

The prototype is intentionally transparent: instead of hiding a recommendation behind a black-box AI score, it exposes the assumptions a PM can challenge.

## Why it exists

Real product teams receive feedback from support tickets, app reviews, interviews, sales calls, and community posts. The hard part is not collecting feedback — it is turning noisy anecdotes into a decision the team can defend.

SignalForge addresses four common failure modes:

- **Loud-user bias:** the most recent request wins.
- **Feature framing:** teams prioritize requested solutions instead of underlying problems.
- **False precision:** a single score hides its assumptions.
- **Decision amnesia:** teams forget why a roadmap choice was made.

## What you can do

### 1. Decision cockpit
See evidence coverage, decision velocity, opportunity health, and the current recommendation at a glance.

### 2. Signal intelligence
Inspect customer problem clusters and drill into their source, volume, severity, confidence, and evidence tags. Add a new signal directly in the interface.

### 3. Transparent prioritization
Use opportunity scoring and RICE-style reasoning. The assumptions are visible so reviewers can disagree with the model rather than blindly trusting it.

### 4. Interactive roadmap
Move opportunities between **Now / Next / Later** to simulate a prioritization conversation and make tradeoffs visible.

### 5. PRD + experiment
Translate the selected problem into a concise PRD brief, primary metric, guardrails, instrumentation plan, and success criteria.

### 6. Decision log
Preserve the reasoning behind roadmap choices: evidence, framework, confidence, and status.

## Product thesis

> **If PMs can move from anecdotal feedback to a transparent prioritization decision in minutes, roadmap conversations become less opinion-driven and more evidence-driven.**

### North-star metric
**% of roadmap decisions linked to ≥3 independent evidence items.**

Initial product targets:

| Metric | Target |
|---|---:|
| Evidence-linked decisions | 70%+ |
| Raw feedback → ranked opportunity | <10 min |
| Reviewer agreement with ranking | 80%+ |

## PM decisions demonstrated

**Transparency over black-box automation** — the score is explainable.

**Problems over feature requests** — customer language is synthesized into underlying friction.

**Metrics before shipping** — every meaningful roadmap bet gets a measurable hypothesis and guardrails.

**Quality of decision over breadth of integrations** — v1 avoids Jira/Linear/auth complexity until the core workflow proves useful.

## Technical approach

- Vanilla HTML / CSS / JavaScript
- No build step
- Responsive SaaS-style interface
- Client-side interactive state for the portfolio prototype
- Render Static Site deployment
- Synthetic, traceable sample data

The intelligence layer is intentionally lightweight and transparent. The portfolio story is about **product reasoning**, not pretending a mock interface is production AI.

## Repository structure

```text
SignalForge/
├── app/
│   └── index.html          # Interactive product prototype
├── docs/
│   ├── PRD.md              # Product requirements
│   ├── ROADMAP.md          # Prioritization and sequencing
│   ├── EXPERIMENT.md       # Validation plan
│   └── CASE_STUDY.md       # PM case study
├── render.yaml             # Deployment configuration
└── README.md
```

## Validation plan

The next validation step is a lightweight controlled usability test:

- **5–8 target users**
- **Control:** spreadsheet / notes workflow
- **Treatment:** SignalForge
- **Primary metric:** median time to a ranked top-three list
- **Guardrails:** reviewer confidence, evidence coverage, contradictory signals ignored
- **Success threshold:** ≥30% reduction in median decision time while maintaining or improving confidence

The goal is to learn whether structured evidence actually changes decision quality — not merely whether users think the interface looks good.

## Roadmap

**NOW**
- Interactive signal inbox
- Transparent opportunity scoring
- RICE reasoning
- Now / Next / Later roadmap
- Decision traceability
- PRD + experiment workflow

**NEXT**
- 5–8 user interviews
- Usability test against a spreadsheet control
- Capture actual decision time and confidence
- Tune weights from observed behavior

**LATER**
- CSV/API ingestion
- Jira / Linear integrations
- LLM-assisted synthesis with citations
- Team workspaces and permissions
- Historical outcome learning

## Live demo

**https://signalforge-52lf.onrender.com**

## Portfolio note

This project is a **PM portfolio artifact**, not a claim of production readiness. Sample metrics and feedback are synthetic and are clearly labeled so the reviewer can focus on the quality of the product decisions.

Built by **Soniya** — AI/ML student exploring product management at the intersection of user problems, data, experimentation, and technology.

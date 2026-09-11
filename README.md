# SignalForge — Product Intelligence OS

> **Turn messy user feedback into an evidence-backed product roadmap.**

SignalForge is a portfolio-grade product management case study built by an AI/ML student to demonstrate PM thinking, product strategy, analytics, experimentation, and execution.

## The decision loop

**Feedback → Themes → Opportunity Score → Prioritization → PRD → Experiment → Outcome**

## What the prototype demonstrates

- **Signal inbox** — simulated feedback from support, app reviews, interviews, sales, and community channels
- **Theme clustering** — turns repeated complaints into product opportunities
- **Opportunity scoring** — frequency + severity + strategic fit + confidence + effort
- **RICE prioritization** — Reach × Impact × Confidence ÷ Effort
- **Now / Next / Later roadmap** — explicit trade-offs instead of feature dumping
- **PRD preview** — problem, target user, hypothesis, scope, non-goals, acceptance criteria
- **Experiment design** — north-star metric, guardrails, and target outcomes
- **Decision log** — preserves why a roadmap choice was made

## PM artifacts

| Artifact | Signal to a hiring manager |
|---|---|
| `docs/PRD.md` | Product discovery, scope, user stories, acceptance criteria |
| `docs/ROADMAP.md` | Prioritization, sequencing, trade-offs |
| `docs/METRICS.md` | Metrics tree and success criteria |
| `docs/EXPERIMENT.md` | Hypothesis-driven experimentation |
| `app/` | Working interactive product prototype |

## Product thesis

> If PMs can move from anecdotal feedback to a transparent prioritization decision in minutes, roadmap conversations become less opinion-driven and more evidence-driven.

## Success metrics

**North-star:** percentage of roadmap decisions linked to customer evidence.

Initial prototype targets:
- 70%+ of decisions linked to ≥3 evidence items
- <10 minutes from raw feedback to a ranked opportunity
- 80%+ agreement between PM ranking and reviewer ranking in a usability test

## Tech

Vanilla HTML/CSS/JavaScript. No build step required. The intelligence layer is deliberately transparent/mock-data driven so the portfolio foregrounds product reasoning, UX, metrics, and trade-offs rather than pretending a black-box model is the product.

## Run 

Open `https://signalforge-52lf.onrender.com/` in a browser.

## Portfolio positioning

This repository is structured like a PM case study: **problem → evidence → decision framework → prototype → measurement plan**.

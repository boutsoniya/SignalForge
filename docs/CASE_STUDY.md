# SignalForge — PM Case Study

## 1. Context

I built SignalForge as a product-management portfolio project to explore a simple question:

> Can a PM turn noisy customer feedback into a roadmap decision that another person can understand, challenge, and measure?

The project deliberately sits at the intersection of product thinking and technical fluency. The interface is implemented with vanilla HTML/CSS/JavaScript, while the product model makes assumptions visible instead of hiding them behind a black-box AI recommendation.

## 2. Problem

Customer feedback arrives as fragmented requests: “add X”, “search is bad”, “I got stuck”, “export takes too long”. A PM can easily mistake volume for importance or a requested feature for the actual problem.

The workflow I wanted to improve was:

**Raw feedback → synthesis → prioritization → roadmap → PRD → experiment**

The key product insight was that the decision itself should remain traceable to evidence.

## 3. Product thesis

If PMs can move from anecdotal feedback to a transparent prioritization decision in minutes, roadmap conversations become less opinion-driven and more evidence-driven.

## 4. Users

**Primary:** early-career and startup PMs managing a small number of product surfaces.

**Secondary:** founders, product analysts, and engineering leads who participate in prioritization.

## 5. Product decisions

### Decision 1 — Transparency over black-box AI

A black-box “AI priority score” would look impressive but make the core decision difficult to challenge. SignalForge exposes frequency, severity, strategic fit, confidence, and effort assumptions.

**Trade-off:** less automation in v1, more trust and reviewability.

### Decision 2 — Problems over feature requests

The system groups feedback around underlying customer problems. This avoids converting every request directly into a roadmap item.

**Trade-off:** synthesis requires interpretation, but it produces a more useful product decision.

### Decision 3 — Metrics before shipping

Every major opportunity leads toward a measurable hypothesis, primary metric, guardrails, and instrumentation.

**Trade-off:** fewer “feature complete” stories, more emphasis on learning.

### Decision 4 — Decision traceability as a first-class feature

A decision log records the evidence, prioritization framework, confidence, and status behind a roadmap choice.

**Trade-off:** a little more interface complexity in exchange for organizational memory.

## 6. MVP

The prototype includes:

- Decision cockpit
- Signal inbox
- Evidence-oriented problem clusters
- Opportunity scoring
- RICE-style prioritization
- Interactive Now / Next / Later roadmap
- PRD preview
- Experiment design
- Decision log
- Add-signal workflow

## 7. Validation plan

The next step is not adding more features. It is testing the core value proposition.

### Experiment

- **Participants:** 5–8 target users
- **Control:** spreadsheet / notes workflow
- **Treatment:** SignalForge
- **Primary metric:** median time to produce a ranked top-three list
- **Guardrails:** reviewer confidence, evidence coverage, contradictory signals ignored

### Success criterion

At least **30% reduction in median decision time** while maintaining or improving decision confidence.

## 8. What I would learn

1. Do users trust a transparent score more than a black-box recommendation?
2. Which scoring inputs do users challenge most often?
3. Does RICE help clarify trade-offs or create false precision?
4. Do users inspect evidence before accepting a recommendation?
5. Does the decision log improve confidence during review?

## 9. What comes next

If the workflow validates:

1. Add CSV/API ingestion.
2. Test LLM-assisted synthesis with citations.
3. Add Jira/Linear integrations.
4. Introduce team workspaces and permissions.
5. Learn from historical roadmap outcomes.

The sequencing is intentional: **validate the decision workflow before investing in automation and integrations.**

## 10. PM takeaway

The goal of SignalForge is not to prove that AI can summarize feedback. The stronger product question is whether better synthesis changes a product decision.

That distinction drives the entire MVP.

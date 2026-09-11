# SignalForge — Metrics & Measurement

## North-star metric

**Evidence-linked roadmap decisions** = percentage of roadmap decisions linked to at least three independent customer evidence items.

This metric reflects the product thesis: better decisions should remain grounded in evidence.

## Product metrics

| Metric | Definition | Initial target |
|---|---|---:|
| Evidence coverage | % roadmap decisions linked to ≥3 evidence items | 70%+ |
| Decision velocity | Median time from raw signal to ranked opportunity | <10 min |
| Reviewer agreement | % of reviewer rankings matching the PM ranking | 80%+ |
| Contradiction rate | % of opportunities with unresolved conflicting evidence | <10% |
| Evidence inspection | % decisions where supporting evidence was reviewed | 90%+ |

## Experiment metrics

### Primary
**Median time to produce a ranked top-three list.**

### Guardrails
- Reviewer confidence
- Evidence coverage
- Contradictory signals ignored
- Activation time where relevant
- Support contacts
- 7-day retention

## Why these metrics

Vanity metrics such as page views do not validate the product thesis. SignalForge therefore measures the quality and speed of the decision workflow itself.

## Instrumentation model

```text
signal_created
    ↓
signal_clustered
    ↓
evidence_reviewed
    ↓
opportunity_scored
    ↓
roadmap_decision_created
    ↓
prd_created
    ↓
experiment_launched
    ↓
outcome_recorded
```

## Measurement principle

A score is useful only if the team can inspect the assumptions behind it and later compare the decision with the outcome.

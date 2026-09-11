# PRD — SignalForge

## 1. Problem
PMs receive feedback across disconnected channels. Manual synthesis creates three failure modes: loud users outweigh representative users, feature requests are mistaken for problems, and prioritization rationale disappears after the meeting.

## 2. Target users
**Primary:** early-career and startup PMs managing 1–3 product surfaces.

**Secondary:** founders, product analysts, and engineering leads who need a shared decision record.

## 3. Jobs to be done
- When feedback arrives in many formats, help me identify recurring problems.
- When multiple opportunities compete, help me compare them consistently.
- When I choose a roadmap item, help me explain why it won.
- When I ship, help me define measurable evidence of success.

## 4. Hypothesis
If customer evidence is normalized and scored using a transparent framework, PMs will make faster, more defensible prioritization decisions.

## 5. MVP scope
### Must have
- Feedback ingestion model
- Theme grouping
- RICE calculator
- Opportunity scoring
- Roadmap view
- PRD generation template
- Experiment/metrics panel

### Won't have in MVP
- Production LLM integration
- Automatic Jira/Linear writes
- Real customer authentication
- Enterprise permissions

## 6. User stories
1. As a PM, I can inspect raw evidence before accepting an insight.
2. As a PM, I can change scoring assumptions and see the ranking update.
3. As a PM, I can convert a winning opportunity into a structured PRD.
4. As a PM, I can define a success metric before calling a feature successful.

## 7. Acceptance criteria
- Every ranked opportunity exposes its scoring inputs.
- Changing effort changes the RICE ranking.
- Every roadmap item links back to evidence IDs.
- A PRD contains problem, user, hypothesis, scope, non-goals, and acceptance criteria.
- The experiment view includes one primary metric and at least two guardrails.

## 8. Risks
| Risk | Mitigation |
|---|---|
| Scores create false precision | Show inputs + confidence; never hide assumptions |
| Feedback is biased | Preserve source and evidence count |
| PMs over-optimize for reach | Balance RICE with strategic fit and severity |
| AI hallucination | Keep evidence traceability and human approval |

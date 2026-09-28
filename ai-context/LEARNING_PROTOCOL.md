# Learning Protocol

## 1. The 70/20/10 allocation

Approximately:

- 70% building and experimentation
- 20% focused study
- 10% tracking the frontier

Adjust when a foundational gap genuinely requires more theory.

## 2. The 30-minute unblock rule

If blocked for ~30 minutes:

1. State the exact failure.
2. Reduce the problem.
3. Build the smallest reproducible example.
4. Inspect assumptions and error messages.
5. Consult documentation/source material.
6. Ask an AI assistant with the exact evidence.
7. Continue or explicitly defer.

Never spend several days silently stuck.

## 3. Topic completion criteria

A topic is considered learned when the user can:

- explain it without notes
- implement a minimal version
- use a modern implementation
- identify at least two failure modes
- run one meaningful experiment
- explain when the technique should not be used

Not every topic needs publication.

## 4. Build-before-framework rule

For important mechanisms, first understand a minimal implementation before relying on a framework abstraction.

Examples:

- attention before an agent framework
- retrieval before a RAG framework
- tool calling before an agent framework
- fine-tuning mechanics before a managed fine-tuning product

## 5. Experiment protocol

Every non-trivial experiment should record:

- hypothesis
- setup
- variables
- baseline
- metric
- result
- interpretation
- limitations
- next experiment

## 6. AI collaboration protocol

An AI assistant should:

- inspect current context first
- avoid repeating mastered topics
- distinguish facts from hypotheses
- state uncertainty
- cite primary sources for current claims
- challenge conclusions
- preserve the user's authorship

## 7. Handoff protocol

Before switching assistants:

1. Update `CURRENT_CONTEXT.md`.
2. Update the session log.
3. Record unresolved questions.
4. Record the exact next action.

The next assistant receives the context files and continues from there.

## 8. Anti-hype filter

For every new AI technology ask:

- What problem does it solve?
- Compared with what?
- Is the improvement measured?
- Under what conditions?
- Is it durable knowledge or a temporary implementation detail?
- Does learning it support the current goal?

If not, put it in `resources/BACKLOG.md`.

## 9. Weekly review

Every 7 days:

- review milestones
- identify weak areas
- remove unnecessary backlog
- choose the next week's highest-value outcome
- update current context
- publish or archive one artifact if appropriate

## 10. Monthly review

Every 30 days:

- review technical breadth
- review depth
- inspect project quality
- inspect public portfolio
- identify one area for deeper specialization
- revise the next 60 days without destroying the long-term roadmap

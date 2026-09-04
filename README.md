# Juno PM — AI Copilot for Retail Business Metrics

> Juno is an Al PM to turn unstructured user requests and comments into prioritized analytical metrics every week.

_Neko Yau · AI PM Cohort · Sep 2026_

Repo: https://github.com/nekoyau/juno-pm

This repo is my final project for the AI Product Management Certification — **Juno PM**. Each module’s artefact lives in its own folder; this README is the dashboard and the pitch.

---

## Module artefacts

### M1 · Prompting
- **System prompt** — [`01-prompting/system-prompt.md`](01-prompting/system-prompt.md)
- **Prototype** — https://juno-aipm-after-rag.lovable.app

### M2 · Strategy
- **Decision matrix** — [`02-strategy/decision-matrix.md`](02-strategy/decision-matrix.md)
- **AI Strategy one-pager** — [`02-strategy/strategy-one-pager.md`](02-strategy/strategy-one-pager.md)

### M3 · RAG / AI PRD
- **AI PRD** — [`03-rag-prd/prd.md`](03-rag-prd/prd.md)

### M4 · AI-Native UX
- **AI user flow** — [`04-ai-ux/user-flow.md`](04-ai-ux/user-flow.md)
- **Trust-gap mitigations** — [`04-ai-ux/trust-gaps.md`](04-ai-ux/trust-gaps.md)

### M5 · Agentic Workflows
- **Agent Workflow Spec (AWSpec)** — [`05-agentic-workflows/awspec.md`](05-agentic-workflows/awspec.md)
- **Agent Control Panel** — [`05-agentic-workflows/agent-control-panel.md`](05-agentic-workflows/agent-control-panel.md)

### M6 · Evals &amp; Guardrails
- **Eval stack** — [`06-evals/eval-stack.md`](06-evals/eval-stack.md)
- **Human evaluation rubric** — [`06-evals/human-rubric.md`](06-evals/human-rubric.md)

---

## PM Execution Plan

### Where Juno is today
- M1–M6 specced and committed.
- The prototype validates the M1 flow with the team.
- Automated evals: 80-item golden set drafted, judge prompt validated against 30 items; not yet connected to the automated engineering pipeline.
- Human rubric drafted; 2 grader candidates lined up; no calibration round yet.

### What ships next (next 2 sprints)
- Sprint 1: connect AI eval to automated engineering pipeline; staff and calibrate 2 graders; ship the Slack triage tool.
- Sprint 2: open closed beta with 3 PMs (1 PM, 2 SMEs); weekly rubric review; instrument abandon-rate.

### What I watch (dashboards)
- Daily: thumbs-down rate, regen rate, hand-off rate.
- Weekly: human-rubric mean per dimension; refusal hit-rate; cost per run.
- Per release: golden-set accuracy; format/citation/refusal pass rate.

### Red lines (what blocks shipping)
- Any critical-safety fail (any "1" on safety dimension in human eval).
- <85% golden-set accuracy on automated layer.
- Fake content or persona (SME) name in last 7 days.
- Cost >$0.50 per run.
- P99 latency >5s on triage flow.

### Governance
- Compliance: obey user privacy law, follow corporate business policy, ethics
- Safety: prompt-injection eval row in golden set; refusal on financial/legal content.
- Reliability: 99.5% SLO; cached top-3 fallback if model is down.
- Reputation: 2-hour incident-response playbook in /docs; canary deploys for every model swap.

---

## Build Insights

- **Friction point.** learning-wise: Many new technical terminologies and concepts first time heard from this program, require more time to digest and review get understand more. I am frustrated if I should have more technical knowledge and get to know more tools to be a AI PM. Definitely will keep exploring. product-wise: Retrieval quality was challenging — getting the correct business use cases mattered more than the model. 
- **Key learning.** was curious if human can fully/ mostly leave the work to AI, what-if the output is not as expected? Glad to know that human must set Evals and Guardrails which can act almost like a human to self-check and save human effort to validate. Though Human review is still critical over time to avoid model drifting. 
- **Aha moment.** Probabilistic instead of deterministic; Human Oversight is still critical (good to know!)

---

_Certification submission — AI Product Management Certification._


---

## Repo structure

```
juno-pm/
├── README.md                          ← this dashboard + pitch
├── 01-prompting/
│   ├── system-prompt.md               ← M1: Juno's system prompt
│   └── lovable-prototype.md           ← M1: prototype link + debrief
├── 02-strategy/
│   ├── decision-matrix.md             ← M2: build / buy / fine-tune / partner call
│   └── strategy-one-pager.md          ← M2: AI strategy one-pager
├── 03-rag-prd/
│   └── prd.md                         ← M3: AI PRD with retrieval requirements
├── 04-ai-ux/
│   ├── user-flow.md                   ← M4: AI-native user flow
│   └── trust-gaps.md                  ← M4: trust-gap mitigations
├── 05-agentic-workflows/
│   ├── awspec.md                      ← M5: Agent Workflow Spec
│   └── agent-control-panel.md         ← M5: Agent Control Panel
└── 06-evals/
    ├── eval-stack.md                  ← M6: layered eval stack
    └── human-rubric.md                ← M6: human evaluation rubric
```

---

_Certification submission — AI Product Management Certification._

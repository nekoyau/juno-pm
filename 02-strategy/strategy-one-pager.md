# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

The Problem: too many use cases and OKRs conservations and comments in different channels. It is difficult to consolidate all the requests and business needs for prioritization and building the roadmap.

Prevention: explicitly prevents 'out-of-scope content' - stakeholders may ask for something irrelevant to the high-level scope, for example: it is about an analytical dashboard of sales-driven demand on materials, while some ask for quality assurance metrics which is not related to sales-driven aspect.

## 2. Target Metrics

Cycle time: reduce average weekly roadmap prioritization from 2-3 hours to 30-45 minutes.

Leadership proof: at least 70% of the prioritized metrics can be decided within 1 week, AND all of them have use cases and OKRs enabled to the stakeholders. 

## 3. Autonomy Level

Choice: Copilot - drafts a ranked priorities with written reasoning + source citations; the human PM reviews and clicks 'approve' before publish.

Explicitly avoiding: Agent. Letting AI moves sprint priorities or modify the context without a human approval step might overlook the key stakeholders' concerns - a single wrong call can result in stakeholders dismiss the system permanently.

## 4. Data & Model Approach

Approach: Buy (LLM). The major needs is consolidation, summarization and categorization the conversations from different source channels (Slack, Zoom meetings recap and recordings).

Explicitly avoiding: Refine (Fine-tune). Without human review and validation, with too much human voices around, AI may create priorities and invent customer signals that don't exist - the failure mode that kills trust fastest.

## 5. Risks & Mitigations

Risk: breakdown source content. the same message from a SME might be posted in separate messages in the source channels which e.g. 3 consecutive threads actually come into 1 comment/callout. AI might miss this and treat as irrelevant content then miss it. 

Mitigation: logic check for consecutive threads posted within 5 min. from the same person - combine those threads as 1 thread before proceeding next. Run weekly; human PM must review.

## 6. V1 Scope

In: ranking the raised business requests based on the number of incidences with cited evidence; surfacing low ranked items but the conversational content may sound critical to the SMEs; flagging conflicts between Slack comments and Zoom meeting conversations (transcripts).

Out: (1) hiring or headcount decisions, (2) separate the items about why a feature was low ranked but required deeper review. Both stay 100% with the human PM.

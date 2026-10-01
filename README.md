# ResolveAI V3 - Stateful AI Operations Copilot

ResolveAI is an interactive portfolio prototype built to demonstrate AI product thinking beyond a generic chatbot.

## What V3 demonstrates

- End-to-end workflow state across Inbox -> AI Analysis -> Human Review
- Structured AI outputs for downstream product logic
- Evidence-first prompting and missing-information detection
- Human approval gates for sensitive actions
- Deterministic product rules around the model
- Editable prompt architecture and output contracts
- A repeatable Challenge Set for prompt regression checks
- Clear separation between what this local prototype can verify and what would require a real model/backend

## Why the metrics changed

V3 intentionally avoids invented performance percentages.

The UI now shows only explainable prototype checks such as:
- 7 / 7 required structured fields
- 3 / 3 grounding checks
- 3 / 3 approval/guardrail checks
- 4 repeatable challenge cases

Accuracy, latency, cost and production quality would require a real backend, real model calls and a versioned evaluation dataset.

## Human Review lifecycle

Each active case has one consistent review state:
- Awaiting decision
- Edited
- Approved
- Escalated

Approve and Escalate are final states in this prototype, so contradictory decisions cannot be recorded afterward.

## Challenge Set

The AI Lab includes four repeatable behavior tests:
1. Missing identity evidence in an access request
2. Missing validation evidence in a CSV failure
3. Unverified requester for master-data changes
4. Complete structured output contract

The tests use the current Prompt Playground configuration so a weak prompt visibly fails checks that the production-style preset passes.

## Run locally

Open `index.html` in a browser.

## GitHub Pages

Upload `index.html` and `README.md` to your `resolveai` repository and publish from the `main` branch, root folder.

Live URL pattern:
`https://idan818.github.io/resolveai/`

## Portfolio positioning

Suggested description:

"Concepted and built an interactive AI operations prototype using AI-assisted development, with focus on prompt architecture, structured outputs, evaluation, stateful workflows, human approval and controlled automation."

This is a portfolio prototype, not a production system and not a live LLM integration.

---
prompt_id: PROMPT-ENG-01
type: implementation
version: v0.1
target_agent: generic-coding-agent
project: TraceSpec
status: Ready
sources:
  - prompts/tracespec/00-project-context.md
  - docs/product/tracespec/PRD.md
  - docs/product/tracespec/PLAN.md
requirements: [FR-01, FR-03]
flows: [FLOW-01, FLOW-03]
screens: [SCR-01, SCR-03]
tasks: [TASK-01, TASK-02, TASK-03]
tests: [TEST-01, TEST-03]
---

# Implement M0 — Foundation

## Objective
Set up the product-information foundation required for TraceSpec: stable artifact IDs, document structure, project context, and traceability-aware data contracts.

## Scope in
- Define models/types for artifact IDs and trace links.
- Define project, PRD, requirement, flow, screen, task, and test contracts.
- Add validation that marks missing required links as `[TRACE GAP]`.
- Seed a minimal TraceSpec project from the committed blueprint.

## Scope out
- Visual editor.
- Authentication.
- GitHub write integration.
- AI model orchestration.

## Acceptance criteria
- A requirement can link to problem, goal, story, flow, screen, task, and test.
- Missing critical links are surfaced as `[TRACE GAP]`.
- Seeded project can represent IDs P-01, FR-01, FLOW-01, SCR-01, TASK-01, dan TEST-01.
- Implementation has tests for valid and missing-link cases.

## Required response
Before coding: list files to inspect, plan, assumptions, and tests. After coding: changed files, completed IDs, tests, limitations, and next build packet.

## Stop conditions
Stop if repository architecture, language, storage choice, or test framework is not established. Do not invent them.

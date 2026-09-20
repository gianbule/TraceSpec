---
prompt_id: '{{PROMPT_ID}}'
type: implementation
version: '{{VERSION}}'
target_agent: '{{TARGET_AGENT}}'
project: '{{PROJECT}}'
status: Ready
sources: ['{{CONTEXT}}', '{{PRD}}', '{{TASK}}', '{{TEST_PLAN}}']
requirements: ['{{FR_IDS}}']
flows: ['{{FLOW_IDS}}']
screens: ['{{SCR_IDS}}']
tasks: ['{{TASK_IDS}}']
tests: ['{{TEST_IDS}}']
---

# Implement {{MILESTONE}}

## Objective
{{OBJECTIVE}}

## Read first
Read every file in `sources` before changing code.

## Scope in
{{SCOPE_IN}}

## Scope out
{{SCOPE_OUT}}

## Acceptance criteria
{{ACCEPTANCE_CRITERIA}}

## Required response
Before coding: files to inspect, plan, ambiguity, test approach.
After coding: summary, changed files, completed IDs, test result, limitation, next packet.

## Stop conditions
Stop and ask when requirements conflict, data model is undefined, a new integration is needed, scope expands, or acceptance criteria are missing.

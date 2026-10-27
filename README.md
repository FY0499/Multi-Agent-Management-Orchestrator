# Multi-Agent Management Orchestrator

An n8n workflow that uses a master AI agent to coordinate specialized agents for company-management requests.

## What it does

1. Receives a manager's request through Telegram.
2. The master agent creates a short plan.
3. Data, Finance, and HR agents independently provide insights.
4. A merge step gathers the reports for the master agent's decision.
5. Operations, Sales, and Security agents produce follow-up recommendations.
6. The workflow sends the generated responses to Telegram.

## Workflow file

Import [workflow.json](./workflow.json) into n8n.

## Setup

- Configure a Telegram Trigger and Telegram send-message credential in n8n.
- Connect a supported chat model credential to the Anthropic Chat Model node, or replace it with a model provider you use.
- Review the node connections and expressions, then test with a non-sensitive request before activating.
- The exported workflow does not include credentials. You must configure your own credentials after importing.

## Notes

This is an exported workflow, not a guarantee that it runs without configuration. Verify the model name and provider availability in your n8n instance before use.

# Multi-Agent Management Orchestrator

I built this n8n workflow to coordinate multiple AI agents and help organize management requests. A main agent receives the request, works with specialized agents, and sends the combined response through Telegram.

<img width="646" height="249" alt="Multi-Agent Management Orchestrator demo" src="https://github.com/user-attachments/assets/9bad544e-b50d-477f-8bd3-d28527804f09" />

## How it works

1. A manager sends a request through Telegram.
2. The main AI agent organizes the request and delegates tasks.
3. Specialized agents work on Data, Finance, HR, Operations, Sales, and Security topics.
4. Their outputs are brought together to prepare the response.
5. The workflow sends the result back through Telegram.

## Technologies

n8n, AI Agents, Anthropic Chat Model, Telegram, and multi-agent orchestration.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Telegram credentials and Anthropic model credentials, then review the agent connections and prompts.

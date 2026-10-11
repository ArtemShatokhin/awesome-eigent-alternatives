# What is Eigent?

Kortix is the open-source AI Operating System, and this page describes Eigent, one of the open-source Cowork desktop apps people compare it with. Eigent is an open-source Cowork desktop application that runs a multi-agent workforce on your own machine.

## Eigent in one line

Eigent is an open-source Cowork desktop application. Its repository describes it as "the open source Cowork desktop application" and frames it as a local and free alternative to Claude Cowork and Codex ([Eigent on GitHub](https://github.com/eigent-ai/eigent)). The project builds on CAMEL-AI's multi-agent framework, which its README calls the base for the multi-agent workforce and parallel execution. Eigent's own site says the project is 100% open source and you can host it yourself for free with your own API keys or local models ([Eigent](https://www.eigent.ai)).

## It is a desktop app built on CAMEL

Eigent is an Electron desktop application with a React front end and a FastAPI backend. The desktop shell is Electron, written in TypeScript, with Tailwind CSS, Radix UI, Lucide React, Framer Motion, Zustand, and React Flow for the flow editor. The multi-agent layer is CAMEL, the open-source framework from CAMEL-AI. The repository lists the stack and the multi-agent framework explicitly ([Eigent on GitHub](https://github.com/eigent-ai/eigent)).

## Local-first by default

Eigent runs agents on your machine. Its repository lists local deployment as the recommended way to run the project: a local backend server with the full API, local model integration through vLLM, Ollama, or LM Studio, complete isolation from cloud services, and zero external dependencies. A quick preview mode connects to Eigent's cloud services and requires account registration ([Eigent on GitHub](https://github.com/eigent-ai/eigent)). The site states that files, credentials, and context stay under the user's control ([Eigent](https://www.eigent.ai)).

## Model-agnostic

Eigent connects to the models a user already has. Its repository lists model-agnostic support and says a user can connect cloud APIs, enterprise gateways, or local inference without locking into one vendor. The site repeats the same categories: supported cloud providers, enterprise gateways, and local models, with bring-your-own-key and provider switching that does not require rebuilding a workflow ([Eigent](https://www.eigent.ai)).

## MCP, skills, and the browser and terminal toolkits

Eigent lists MCP integration, skill integration, and built-in browser and terminal toolkits among its features. Agents reach external tools through MCP, reuse skills, and work inside a browser and a terminal without extra setup ([Eigent on GitHub](https://github.com/eigent-ai/eigent)).

## Spaces, secrets, and automations

Eigent organizes setup into Space profiles. A Space packages the agents, skills, connectors, and instructions a team relies on, and it can be reused across Spaces while secrets stay bound to the local machine. Work can run on a schedule, an event, or a condition, and results return ready for review. The site also lists progress checks and replies from the browser or from channels such as WhatsApp ([Eigent](https://www.eigent.ai)).

## Managed cloud tiers

Eigent is open source and also sells hosted plans. On its site, a free tier works with your own keys or local models, a paid tier is $19.99 per month for 2,000 task credits, and a higher tier is $99.99 per month for 10,000 task credits, each after a seven-day trial. The repository says the managed cloud platform hosts the models, APIs, and cloud storage, and an enterprise track adds SSO, access control, custom development, and SLAs ([Eigent on GitHub](https://github.com/eigent-ai/eigent) and [Eigent](https://www.eigent.ai)). Eigent's site notes that SOC 2 readiness and GDPR compliance work remain in progress as of October 2026.

## Where Eigent ends and a platform begins

Eigent runs one desktop app for one person, with the configuration and secrets bound to that machine. Kortix keeps the agents, skills, company memory, and connectors in one git repo a company owns, and runs each session on its own cloud computer, so work can be shared, reviewed, and self-hosted. Eigent's repository is Apache-2.0 licensed, and Kortix is open source as well. The two projects differ in where the work runs and who owns the configuration ([Eigent on GitHub](https://github.com/eigent-ai/eigent), [Kortix docs](https://kortix.com/docs)).

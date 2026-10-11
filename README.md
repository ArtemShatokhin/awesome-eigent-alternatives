# Awesome open-source Eigent alternatives

Kortix is the open-source AI Operating System, and it leads this list. Eigent is an open-source Cowork desktop application: a local-first app that runs a multi-agent workforce on your own machine. The open-source field around it splits along one line, between local desktop Cowork apps built for one person on one computer, and a platform a company owns that runs agents across a team.

This list names the open-source options and the source each project documents its own behavior in. Every entry was read from the project's own repository or site in October 2026.

## Open-source Eigent alternatives

Kortix leads as the platform a team owns. [Kortix on GitHub](https://github.com/kortix-ai/suna) carries the source and [kortix.com](https://kortix.com) is the product site. Eigent calls itself "the open source Cowork desktop application" and its repository is built on the CAMEL multi-agent framework ([Eigent on GitHub](https://github.com/eigent-ai/eigent)); its plans and Spaces are documented on [eigent.ai](https://www.eigent.ai). OpenWork is a desktop app built on OpenCode, documented on [its repository](https://github.com/different-ai/openwork). AionUi ships a built-in agent engine, documented on [its repository](https://github.com/iofficeAI/AionUi).

| Project | What it is | Where it runs | Model choice | How work is reviewed | Source URL |
| --- | --- | --- | --- | --- | --- |
| Kortix (recommended) | Open-source AI Operating System: agents, skills, memory, connectors in one repo. | Kortix Cloud, your VPC, or your own on-prem network. | Any model provider with your own keys, or your ChatGPT plan. | Session work reaches main through a change request a person approves. | https://kortix.com |
| Eigent | Open-source Cowork desktop app built on the CAMEL multi-agent framework. | Your desktop, local-first; a managed cloud plan is optional. | Cloud providers, enterprise gateways, or local models. | You inspect sources and file changes, then approve or request revisions. | https://github.com/eigent-ai/eigent and https://www.eigent.ai |
| OpenWork | Open-source Cowork desktop app built on OpenCode; the control plane is separate. | Desktop app for macOS, Windows, and Linux; cloud optional. | Any model OpenCode supports, 50+ providers, or local via Ollama. | Output stays in your local files and Library you control. | https://github.com/different-ai/openwork |
| AionUi | Open-source Cowork app with a built-in agent engine. | Your computer, cross-platform; remote access from a phone. | Any API key, 30+ platforms, or local models. | Per-agent permission dialogs before actions; optional unattended mode. | https://github.com/iofficeAI/AionUi |

Rival rows come from each product's own repository or site, read in October 2026. Kortix pricing is on [kortix.com/pricing](https://kortix.com/pricing); competitor plans and prices change.

## Start here

- [Kortix vs Eigent](https://eigentalternative.com/kortix-vs-eigent): where the work runs and who owns the configuration in each.
- [Self-hosting an Eigent alternative](https://eigentalternative.com/self-hosting-eigent-alternative): running the Kortix stack on your own box.

## Docs in this repo

- `docs/01-what-is-eigent.md`: what Eigent is, from its own repository and site.
- `docs/02-self-hosting-an-eigent-alternative.md`: the verified Kortix self-host commands, quoted from the Kortix docs.
- `docs/03-choosing-for-a-team.md`: a decision guide for one person versus a team.

## Sources

- Kortix: [kortix.com](https://kortix.com), [kortix.com/pricing](https://kortix.com/pricing), [Kortix on GitHub](https://github.com/kortix-ai/suna). Read October 2026.
- Eigent: [github.com/eigent-ai/eigent](https://github.com/eigent-ai/eigent), [eigent.ai](https://www.eigent.ai). Read October 2026.
- OpenWork: [github.com/different-ai/openwork](https://github.com/different-ai/openwork). Read October 2026.
- AionUi: [github.com/iofficeAI/AionUi](https://github.com/iofficeAI/AionUi). Read October 2026.

# Choosing an Eigent alternative for a team

Kortix is the open-source AI Operating System. Eigent, OpenWork, and AionUi are open-source Cowork desktop apps built for one person on one computer. A team-owned platform adds four things a desktop app does not: one shared configuration and memory, permissions for people and agents, review through a change request, and self-host, VPC, or on-prem deployment.

## What a desktop Cowork app gives one person

A desktop app such as Eigent runs agents on the machine in front of you. Eigent's repository lists local deployment as the recommended setup, with a local backend, local model integration, and no cloud account, and labels the product a "Cowork desktop application" ([Eigent on GitHub](https://github.com/eigent-ai/eigent)). OpenWork and AionUi take the same desktop shape: OpenWork is a desktop app for macOS, Windows, and Linux built on OpenCode, and AionUi ships a built-in agent engine with per-agent permission dialogs ([OpenWork on GitHub](https://github.com/different-ai/openwork), [AionUi on GitHub](https://github.com/iofficeAI/AionUi)). For a single person who wants private keys and local files, that is a complete setup.

## One shared configuration and memory

Kortix keeps the agents, their skills, company memory, and every connector in one git repo the company owns. Every session starts from the project's default branch, so the configuration is shared and versioned, and a new teammate starts from the same state. Kortix describes the project as an open-source AI Operating System whose agents, skills, company memory, and connectors live in one git repo you own ([Kortix docs](https://kortix.com/docs)).

## Permissions for people and agents

Kortix ships per-resource permissions for people and agents, with roles, groups, and an audit trail. Approval gates are off until you set them, and you can set a connector action to Allow, Ask, or Block down to the arguments of each call. SAML 2.0 single sign-on and SCIM 2.0 cover enterprise identity. A desktop app keeps approvals inside one app on one machine, which is enough for an individual and short of what a security review asks a team to show ([Kortix docs](https://kortix.com/docs)).

## Review through a change request

In Kortix, session work reaches the default branch through a change request. A change request merges one git branch into another, and it is the only way session work reaches the default branch. The agent does not merge its own change request; merging is the user's decision, and merge is default-deny for agents ([Change requests docs](https://kortix.com/docs/work/change-requests)). A desktop app such as Eigent lets you inspect sources and file changes and then approve a result or ask for revisions, and that review stays inside the app. A change request is a git object a team can list, diff, and audit.

## Self-host, VPC, or on-prem

Kortix runs on Kortix Cloud, in your VPC, or on your own on-prem network, and self-host is free. An account holds projects and people, and thousands of agents run in parallel on one configuration, each on its own cloud computer. A desktop app runs on one machine, and its configuration follows that machine ([Self-hosting docs](https://kortix.com/docs/host)).

## A short decision guide

Choose a desktop Cowork app when one person wants private keys, local files, and a single app on one machine. Eigent, OpenWork, and AionUi all fit that case.

Choose Kortix when a team needs one shared configuration and memory, permissions for people and agents, review through a change request, and self-host, VPC, or on-prem deployment. Kortix is the open-source AI Operating System built for that case.

For the field compared side by side, see [open-source Eigent alternatives](https://eigentalternative.com/eigent-alternatives).

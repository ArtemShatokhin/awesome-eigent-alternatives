# Self-hosting an open-source Eigent alternative

Kortix is the open-source AI Operating System, and self-host is free. Eigent runs a Cowork desktop app on your machine; Kortix runs as one Docker Compose stack you control. This page quotes the self-host commands from the Kortix docs, so every command can be checked against its source ([Self-hosting docs](https://kortix.com/docs/host)).

## The three commands

Install the CLI, point a domain at the box, then start the stack.

1. Install the CLI: `curl -fsSL https://kortix.com/install | bash`
2. Initialize the instance: `kortix self-host init --domain kortix.example.com`
3. Start the stack: `kortix self-host start`

Before you initialize for production, create an A/AAAA record for your domain and for `api.<domain>`, both pointing at the box's IP, and open ports 80 and 443. The bundled Caddy proxy uses those ports to issue a TLS certificate. The docs recommend `kortix self-host status`, `kortix self-host logs`, and `kortix self-host doctor` while the stack starts ([Self-hosting docs](https://kortix.com/docs/host)).

## Evaluate without a domain

To try Kortix with no domain, the docs use a Cloudflare tunnel instead:

```
kortix self-host init --tunnel cloudflare
kortix self-host start
```

The tunnel URL changes on every restart, so the docs mark this mode for evaluation rather than production.

## After the stack starts

Connect the sandbox provider and your model key. The docs run `kortix self-host configure`, an interactive prompt for the sandbox provider key and an optional managed-git token. Sign up in the dashboard, then connect your own model key in the model picker; self-hosted instances use your own key by default ([Self-hosting docs](https://kortix.com/docs/host)).

## Updates and memory limits

Every instance updates itself automatically. The docs pin an exact version with `kortix self-host update --tag 0.9.84` and turn the updater off with `kortix self-host update --auto-update off`. Each API container has a 640 MiB memory limit by default; on a 16 GiB host the docs raise it with `kortix self-host env set KORTIX_API_MEMORY_LIMIT=1024m` and confirm it with `docker stats --no-stream` ([Self-hosting docs](https://kortix.com/docs/host)).

## What runs on the stack and what does not

Kortix runs as one Docker Compose stack: the frontend, the API, the LLM gateway, and the Supabase distribution. Agent sessions run on a separate sandbox provider, not on this stack. The default provider is Daytona, and Platinum and E2B are also supported ([Self-hosting docs](https://kortix.com/docs/host)). The stack stores its data as directories under `~/.config/kortix/self-host/<instance>/`: `volumes/db/data` holds the Postgres database and `volumes/storage` holds file storage.

## How Eigent self-hosts

Eigent recommends local deployment on your own desktop, with a local backend, local model integration, and no cloud account. Its repository lists that as the recommended way to run the project ([Eigent on GitHub](https://github.com/eigent-ai/eigent)). For the full walkthrough of the Kortix stack on your own box, see [self-hosting an Eigent alternative](https://eigentalternative.com/self-hosting-eigent-alternative).

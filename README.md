# Arnaldo Sepulveda

Senior AI Engineer building governed AI systems for regulated enterprises.

Nearly 13 years at Genesys working across the AI intelligence layer of enterprise contact centers: Knowledge Center retrieval, chat suite, e-services, contact intelligence. That was conversational AI in regulated and public-sector environments long before LLMs became fashionable.

Now building **Keystone Applied Intelligence**: a local, regulated AI platform for governed retrieval, multi-agent orchestration, and reproducible evaluation. The goal is simple: make AI systems behave like they are operating under real regulatory pressure, not demo conditions.

## What I build

Keystone is not a chatbot demo and not a thin wrapper around an API. It is a platform for AI systems that must be:

- evidence-backed,
- fail-closed when evidence is insufficient,
- access-controlled at query time,
- auditable after the fact,
- deployable on customer-controlled infrastructure.

The platform runs on-premises with local models and no external API dependency for core operation.

## Keystone platform

Three extensions currently prove the platform in different ways:

- **Keystone Engage** — governed conversational agents for regulated customer interaction.
- **Keystone Counsel** — authorization-first retrieval for legal, financial, and compliance content.
- **Keystone Verify** — standalone evaluation harness for governed AI systems.

These sit on a shared substrate for:

- agent identity and role registration,
- task lifecycle state management,
- hash-chained audit logging,
- event-driven coordination,
- local or remote dispatch abstraction,
- sealed evaluation artifacts.

That is the actual product: not one app, but the operating model underneath multiple regulated AI workloads.

## What is already proven

This work is not positioned as roadmap fiction. It has live demos, published baselines, failing runs, passing runs, and public artifacts.

Published proof points include:

- governed retrieval baseline with adversarial ACL blocking and fail-closed behavior,
- governed agent baseline with 186 test cases across 12 categories and 0 failures,
- evaluation methodology strong enough to uncover real bugs in the system it was testing,
- public failing runs preserved alongside passing runs.

The point is not just to ship AI behavior. The point is to make claims that can survive inspection.

## Technical position

Most LLM systems are still missing the operational discipline that enterprise contact centers had to learn years ago:

- severity-tier escalation,
- per-step validation,
- compliance logging,
- confidence-threshold refusal,
- explicit routing under policy and cost constraints.

Keystone rebuilds that discipline for the LLM substrate.

## Current stack

Python · FastAPI · PostgreSQL 16 + pgvector · Ollama · React / TypeScript · Docker Compose · NATS JetStream · Grafana Tempo · Caddy · Tailscale

## Current focus

- governed conversational agents,
- authorization-first retrieval,
- audit-grade agent orchestration,
- portable evaluation infrastructure,
- local-first deployment for regulated environments.

## Links

- Website: https://getkeystone.ai
- Demo: https://demo.getkeystone.ai
- Blog: https://getkeystone.ai/blog
- Keystone org: https://github.com/getkeystone
- LinkedIn: https://www.linkedin.com/in/arnaldosepulveda
- Contact: arnaldo@getkeystone.ai

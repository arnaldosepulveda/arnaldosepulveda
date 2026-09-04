# Arnaldo Sepulveda

AI Engineer & Builder working at the intersection of enterprise Customer Support and applied AI.

## Background

12+ years at Genesys in enterprise Customer Support and Technical Escalations: contact-center systems, Digital Services, Agent Workspace, customer and interaction data, routing and integrations, WFM-integrated workflows, severe incident investigation, and migrations and go-lives. That included earlier enterprise conversational and classification systems (Knowledge Center retrieval, chat suite, e-services) — those predate the current generation of LLM-based systems and I don't describe them as such.

## Why I moved into applied AI

The organizations I supported already had the knowledge they needed. It was fragmented across tickets, documentation, conversations, and individual experts, and skilled people kept reconstructing context the organization had already encountered. The organization already possessed the knowledge, but had not operationalized it so the right person could reliably get the right answer in the right context.

That's the problem I build for now: AI should reduce reconstruction work, not remove judgment where judgment matters.

## What I build

Through [Keystone Applied Intelligence](https://getkeystone.ai), an independent applied-AI engineering and R&D practice, I build and evaluate reference implementations: authorization-aware retrieval, hybrid RAG with deterministic reranking, conversational and workflow agents, and the evaluation infrastructure to hold them accountable — on PostgreSQL/pgvector, local model serving, and OpenTelemetry-instrumented services.

The more important habit behind the work is the cycle: understand the operational problem, find the constraint, establish a baseline, decide whether AI is actually the right intervention, build the smallest justified version, evaluate it both technically and with real users, measure the operational effect, and recommend scale, modify, or stop.

## Evidence

Keystone's repositories are separately composed engineering instruments, not one demonstrated production platform. Evaluation evidence — including failing runs — is retained and public:

- [keystone-engage](https://github.com/getkeystone/keystone-engage) — conversational agent reference implementation
- [keystone-counsel](https://github.com/getkeystone/keystone-counsel) — authorization-first retrieval
- [keystone-verify](https://github.com/getkeystone/keystone-verify) — standalone evaluation harness
- [keystone-ledger](https://github.com/getkeystone/keystone-ledger) — retained internal evaluation lineage, including failing runs

## Research

A secondary, deeper thread: [Governed Execution](https://github.com/getkeystone/runtime-validity), a research program on runtime governance for agentic systems. Runtime Validity is its bounded Track A reference implementation.

## Links

- Site: https://arnaldosepulveda.com
- Writing: https://arnaldosepulveda.com/writing/
- Keystone: https://getkeystone.ai
- Keystone org: https://github.com/getkeystone
- LinkedIn: https://www.linkedin.com/in/arnaldosepulveda

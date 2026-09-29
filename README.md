# Arnaldo Sepulveda

I spent 12+ years at Genesys in enterprise Technical Support and Escalations, diagnosing production problems across contact-center routing, digital channels, agent desktop, customer and interaction data, knowledge and search systems, and integrations. I hold a BScE and MScE in Electrical Engineering.

My Genesys work was Support and Escalations, not product development. This GitHub shows separate, independent technical work since late 2024, mostly under Keystone Applied Intelligence.

## What these repositories demonstrate

- Python services and APIs (FastAPI, Pydantic) over PostgreSQL, including full-text plus pgvector hybrid retrieval
- Access control enforced at retrieval time, including a cross-client isolation defect found, fixed, and covered by regression tests
- Evaluation as part of engineering: declarative test cases, retained failing runs, regression evidence
- Conversational workflows with explicit task state, escalation, and human handoff
- Observability with OpenTelemetry tracing
- Reproducible data work: a tested pipeline over 7.47 million public Calgary 311 records

## Start here

| Repository | What it shows |
|---|---|
| [keystone-gov](https://github.com/getkeystone/keystone-gov) | Hybrid retrieval and RAG API with citations, evidence thresholds, and query-time access control |
| [keystone-counsel](https://github.com/getkeystone/keystone-counsel) | Authorization-first retrieval with role, document-classification, and client-isolation filters |
| [keystone-verify](https://github.com/getkeystone/keystone-verify) | Endpoint-agnostic evaluation harness with declarative assertions and structured JSON results |
| [keystone-engage](https://github.com/getkeystone/keystone-engage) | Conversational workflow reference implementation with task state, escalation, and human handoff |
| [support-operations-intelligence](https://github.com/arnaldosepulveda/support-operations-intelligence) | Contract-based ingestion, validation, and baselines over 7.47M public records, with a 218-test suite |

One retained internal evaluation of keystone-gov used 186 cases across 12 categories (558 executions) and surfaced four implementation defects before release. Runs, including the failing predecessor, are in [keystone-ledger](https://github.com/getkeystone/keystone-ledger).

## What these repositories do not claim

- They are independent projects, not paid client work.
- They are separate reference implementations, not one integrated production platform.
- Internal evaluation results apply to specific commits and runs. They are not independent validation.
- A retrieval prototype from this work was piloted by a small group at a volunteer fire department. That is a small real-user pilot, not an organization-wide deployment or a measured outcome.
- [runtime-validity](https://github.com/getkeystone/runtime-validity) is exploratory research, not a deployed capability.

[LinkedIn](https://www.linkedin.com/in/arnaldosepulveda/) · [arnaldosepulveda.com](https://arnaldosepulveda.com/) · [getkeystone.ai](https://getkeystone.ai/) · [Keystone on GitHub](https://github.com/getkeystone)

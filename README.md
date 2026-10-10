# Arnaldo Sepulveda

**Enterprise Technical Solutions | 12+ Years at Genesys | CX Platforms, APIs & Integrations | Production Diagnosis | Applied AI**

## Professional background

I spent more than 12 years at Genesys in Technical Support and Escalations, working with enterprise and public-sector customers across North America, Latin America, and EMEA.

My work involved difficult production diagnosis across enterprise CX/contact-center platforms, integrations, routing, digital channels, knowledge systems, conversational AI, customer and interaction data, agent applications, and distributed systems.

I worked directly with customers, Product, and Engineering to isolate problems, reproduce failures, investigate configuration and integration issues, distinguish product defects, recommend technical changes, and support migrations, go-lives, and post-launch stabilization.

Earlier responsibilities included product-specialist customer discovery, including onsite engagements, and translating workflow and deployment constraints into technical requirements. During my final months I served as technical lead for a six-person Genesys Cloud CX UI Support team, providing diagnostic guidance and coaching.

I was not employed at Genesys as a software developer, formal people manager, or dedicated implementation consultant.

### What I'm good at

- Production diagnosis across distributed enterprise systems
- Customer-facing technical investigation and escalation
- CX platform internals: routing, knowledge, digital channels, conversational AI, agent applications
- API and integration troubleshooting
- Translating operational and deployment constraints into technical requirements
- Cross-team coordination with Product, Engineering, and customer operations

## Independent engineering work (since late 2024)

Since leaving Genesys I have been extending that enterprise background through independent applied-AI engineering under [Keystone Applied Intelligence](https://github.com/getkeystone), a Canadian sole proprietorship.

This work builds practical systems and evaluates them against their own evidence. It is a differentiator extending my professional experience, not a replacement for it.

### What I've built

- **Python, FastAPI, Pydantic, and REST APIs** — governed retrieval and conversational services
- **PostgreSQL FTS + pgvector hybrid retrieval** — lexical and vector search with deterministic reranking
- **Authorization-aware retrieval** — role-based access control, client isolation, and document classification filters enforced at the database layer, including a cross-client isolation defect found, fixed, and covered by regression tests
- **Evidence thresholds, citations, and refusal** — fail-closed behavior when retrieved evidence is insufficient
- **Conversational workflows** — structured task state, escalation, human handoff, and intent classification
- **Evaluation infrastructure** — endpoint-agnostic harness with declarative assertions, retained evaluation runs, and regression lineage ([keystone-verify](https://github.com/getkeystone/keystone-verify), [keystone-ledger](https://github.com/getkeystone/keystone-ledger))
- **OpenTelemetry instrumentation** — GenAI model, token, latency, and HTTP spans delivered to Grafana Tempo
- **Docker, Linux, local inference through Ollama** — customer-infrastructure-first deployment

### Key repositories

| Repository | What it demonstrates |
|---|---|
| [keystone-gov](https://github.com/getkeystone/keystone-gov) | Governed RAG: hybrid retrieval, role-based ACL, evidence thresholds, factual consistency scoring, HMAC audit trail |
| [keystone-engage](https://github.com/getkeystone/keystone-engage) | Governed conversational agent: authorization, escalation routing, intent classification, fail-closed refusal |
| [keystone-counsel](https://github.com/getkeystone/keystone-counsel) | Authorization-first retrieval: role × classification × client isolation for regulated content |
| [keystone-verify](https://github.com/getkeystone/keystone-verify) | Standalone evaluation harness: declarative assertions over HTTP endpoints |
| [keystone-ledger](https://github.com/getkeystone/keystone-ledger) | Retained evaluation artifacts: passing and failing runs, remediation lineage |
| [Support Operations Intelligence](https://github.com/arnaldosepulveda/support-operations-intelligence) | Evidence-driven operational analysis: 7.47M Calgary 311 records, reproducible baselines, 218-test suite |

These are separate reference implementations and research projects. They are not one integrated production platform and do not represent client engagements.

### Evaluation evidence

A retained internal evaluation of keystone-core/agent-v1 exercised 186 cases across 12 categories and 558 executions, with 153 strict passes, 33 characterization cases, and 0 strict failures at the evaluated keystone-gov commit. The retained artifacts are in [`keystone-ledger/artifacts/kdat-002d/`](https://github.com/getkeystone/keystone-ledger/tree/main/artifacts/kdat-002d).

A preceding run (agent-v0) found 9 failures traced to 4 implementation defects, which were fixed before agent-v1. Both runs are retained.

These results are bound to the evaluated commits, configurations, datasets, and runs. A passing internal run is not independent validation or evidence of universal correctness.

### Community pilot

A role-aware knowledge-access prototype was used by a small group at a volunteer fire department. This was a limited real-user pilot, not an organization-wide deployment or a measured operational improvement.

## Education

BScE and MScE in Electrical Engineering, University of New Brunswick. Graduate research applied machine learning, optimization, and predictive control to aggregated electrical loads using smart-meter data.

## Links

- [LinkedIn](https://www.linkedin.com/in/arnaldosepulveda/)
- [Personal site](https://arnaldosepulveda.com/)
- [Keystone Applied Intelligence](https://getkeystone.ai/) · [GitHub](https://github.com/getkeystone)
- [Support Operations Intelligence](https://github.com/arnaldosepulveda/support-operations-intelligence)
- [Contact](mailto:arnaldo@getkeystone.ai)

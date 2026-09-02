# Arnaldo Sepulveda

**AI Engineer & Builder working across production AI, conversational AI, RAG, evaluation, and enterprise contact-center systems.**

I spent more than 12 years at Genesys working on enterprise contact-center systems. Since late 2024, I have applied that operational foundation to hands-on AI engineering through Keystone Applied Intelligence.

## What I build

I build production-oriented AI systems and engineering instruments, including:

* Python, FastAPI, Pydantic, and REST services
* PostgreSQL and pgvector
* PostgreSQL full-text search and hybrid retrieval
* deterministic procedural reranking
* RAG with citations and evidence thresholds
* conversational workflows
* authorization-aware retrieval
* endpoint-agnostic evaluation harnesses and regression tests
* OpenTelemetry GenAI and HTTP tracing
* local model execution

The emphasis is practical: understand the operational problem, build something useful, evaluate it, find its failure modes, and improve it using evidence and real use.

## Why this work

In enterprise support, I repeatedly saw organizations reconstruct answers they already possessed. The knowledge was fragmented across tickets, documentation, internal discussions, and individual experts, making the right answer difficult to retrieve in the right context.

The organization already possessed the knowledge, but had not operationalized it so the right person could reliably get the right answer in the right context.

Applied AI can reduce that repeated reconstruction. The goal is not to replace experienced support engineers, but to make existing organizational knowledge more usable so they can focus on novel, ambiguous, and higher-value problems.

**[The knowledge was already there. The system to use it was not.](https://arnaldosepulveda.com/writing/the-knowledge-was-already-there/)**

## Current work: Keystone Applied Intelligence

[Keystone Applied Intelligence](https://getkeystone.ai/) is my independent AI engineering and R&D practice. I use it to build and evaluate retrieval systems, conversational workflows, APIs, observability, and bounded runtime controls.

Current implementation work includes:

* Python, FastAPI, Pydantic, and REST APIs
* PostgreSQL FTS + pgvector hybrid retrieval
* deterministic reranking
* citations and evidence thresholds
* authorization-first retrieval
* conversational AI workflows
* evaluation and regression infrastructure
* OpenTelemetry tracing with GenAI model, token, latency, and HTTP spans delivered to Grafana Tempo
* local inference through Ollama

The public projects are separately composed engineering instruments. They are not evidence of one complete demonstrated production runtime.

In [Keystone Engage](https://github.com/getkeystone/keystone-engage), the default served application uses one orchestrator. A separate experimental path implements five specialist agent identities across four coordination phases. NATS JetStream integration is optional and experimental, not evidence of distributed production deployment. The repositories do not establish production high availability, durable agent leases, fencing, or platform-wide Prometheus metrics.

Selected links:

* [Keystone website](https://getkeystone.ai/)
* [Live demo](https://demo.getkeystone.ai/)
* [Keystone GitHub organization](https://github.com/getkeystone)
* [Keystone Engage](https://github.com/getkeystone/keystone-engage)
* [Keystone Counsel](https://github.com/getkeystone/keystone-counsel)
* [Keystone Verify](https://github.com/getkeystone/keystone-verify)
* [Keystone evaluation ledger](https://github.com/getkeystone/keystone-ledger)

## Enterprise engineering background

I spent more than 12 years at Genesys across enterprise contact-center, hybrid, and cloud environments. Within the Business Applications organization, I specialized in Knowledge, AI and classification, Digital Services, Agent Workspace, and customer and interaction data.

My work included:

* Genesys Knowledge Center
* Classification Server, Training Server, and Content Analyzer
* Digital Services and Agent Workspace
* Universal Contact Server and customer/interaction data
* routing and conversational systems
* implementations, migrations, and go-lives
* distributed troubleshooting and enterprise integrations
* customer-facing technical investigations
* high-severity production incidents

I troubleshot WFM-integrated agent and supervisor workflows and operational statistics in production, tracing missing or incorrect data across Workspace, Interaction Server, and adjacent application/data layers to isolate failure domains and drive resolution across product boundaries. I was not the dedicated WFM forecasting or planning SME.

I worked directly with product managers, developers, and technical directors on product behavior, supportability, customer requirements, and deployment architecture, including clustered and high-volume customer/interaction-data deployments. I later led the Genesys Cloud CX UI Support Team.

That experience taught me to treat routing, state, observability, failure recovery, escalation, and cross-component diagnosis as core engineering concerns. My classification and conversational-systems work at Genesys preceded modern LLM and generative-AI systems.

## Evaluation

Evaluation is part of the engineering loop, not a final marketing checkpoint.

Current retained internal evidence includes:

* endpoint-agnostic evaluation tooling
* 186 cases across 12 categories
* 558 executions
* adversarial authorization testing
* preserved failing and passing runs
* regression evidence after remediation
* implementation defects surfaced through evaluation

These results are bound to the evaluated commits, configurations, datasets, and runs. A passing internal run is not independent validation or evidence of universal correctness.

[Review the retained evaluation lineage and artifacts.](https://github.com/getkeystone/keystone-ledger)

## Secondary research: Governed Execution

**Governed Execution** is a secondary research program behind my applied engineering work. It studies runtime governance for consequential AI actions.

> **Orchestration determines how work proceeds. Governance determines whether the intended consequence remains justified to proceed.**

The working architecture separates:

* a **control plane** for authority, policy, admissibility, placement, budget, and release
* an **execution plane** for models, retrieval, tools, delegation, and workflows
* an **evidence plane** for decisions, authorizations, actions, evaluations, failures, and outcomes
* a separate **action boundary** for external consequence

The program also examines six candidate runtime dimensions:

* Identity
* Task state
* Tempo
* Cost
* Currency
* Fidelity

These dimensions are research hypotheses, not a complete ontology or a claim of complete AI governance coverage.

### Track A: Runtime Validity

[Runtime Validity](https://github.com/getkeystone/runtime-validity) is a bounded Track A reference implementation.

Current evidence supports only a controlled process-local authority change that can be retained as transition evidence and, under full revalidation, alter the implemented outcome from `PROCEED` / `MATCH` to `HOLD` / `MISMATCH`.

It does not establish authentic external revocation, production authentication or authorization, independent witness evidence, durable persistence guarantees, external consequence enforcement, distributed correctness, or universal validity of the broader Governed Execution architecture.

## Earlier research

I completed an MScE in Electrical Engineering at the University of New Brunswick. My research applied machine learning, optimization, and predictive control to aggregated electrical loads using smart-meter data.

Official thesis title: [*Soft computing methods for the implementation of aggregated load control of domestic electric water heaters*](https://unbscholar.lib.unb.ca/items/43166071-7869-4770-887d-4adb63fe8104).

## Current stack

**AI / Retrieval**

Python · FastAPI · PostgreSQL · pgvector · PostgreSQL full-text search · RAG · hybrid retrieval · embeddings · Ollama

**Evaluation / Observability**

evaluation harnesses · regression testing · OpenTelemetry · Grafana Tempo

**Application / Infrastructure**

Docker · Linux · React · TypeScript · NATS JetStream (experimental/optional)

## Public work

* [Personal site](https://arnaldosepulveda.com/)
* [Writing](https://arnaldosepulveda.com/writing/)
* [Keystone Applied Intelligence](https://getkeystone.ai/)
* [Live demo](https://demo.getkeystone.ai/)
* [Keystone GitHub](https://github.com/getkeystone)
* [Keystone Verify](https://github.com/getkeystone/keystone-verify)
* [Evaluation ledger](https://github.com/getkeystone/keystone-ledger)
* [Runtime Validity](https://github.com/getkeystone/runtime-validity)
* [LinkedIn](https://www.linkedin.com/in/arnaldosepulveda/)
* [Contact](mailto:arnaldo@getkeystone.ai)

## Working principle

Build the control.

Test the control.

Preserve the failure.

Limit the claim to what the evidence supports.

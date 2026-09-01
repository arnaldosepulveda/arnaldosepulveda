# Arnaldo Sepulveda

**AI Systems Engineer with 14+ years in enterprise technology, including more than 12 years at Genesys, now building and evaluating modern retrieval and agent systems.**

My background connects enterprise contact-center engineering with hands-on AI development in Python, FastAPI, structured APIs, RAG, hybrid retrieval, agent workflows, evaluation, and observability.

## Engineering background

At **Genesys**, I worked within the Business Applications team across customer implementations, product-fitness investigations, migrations, go-lives, and production incidents.

I specialized in:

* Knowledge
* AI and classification
* Digital Services and eServices
* Agent Workspace

My product SME experience included:

* Genesys Knowledge Center
* Classification Server
* Training Server
* Universal Contact Server

The work required direct collaboration with customers, product managers, developers, and engineering teams across on-premises, hybrid, and cloud contact-center environments. That experience with knowledge systems, routing, state, escalation, integration, and production diagnostics shapes how I build AI systems today.

## Current AI engineering

My current work includes:

* Python, FastAPI, Pydantic, and structured APIs
* RAG, chunking, embeddings, and evidence-aware generation
* PostgreSQL full-text search and pgvector hybrid retrieval
* deterministic procedural reranking
* agent workflows and explicit state machines
* evaluation harnesses and regression testing
* observability instrumentation, including OpenTelemetry where implemented

I develop this work through **Keystone Applied Intelligence**, an independent engineering and R&D practice and reference implementation environment. Keystone is not presented as a universal governance platform. Its public repositories distinguish default served paths from experimental, feature-flagged, configured, and planned components.

## Selected public work

### Keystone Gov

A FastAPI RAG reference implementation with PostgreSQL full-text search, pgvector hybrid retrieval, query-time ACL filtering, deterministic procedural reranking, HHEM as an additional factual-consistency signal, and retained internal evaluation evidence.

[Repository](https://github.com/getkeystone/keystone-gov) | [Documentation](https://docs.getkeystone.ai/)

### Keystone Engage

A conversational-agent reference implementation whose default served path uses one `EngageOrchestrator`. An experimental five-phase coordinator is available through an alternate entry point behind a feature flag. OpenTelemetry instrumentation is wired in code; optional NATS JetStream integration belongs to the experimental path.

[Repository](https://github.com/getkeystone/keystone-engage)

### Keystone Verify

Deterministic, endpoint-agnostic tooling for testing HTTP responses against declarative assertions and retaining structured JSON results. The output is inspectable evaluation evidence, not cryptographically sealed proof.

[Repository](https://github.com/getkeystone/keystone-verify)

### Runtime Validity

**Runtime Validity** is a bounded reference implementation within the broader **Governed Execution** research and engineering program. It is identified as Track A in the research program.

The current implementation shows only that a controlled process-local authority change can be retained as transition evidence and, under full revalidation, can change the implemented result from `PROCEED` / `MATCH` to `HOLD` / `MISMATCH`. With `revalidation_mode="none"`, authority is `NOT_EVALUATED`; proceeding in that mode is not evidence that the intended consequence remains justified.

It does not establish authentic external revocation, production authorization, independent witness evidence, durable persistence, structural decision-to-transition binding, or external consequence enforcement.

[Repository](https://github.com/getkeystone/runtime-validity)

## Governed Execution

**Governed Execution** is the umbrella research and engineering program. Its controlling architecture is *Governed Execution as a Runtime Contract: A Substrate Architecture for Agentic AI*, v4.4.

The architecture distinguishes three planes:

* Control
* Execution
* Evidence

It also defines a separate action boundary.

The core distinction is:

> Orchestration determines how work proceeds. Governance determines whether the intended consequence remains justified to proceed.

The architecture and its candidate runtime dimensions are research hypotheses. They are not claims of complete AI governance coverage or a complete composed runtime.

## Evaluation discipline

Keystone's published evaluation results are internal evaluations bound to specific commits, configurations, datasets, and runs. They are not independent or third-party validation.

The retained ledger includes passing and failing runs, known limitations, remediation history, and cases where re-verification remains outstanding.

[Internal evaluation ledger](https://github.com/getkeystone/keystone-ledger)

## Earlier research

I completed an MScE in Electrical Engineering at the University of New Brunswick. My thesis, *Soft Computing Methods for Aggregated Load Control Using Smart Meters*, applied machine learning, optimization, and predictive control to aggregated electrical loads using smart-meter data.

Research is a differentiator behind my engineering work, especially in evaluation and runtime systems, rather than my primary professional positioning.

## Links

* [Personal site](https://arnaldosepulveda.com)
* [Keystone Applied Intelligence](https://getkeystone.ai)
* [Keystone documentation](https://docs.getkeystone.ai/)
* [LinkedIn](https://www.linkedin.com/in/arnaldosepulveda)
* [Email](mailto:arnaldo@getkeystone.ai)

## Working principle

Build the control.

Test the control.

Preserve the failure.

Limit the claim to what the evidence supports.

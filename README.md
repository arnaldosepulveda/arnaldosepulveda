# Arnaldo Sepulveda

**AI Systems Engineer developing governed agent systems and a research program on runtime governance for consequential AI actions.**

I build and evaluate AI systems for environments where generating a useful answer is not enough.

The system must also be able to answer questions such as:

* Who is authorized to act?
* What task is actually being performed?
* Which evidence supports the result?
* What changed during execution?
* Does an earlier authorization still justify the intended consequence?
* What happens when authority, evidence, policy, or execution state changes?
* Can an external reviewer reconstruct why the system proceeded, held, denied, or escalated?

My current engineering and research work is through **Keystone Applied Intelligence**, an independent engineering and R&D practice focused on governed retrieval, agent execution, evaluation, runtime evidence, and technical governance.

---

## Current work

### Keystone Applied Intelligence

Keystone develops AI systems and research infrastructure for regulated and higher-consequence environments.

Current engineering work includes:

* authorization-first retrieval
* fail-closed evidence handling
* explicit task lifecycle state
* agent and runtime identity
* event-driven coordination
* hash-chained audit records
* reproducible agent and retrieval evaluation
* OpenTelemetry-based AI observability
* local-first model execution

The current platform architecture is designed for operator-controlled infrastructure and does not require an external model API for core functionality.

### Governed Execution

Within Keystone, I am developing **Governed Execution**, a runtime-governance research program and reference platform for autonomous and semi-autonomous AI systems.

The architecture separates:

* a **control plane** for authority, policy, admissibility, placement, budget, and release
* an **execution plane** for models, retrieval, tools, delegation, and workflows
* an **evidence plane** for decisions, authorizations, actions, evaluations, failures, and outcomes
* a separate **action boundary** governing whether model or agent output may create external consequence

The individual research tracks are deliberately narrow. Each isolates a governance question so its assumptions, implementation, failure modes, and evidence can be examined before broader integration.

### Track A: Runtime Validity

The first public track is:

**[Track A Runtime Validity](https://github.com/getkeystone/track-a-runtime-validity)**

Track A studies runtime validity and revalidation of prior governance decisions before consequential action.

The current implementation can compare an authority obligation attached to a prior decision against separately sourced runtime authority state, produce `MATCH`, `MISMATCH`, or `NOT_EVALUATED` evidence, return `PROCEED` or `HOLD`, and retain the resulting decision record for retrieval.

It is a bounded reference implementation, not evidence that the broader governance architecture is complete or validated.

---

## Evaluation

I treat evaluation as part of the system rather than a final benchmark.

Current Keystone evaluation work includes:

* 186 cases across 12 categories
* 558 executions
* adversarial authorization testing
* fail-closed retrieval tests
* preserved failing and passing runs
* regression evidence after remediation

The evaluation process has surfaced real implementation defects.

That is intentional.

A useful evaluation system should be capable of showing where its own implementation fails.

---

## Research

My current working manuscript is:

**Governed Execution as a Runtime Contract: A Substrate Architecture for Agentic AI**

The research starts from a systems distinction:

> Model capability and execution governance are different problems.

Agentic systems retrieve data, call tools, delegate work, wait, retry, consume resources, maintain durable state, and create external consequences.

Those behaviors introduce governance questions that cannot be resolved solely through prompts or model evaluation.

The manuscript proposes six **candidate** runtime substrate dimensions:

* Identity
* Task state
* Tempo
* Cost
* Currency
* Fidelity

These are research hypotheses and a candidate representation, not a claim that six dimensions form a complete ontology or theory.

My current narrow research question is:

> Which runtime changes make a prior governance decision stale or otherwise invalid, what should trigger revalidation before consequential action, and what evidence should let an external reviewer reconstruct why the resulting action proceeded, was held, denied, or escalated?

Current candidate classes of governance-material change include:

* Authority
* Governance / policy
* Evidence
* Target / environment
* Interface / tool
* Execution state

That taxonomy is also a hypothesis to test.

---

## Engineering background

Before Keystone, I spent more than 12 years at **Genesys** working on enterprise contact-center and cloud systems across on-premises, hybrid, and cloud environments.

The work involved direct technical collaboration with customer engineers, DBAs, developers, deployment teams, and technical managers.

Areas included:

* SIP and voice infrastructure
* contact-center routing
* desktop and digital channels
* knowledge retrieval
* conversational systems
* cloud migration
* distributed troubleshooting
* production incident response
* enterprise integrations

Later work included Knowledge Center retrieval, conversational-AI workflows, Cloud CX support, digital channels, and complex cross-component production diagnostics.

That systems background strongly influences how I approach AI agents.

Identity, state, routing, authorization, escalation, deadlines, capacity, recovery, and auditability were production engineering concerns long before LLM agents appeared.

---

## Earlier research

I completed an MScE in Electrical Engineering at the University of New Brunswick.

My research applied machine learning, optimization, and predictive control to aggregated electrical loads using smart-meter data.

**Thesis:**  
*Soft Computing Methods for Aggregated Load Control Using Smart Meters*

That work combined machine learning with constrained execution and control, themes that continue to influence my current systems work.

---

## Current stack

**AI / Agent Systems**

Python · FastAPI · PostgreSQL · pgvector · Ollama · RAG · agent orchestration · evaluation harnesses · embeddings · vector search

**Infrastructure**

Docker · NATS JetStream · Linux · Caddy · Tailscale

**Observability**

OpenTelemetry · Grafana · Tempo · Prometheus

**Frontend**

React · TypeScript

**Research / Governance**

Runtime governance · authorization · evaluation · audit evidence · fail-closed systems · provenance · human oversight · material-change revalidation · governance-decision reconstruction

---

## Current interests

* AI systems engineering
* Agentic systems
* Governed retrieval
* Runtime authorization
* Runtime governance
* Agent evaluation
* Runtime evidence and auditability
* Governance-decision reconstruction
* Material-change and revalidation rules
* Distributed agent execution
* Local-first AI infrastructure
* AI systems for regulated environments

---

## Public work

**Track A: Runtime Validity**  
https://github.com/getkeystone/track-a-runtime-validity

**Keystone Applied Intelligence**  
https://getkeystone.ai

**Architecture and documentation**  
https://docs.getkeystone.ai

**Keystone Verify**  
https://github.com/getkeystone/keystone-verify

**Evaluation ledger**  
https://github.com/getkeystone/keystone-ledger

**Keystone GitHub organization**  
https://github.com/getkeystone

**LinkedIn**  
https://www.linkedin.com/in/arnaldosepulveda

**Contact**  
[arnaldo@getkeystone.ai](mailto:arnaldo@getkeystone.ai)

---

## Working principle

Build the control.

Test the control.

Preserve the failure.

Limit the claim to what the evidence supports.

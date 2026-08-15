# Arnaldo Sepulveda

**AI Systems Engineer and Independent Researcher working on technical governance of agentic systems.**

I build and study AI systems for environments where generating a useful answer is not enough.

The systems I am interested in must also answer:

* Who is authorized to act?
* What task is actually being performed?
* Which evidence supports the result?
* What changed during execution?
* Should an earlier authorization still be valid?
* What happens when evidence or authorization becomes insufficient?
* Can someone reconstruct why the system proceeded, refused, held, or escalated?

My current engineering and research work is through **Keystone Applied Intelligence**, an independent engineering and R&D practice focused on governed retrieval, agent execution, evaluation, and runtime evidence.

---

## Current work

### Keystone Applied Intelligence

Keystone is an experimental platform for governed AI systems in regulated and higher-consequence environments.

Current implementation work includes:

* authorization-first retrieval,
* fail-closed evidence handling,
* explicit task lifecycle state,
* agent and runtime identity,
* event-driven coordination,
* hash-chained audit records,
* reproducible agent and retrieval evaluation,
* OpenTelemetry-based AI observability,
* local-first model execution.

The core platform runs on customer-controlled infrastructure without requiring an external model API for core functionality.

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

The evaluation process has surfaced real defects in the systems being tested.

That is intentional.

A useful evaluation system should be capable of proving its own implementation wrong.

---

## Research

My current working manuscript is:

**Governed Execution as a Runtime Contract: A Substrate Architecture for Agentic AI**

The paper starts from a systems-engineering observation:

> Model capability and execution governance are different problems.

Agentic systems retrieve data, call tools, delegate work, wait, retry, consume resources, and create external consequences. Those behaviors introduce governance questions that cannot be solved solely through prompts or model evaluation.

The manuscript proposes six **candidate** runtime substrate dimensions:

* Identity
* Task state
* Tempo
* Cost
* Currency
* Fidelity

These are hypotheses about durable properties of governed execution, not a claim that six dimensions form a complete theory.

My current research question has narrowed further:

> Which runtime changes should invalidate a prior governance decision, what should trigger revalidation, and what evidence should allow an external reviewer to reconstruct why the resulting action proceeded, was held, denied, or escalated?

I am currently treating authority, governance, evidence, target/environment, interface, and execution state as candidate classes of governance-material change.

The taxonomy itself is something to test.

---

## Before Keystone

I spent 12 years at **Genesys** working on enterprise contact-center and cloud systems across on-premises, hybrid, and cloud environments.

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

That background strongly influences how I approach AI agents today.

Identity, state, routing, authorization, escalation, deadlines, capacity, recovery, and auditability were production requirements long before LLM agents appeared.

---

## Earlier research

Before Genesys, I completed an MScE in Electrical Engineering at the University of New Brunswick.

My research applied machine learning, optimization, and predictive control to aggregated electrical loads using smart-meter data.

**Thesis:**
*Soft Computing Methods for Aggregated Load Control Using Smart Meters*

That work established an early connection between machine learning and constrained execution that continues to influence how I think about AI systems.

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

Runtime governance · authorization · evaluation · audit evidence · fail-closed systems · provenance · human oversight · technical AI governance

---

## What I am interested in

* Technical governance of agentic systems
* Governed retrieval
* Runtime authorization
* Agent evaluation
* Runtime evidence and auditability
* Governance-decision reconstruction
* Material-change and revalidation rules
* Distributed agent execution
* Local-first AI infrastructure
* AI systems for regulated environments

---

## Public work

**Keystone website**
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

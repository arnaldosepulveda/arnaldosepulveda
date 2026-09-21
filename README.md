# Arnaldo Sepulveda

**Digital Transformation | Enterprise Workflows | Applied AI**

I work at the intersection of operational problem solving, enterprise workflows, customer-facing technology, analytics, automation, and Applied AI.

I spent more than 12 years at Genesys working directly with enterprise customers across Technical Support, Escalations, implementations, migrations, knowledge systems, routing, conversational systems, customer and interaction data, and cloud and hybrid environments.

That work repeatedly required the same pattern:

```text
understand how work happens today
        ->
identify constraints, failure points, and repeated effort
        ->
gather requirements
        ->
separate symptoms from causes
        ->
evaluate possible interventions
        ->
implement and test changes
        ->
support rollout and adoption
        ->
observe what improved and what did not
```

Since late 2024, through Keystone Applied Intelligence and related applied work, I have extended that background into AI-enabled workflows, operational analysis, retrieval systems, evaluation, and runtime governance research.

My current work starts with a question upstream of implementation:

> **What is actually constraining the operation, what evidence supports that conclusion, and what intervention is justified?**

The answer may be process redesign, better knowledge access, integration, workflow automation, deterministic software, analytics, Applied AI, or no intervention until stronger evidence exists.

AI is a tool in that process, not the starting assumption.

---

## Current applied work: Support Operations Intelligence

[Support Operations Intelligence](https://github.com/arnaldosepulveda/support-operations-intelligence) is an evidence-driven portfolio and research project examining how operational evidence can support workflow diagnosis and intervention selection.

The intended sequence is:

```text
operational evidence
        ->
baseline
        ->
competing explanations
        ->
workflow understanding
        ->
diagnosis
        ->
intervention selection
        ->
implementation
        ->
evaluation
        ->
workflow outcome
        ->
business outcome
```

The project deliberately separates:

- what the source actually says
- what can be defensibly derived
- what remains unavailable
- what is simulated
- what would require additional evidence
- what has been implemented
- what has actually been evaluated

The objective is not to add AI to an operation by default.

It is to determine whether a problem is real and material, understand what is causing it, establish what simpler alternatives can achieve, and then evaluate whether an intervention improves the intended workflow.

### Calgary 311 evidence work

Current empirical work uses a 7.47-million-record Calgary 311 artifact.

The current stage is deliberately limited to source and evidence establishment.

Completed work includes:

- reproducible ingestion and full-artifact execution
- structural and identifier validation
- descriptive source-native baselines
- deterministic missingness and sentinel checks
- controlled source-quality review procedures
- retained engineering and evaluation artifacts

This work has not established:

- an end-to-end Calgary 311 operational workflow model
- a diagnosed service-performance problem
- an intervention priority
- an AI intervention
- a before-and-after improvement
- a business outcome
- a production deployment

The purpose of this stage is to establish what the evidence can support before making operational claims.

---

## Applied transformation example: fire-department knowledge workflow

A volunteer fire department had a practical knowledge-access problem: procedures and operational documentation existed, but firefighters could spend unnecessary time locating the right information during training, truck work, maintenance, and other internal activities.

I worked from the operational problem through implementation:

```text
knowledge-access problem
        ->
understand user need and document environment
        ->
define retrieval and access requirements
        ->
design the workflow
        ->
build and test
        ->
deploy on-premises
        ->
support firefighter use
        ->
observe operational feedback
```

The resulting workflow uses role-aware retrieval to help firefighters find relevant procedures and documentation more quickly.

Because some source material relates to operational and medical procedures, the workflow uses evidence thresholds and can withhold an answer when retrieved evidence is insufficient rather than presenting low-confidence output as authoritative.

Firefighters have used the system during internal departmental activities including training, truck work, and maintenance.

This is a bounded internal operational deployment. It does not establish clinical validation, independent safety validation, enterprise high availability, or suitability outside the department and use case in which it is being used.

---

## Enterprise systems and transformation background

I spent more than 12 years at Genesys across enterprise contact-center, on-premises, hybrid, and cloud environments.

Within the Business Applications organization, I specialized in areas including:

- Knowledge systems
- Classification Server and Training Server
- Digital Services
- Agent Workspace
- customer and interaction data
- routing
- conversational systems
- operational statistics
- enterprise integrations

### Customer discovery and requirements

As a product SME, I worked directly with enterprise customers, including onsite engagements, to understand:

- existing workflows
- operational constraints
- deployment requirements
- integration dependencies
- scale and availability requirements
- desired application behavior

I translated those findings into technical requirements, customization decisions, deployment architectures, and implementation guidance.

This included work around multi-node customer and interaction data environments, Knowledge deployments, integrations, and hybrid transitions.

### Cloud and hybrid transitions

I supported customers moving from on-premises environments toward hybrid and cloud architectures.

That work required understanding the existing environment, gathering constraints, defining target requirements, validating integrations, supporting migrations, and helping stabilize systems after transition.

### Workflow automation and routing

Genesys platforms included routing and workflow capabilities that could respond to events, schedules, business rules, integrations, and API-driven conditions.

I designed and configured workflows and automations within those platform capabilities, including operational routing behavior and integrations between systems.

Within Support, I also participated in redesigning case-routing behavior during a ticketing-system transition.

The previous process depended more heavily on analysts manually selecting work from queues.

The revised workflow moved toward automated assignment based on factors such as severity and impact, while allowing lower-risk work to support developing analysts and moving higher-impact escalations more rapidly toward experienced specialists.

### Knowledge and self-service

A recurring operational problem was repeated dependence on subject-matter experts for questions whose answers already existed.

I created and maintained technical knowledge, troubleshooting documentation, tutorials, and internal training material so support engineers could find known answers without repeatedly waiting for an expert to respond.

This experience is one of the reasons my current work focuses heavily on operationalizing organizational knowledge rather than merely generating new text.

### Training and enablement

I developed and delivered internal training, presentations, tutorials, and technical documentation for support engineers and junior staff.

Topics included product behavior, architecture, troubleshooting methods, multi-node deployments, application interactions, and the products for which I served as SME.

I later led the Genesys Cloud CX UI Support Team and mentored engineers on structured troubleshooting, documentation, technical communication, and escalation practices.

### Production operations

I owned and supported high-severity enterprise production problems across North America, Latin America, and EMEA.

The work frequently crossed:

- cloud services
- routing
- digital channels
- agent applications
- APIs
- customer and interaction data
- integrations
- middleware
- databases
- customer infrastructure
- product boundaries
- organizational boundaries

The core task was often not simply fixing a component.

It was establishing what was actually happening, identifying the failure domain, coordinating the appropriate people, validating the change, and restoring the customer workflow.

---

## Conversational AI before generative AI

My experience with conversational and classification systems predates modern LLM systems.

At Genesys I worked with production systems involving:

- intent classification
- text classification
- model-training workflows
- category tuning
- dialog behavior
- confidence thresholds
- slot validation
- escalation
- human handoff
- routing
- compliance logging

I do not present those systems as equivalent to modern LLM applications.

They are relevant because they provided earlier experience with production AI behavior, confidence, routing, human escalation, and the operational consequences of imperfect automated decisions.

---

## Keystone Applied Intelligence

[Keystone Applied Intelligence](https://getkeystone.ai/) is my independent engineering and R&D practice.

It provides the technical implementation side of my current work.

I use Keystone to build and evaluate mechanisms involving:

- retrieval and RAG
- conversational workflows
- authorization-aware retrieval
- evaluation and regression testing
- task state
- observability
- local model execution
- bounded runtime controls

The public Keystone projects are separate engineering instruments.

They are not evidence of one complete demonstrated production runtime, and mechanisms demonstrated in one workload are not automatically attributed to another.

Selected work includes:

- [Keystone Gov](https://github.com/getkeystone/keystone-gov)
- [Keystone Engage](https://github.com/getkeystone/keystone-engage)
- [Keystone Counsel](https://github.com/getkeystone/keystone-counsel)
- [Keystone Verify](https://github.com/getkeystone/keystone-verify)
- [Keystone Ledger](https://github.com/getkeystone/keystone-ledger)

---

## Applied AI engineering

My current implementation work includes:

### AI and retrieval

Python · FastAPI · Pydantic · PostgreSQL · pgvector · PostgreSQL full-text search · RAG · hybrid retrieval · embeddings · Ollama

### Evaluation and observability

Evaluation harnesses · regression testing · structured run artifacts · OpenTelemetry · Grafana Tempo

### Application and infrastructure

REST/HTTP APIs · Docker · Linux · Git · React · TypeScript

I also have limited hands-on exposure to Power Automate, Power Apps, Copilot, and Azure AI Foundry and am developing broader competency in enterprise automation and AI tooling.

The engineering objective is not to maximize architectural complexity.

It is to build the smallest intervention that can be tested against the operational problem.

---

## Evaluation discipline

Evaluation is part of the engineering loop, not a final demonstration step.

Current Keystone evaluation work includes:

- declarative evaluation cases
- deterministic assertions
- endpoint-agnostic testing
- adversarial authorization cases
- preserved failing runs
- remediation lineage
- regression evidence
- latency measurement
- structured run artifacts

A retained internal evaluation of `keystone-core/agent-v1` exercised:

- 186 cases
- 12 categories
- 558 executions
- 153 strict-pass cases
- 33 characterization cases
- 0 strict failures at the evaluated commit

The failing predecessor is retained.

Those results apply only to the evaluated commits, configurations, cases, and runs.

They are internal evaluation results, not independent validation or evidence of universal correctness.

[Review the retained evaluation lineage and artifacts.](https://github.com/getkeystone/keystone-ledger)

---

## Secondary research: Governed Execution

**Governed Execution** is a separate research program examining runtime governance for consequential AI actions.

> **Orchestration determines how work proceeds. Governance determines whether the intended consequence remains justified to proceed.**

The working architecture separates:

- a **Control plane** for authority, policy, admissibility, placement, budget, and release
- an **Execution plane** for models, retrieval, tools, delegation, and workflows
- an **Evidence plane** for decisions, authorizations, actions, evaluations, failures, and outcomes
- a separate **action boundary** determining whether output may create external consequence

The research examines candidate runtime dimensions including:

- Identity
- Task state
- Tempo
- Cost
- Currency
- Fidelity

These are research hypotheses rather than a complete ontology or claim of complete AI governance coverage.

### Runtime Validity: Track A

[Runtime Validity](https://github.com/getkeystone/runtime-validity) is a bounded reference implementation and research instrument for Track A.

Current evidence supports only a controlled process-local authority change that can be retained as transition evidence and, under full revalidation, alter the implemented result from `PROCEED / MATCH` to `HOLD / MISMATCH`.

It does not establish authentic external revocation, production authentication or authorization, independent witness evidence, durable persistence, external consequence enforcement, distributed correctness, or universal validity of the broader architecture.

The detailed research framing and current claim boundaries are maintained in the Runtime Validity and Keystone repositories.

---

## Earlier research

I completed an MScE in Electrical Engineering at the University of New Brunswick.

My graduate research applied machine learning, optimization, predictive control, simulation, and smart-meter data to aggregated electrical load control.

Official thesis title:

**Soft computing methods for the implementation of aggregated load control of domestic electric water heaters**

---

## What I am interested in

I am particularly interested in work involving the full path from operational problem to measurable improvement:

```text
discovery
        ->
process and workflow understanding
        ->
requirements
        ->
root-cause analysis
        ->
intervention selection
        ->
implementation
        ->
testing
        ->
deployment
        ->
adoption
        ->
evaluation
```

That may involve AI.

It may also involve process change, enterprise systems, integration, automation, analytics, or a simpler deterministic solution.

The important question is whether the intervention improves the work.

---

## Public work

- [Support Operations Intelligence](https://github.com/arnaldosepulveda/support-operations-intelligence)
- [Personal site](https://arnaldosepulveda.com/)
- [Writing](https://arnaldosepulveda.com/writing/)
- [Keystone Applied Intelligence](https://getkeystone.ai/)
- [Keystone GitHub](https://github.com/getkeystone)
- [Keystone Engage](https://github.com/getkeystone/keystone-engage)
- [Keystone Verify](https://github.com/getkeystone/keystone-verify)
- [Keystone Ledger](https://github.com/getkeystone/keystone-ledger)
- [Runtime Validity](https://github.com/getkeystone/runtime-validity)
- [LinkedIn](https://www.linkedin.com/in/arnaldosepulveda/)
- [Contact](mailto:arnaldo@getkeystone.ai)

---

## Working principle

Understand the operation.

Establish the evidence.

Choose the intervention.

Build only what is justified.

Test what was built.

Preserve failures.

Measure the outcome.

Limit the claim to what the evidence supports.

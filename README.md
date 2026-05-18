## Arnaldo Sepulveda

Enterprise AI engineer. 12+ years at Genesys building infrastructure
and platform systems for regulated and public sector customers.
MScE in Electrical Engineering (AI/ML focus), UNB.

### What I'm building

**Keystone Applied Intelligence** — a governed RAG system designed for regulated industries.
Runs entirely on-premises. No external API dependencies for inference
or embedding.

Core constraints the system enforces:
- Evidence-backed answers tied to specific source documents and sections
- Role-based access control enforced at query time, before results return
- Domain scope guard: pre-retrieval refusal for out-of-corpus queries
- Fail-closed refusal when evidence is insufficient
- Factual consistency scoring on every response
- Hash-chained, tamper-evident audit trail (INSERT-only database role)

### Evaluation baseline (KDAT-001B, 2026-04-11)

| Metric | Result |
|---|---|
| Corpus | 53 Alberta OHS safety documents, 2,674 chunks |
| Retrieval P@1 | 0.75 |
| MRR | 0.79 |
| Adversarial ACL | 8/8 blocked, 0 leaks |
| Fail-closed | 5/6 (83%) — FC-005 remediated 2026-05-17 |
| Audit chain | Intact, immutable |

FC-005 (domain scope failure on TIER greenhouse gas query) remediated 2026-05-17 with a pre-retrieval domain scope guard (v0.5.2-fc005). Validated manually against the KDAT-001B probe set. Sealed re-eval pending KDAT-002.

Eval methodology and ledger: [keystone-kdat](https://github.com/getkeystone/keystone-kdat)

### Stack

Python · FastAPI · PostgreSQL + pgvector · Ollama · React/TypeScript · Docker Compose · Caddy

### Recent (May 2026)

**[governed-incident-agent](https://github.com/arnaldosepulveda/governed-incident-agent)** — Solo build for the AI Tinkerers Generative UI Hackathon, Boston, May 9, 2026. An agentic interface where every tool call is authorized by the user's role and logged to a tamper-evident audit trail. The agent generates different UI depending on what the user is allowed to do. CopilotKit + Next.js.

**[Provana AcuteCare](https://getkeystone.ai/blog/provana-acutecare/)** — Team build at the same hackathon, applying the governed-incident-agent scaffold to acute care medicine. Three protocols (sepsis, stroke, pediatric fever). I contributed the governance layer; teammate built the dynamic clinical UI. The governance architecture moved from workplace safety to medicine with zero structural changes.

### Currently working on

Extending Keystone to governed agentic actions: tool authorization by role,
action audit trails, HITL approval gates, multi-step reasoning with
per-step evidence. Eval target: KDAT-002.

### Links

| Property | URL |
|---|---|
| Personal site | https://arnaldosepulveda.com |
| Project | https://getkeystone.ai |
| Demo | https://demo.getkeystone.ai (operator1 / demo123) |
| Blog | https://getkeystone.ai/blog/ |
| Eval ledger | https://github.com/getkeystone/keystone-kdat |
| LinkedIn | https://linkedin.com/in/arnaldosepulveda |
| Contact | arnaldo@getkeystone.ai |

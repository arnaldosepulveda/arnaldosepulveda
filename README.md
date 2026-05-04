## Arnaldo Sepulveda

Enterprise AI engineer. 12+ years at Genesys building infrastructure
and platform systems for regulated and public sector customers.
MScE in Electrical Engineering (AI/ML focus), UNB.

### What I'm building

**Keystone** — a governed RAG system designed for regulated industries.
Runs entirely on-premises. No external API dependencies for inference
or embedding.

Core constraints the system enforces:
- Evidence-backed answers tied to specific source documents and sections
- Role-based access control enforced at query time, before results return
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
| Fail-closed | 5/6 (83%) |
| Audit chain | Intact, immutable |

Eval methodology and ledger: [keystone-kdat](https://github.com/getkeystone/keystone-kdat)

### Stack

Python · FastAPI · PostgreSQL + pgvector · Ollama · React/TypeScript · Docker Compose · Caddy

### Currently working on

Extending Keystone to governed agentic actions: tool authorization by role,
action audit trails, HITL approval gates, multi-step reasoning with
per-step evidence. Eval target: KDAT-002.

### Links

| | |
|---|---|
| Project | [getkeystone.ai](https://getkeystone.ai) |
| Demo | [demo.getkeystone.ai](https://demo.getkeystone.ai) — log in as `operator1` / `demo123` |
| Eval ledger | [getkeystone/keystone-kdat](https://github.com/getkeystone/keystone-kdat) |
| LinkedIn | [linkedin.com/in/arnaldosepulveda](https://linkedin.com/in/arnaldosepulveda) |
| Contact | arnaldo@getkeystone.ai |

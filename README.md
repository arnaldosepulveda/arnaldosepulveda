# Arnaldo Sepulveda

Senior AI engineer specializing in conversational and retrieval AI under audit pressure. Thirteen years at Genesys building the AI intelligence layer of enterprise contact centers (Knowledge Center retrieval, chat suite, e-services, contact intelligence: the pre-LLM era of conversational AI). MScE in Electrical Engineering with thesis on multi-agent coordination, UNB.

## What I'm building

Keystone Applied Intelligence — a governed retrieval and agent system for regulated industries. Runs entirely on-premises. No external API dependencies for inference or embedding.

Core constraints the system enforces:
- Evidence-backed answers tied to specific source documents and sections
- Role-based access control enforced at query time, before results return
- Domain scope guard: pre-retrieval refusal for out-of-corpus queries
- Fail-closed refusal when evidence is insufficient
- Factual consistency scoring on every response
- Hash-chained, tamper-evident audit trail (INSERT-only database role)

Every architectural decision traces to a documented contact center AI pattern (severity-tier escalation, per-step validation, compliance logging, confidence-threshold refusal) rebuilt for the LLM substrate.

## Evaluation baselines

| Baseline | Description | Cases | Date |
|---|---|---|---|
| keystone-core/agent-v1 (formerly KDAT-002D) | Governed agent extension | 186 cases, 12 categories, 0 fail | 2026-05-20 |
| keystone-core/retrieval-v1 (formerly KDAT-001B) | Governed retrieval | P@1 0.75, MRR 0.79, 8/8 ACL blocked | 2026-04-11 |

FC-005 (domain scope failure on TIER greenhouse gas query) remediated 2026-05-17 with a pre-retrieval domain scope guard (v0.5.2-fc005).

Forward eval lineage uses `keystone-{component}/{type}-v{n}` versioning. Existing keystone-core/retrieval-v1 and keystone-core/agent-v1 remain published as the canonical historical baselines; the migration cross-reference lives in keystone-kdat.

Eval methodology and ledger: keystone-kdat

## Stack

Python · FastAPI · PostgreSQL + pgvector · Ollama · React/TypeScript · Docker Compose · Caddy

## Recent (May 2026)

**governed-incident-agent** — Solo build for the AI Tinkerers Generative UI Hackathon, Boston, May 9, 2026. An agentic interface where every tool call is authorized by the user's role and logged to a tamper-evident audit trail. The agent generates different UI depending on what the user is allowed to do. CopilotKit + Next.js.

**Provana AcuteCare** — Team build at the same hackathon, applying the governed-incident-agent scaffold to acute care medicine. Three protocols (sepsis, stroke, pediatric fever). I contributed the governance layer; teammate built the dynamic clinical UI. The governance architecture moved from workplace safety to medicine with zero structural changes.

## Next

Keystone platform extending into three regulated verticals: governed conversational agents (keystone-engage), regulated content retrieval (keystone-counsel), and standalone evaluation framework (keystone-verify).

## Links

| Property | URL |
|---|---|
| Project | https://getkeystone.ai |
| Demo | https://demo.getkeystone.ai (operator1 / demo123) |
| Blog | https://getkeystone.ai/blog/ |
| Eval ledger | https://github.com/getkeystone/keystone-kdat |
| LinkedIn | https://linkedin.com/in/arnaldosepulveda |
| Contact | arnaldo@getkeystone.ai |

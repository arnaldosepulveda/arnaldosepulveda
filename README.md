# Arnaldo Sepulveda

I build **on-prem AI knowledge infrastructure** for organizations that cannot use cloud AI.

My focus is **governed retrieval**: permission-aware answers with citations, fail-closed behavior when evidence is insufficient, and audit records that stand up in compliance-constrained environments.

Runs fully on customer infrastructure. No external API calls. Air-gap compatible.

## Current Focus: single-machine air-gapped proof (KDAT-001A)

I’m shipping a single-machine demo that runs fully offline and proves:

- Evidence-backed answers with citations
- Fail-closed behavior when evidence is insufficient
- Query-time authorization (users only retrieve what they’re allowed to see)
- Tamper-evident audit records for every query (verifiable chain)
- Reproducible run: same results twice while air-gapped

## Keystone AI

**Keystone AI** is an on-prem knowledge system designed for regulated enterprises:

- No external API calls
- No data exfiltration
- Audit-first by default
- Deployable in air-gapped environments

Target: regulated and compliance-constrained environments where access control and auditability are mandatory.

## What I’m Building

- **Permission-aware retrieval**: enforce access control at retrieval time
- **Multi-source ingestion**: SharePoint, file shares, databases (with ACL fidelity)
- **Audit-grade logging**: query, retrieval, response, and verification artifacts
- **Operational discipline**: runbooks, backup/restore, measurable verification

## Stack (today)

- Python, FastAPI
- PostgreSQL (permissions, sync state, audit log)
- Vector search backend (evolving)
- Ollama (local inference)
- Docker Compose (demo packaging)
- Microsoft Graph API (SharePoint ingestion, OAuth delegation)

## Links

- Keystone AI: https://getkeystone.ai
- GitHub org: https://github.com/getkeystone
- LinkedIn: https://linkedin.com/in/arnaldo-sepulveda
- Contact: arnaldo@getkeystone.ai

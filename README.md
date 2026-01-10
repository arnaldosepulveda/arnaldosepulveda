# Arnaldo Sepulveda

Building on-premise AI knowledge infrastructure for organizations that can't use cloud AI.

## Current Focus

**Keystone AI** — Enterprise RAG platform with query-time authorization and multi-source ingestion.

Core problems I'm solving:
- Permission-aware vector retrieval (users only see content they're authorized to access)
- Multi-source knowledge ingestion with access control inheritance
- Audit logging for compliance frameworks (NIST 800-171, CMMC, HIPAA)
- On-premise deployment patterns for air-gapped and regulated environments

## Technical Stack

**Inference & Embeddings**
- Ollama for local LLM deployment (Qwen2.5, Llama 3)
- BGE-large-en-v1.5 for embeddings
- Multi-GPU inference environments (RTX 3090/3080 class hardware)

**Vector Storage & Retrieval**
- Qdrant for metadata-filtered vector search
- PostgreSQL for permissions, sync state, audit trails
- Query-time authorization with role-based filtering

**API & Integration**
- FastAPI with async processing
- Microsoft Graph API for SharePoint integration (OAuth On-Behalf-Of flow)
- File share monitoring with metadata extraction
- PDF/OCR processing pipelines

**Deployment & Security**
- Docker Compose for service orchestration
- Network segmentation with VLAN isolation
- Encryption at rest, comprehensive audit logging
- Backup/restore runbooks with timed recovery drills

## Background

**12 years at Genesys** deploying enterprise contact center platforms for:
- Defense contractors
- Federal agencies
- Fortune 500 companies

Built production systems handling millions of interactions with strict uptime, security, and audit requirements.

**MScE Electrical Engineering** — AI/ML specialization

## What I'm Building

Enterprise knowledge infrastructure that runs entirely on customer hardware:
- No external API calls
- No data exfiltration
- Complete audit trails
- Role-based content access
- Citation-backed answers

Target deployments: Organizations operating under NIST 800-171, CMMC readiness frameworks, FedRAMP-aligned patterns, HIPAA, SOX.

## Architecture Principles

1. **Query-time authorization** — permission checks at retrieval, not ingestion
2. **Multi-source ingestion** — unified interface across SharePoint, file shares, databases, email
3. **Audit-first design** — every query logged with user, sources, timestamps
4. **Zero external dependencies** — deployable in air-gapped environments
5. **Production-grade operations** — monitoring, alerting, backup/restore

## Contact

🌐 [getkeystone.ai](https://getkeystone.ai)  
📧 arnaldo@getkeystone.ai  
💼 [LinkedIn](https://linkedin.com/in/arnaldo-sepulveda)

---

*Building infrastructure that enables regulated industries to deploy AI without losing data control.*

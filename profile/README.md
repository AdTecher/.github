<div align="center">

# AdTecher

**Enterprise ad-tech platform -- real-time fraud detection, campaign intelligence, and AI-driven optimization for digital advertising.**

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.110+-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Next.js](https://img.shields.io/badge/Next.js-14+-000000?style=flat-square&logo=next.js&logoColor=white)](https://nextjs.org)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15+-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://postgresql.org)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)]()

</div>

---

## Products

| Product | Description | Status |
|---------|-------------|--------|
| **Vulcan** | Enterprise ad analytics API with multi-tenant RLS, real-time fraud scoring, and campaign performance intelligence. Python / FastAPI / PostgreSQL. | Active |
| **Selene AI** | Intelligent ad spend protection system. Monitors 50+ campaign metrics, detects anomalies via ML, and auto-pauses wasteful spend. | Active |
| **KeyTakeAways** | AI-powered Shopify e-commerce analytics dashboard with multi-model chat (Llama 2, Mistral, DeepSeek) and N8N workflow automation. | Active |
| **Canary** | Early-warning system for business opportunity detection via Shopify ecosystem analysis. | Archived |

## Architecture

```
                          AdTecher Platform
  ================================================================

  INGESTION LAYER
  ----------------------------------------------------------------
  [ Meta Ads ]  [ Google Ads ]  [ Shopify ]  [ Custom Sources ]
       |              |              |              |
       v              v              v              v
  +----------------------------------------------------------+
  |                   API Gateway (FastAPI)                   |
  |               JWT Auth  |  Rate Limiting                 |
  +----------------------------------------------------------+

  PROCESSING LAYER
  ----------------------------------------------------------------
       |                    |                    |
  +-----------+   +------------------+   +--------------+
  |  Fraud    |   |  Campaign        |   |  Spend       |
  |  Scoring  |   |  Analytics       |   |  Protection  |
  |  Engine   |   |  Pipeline        |   |  (Selene AI) |
  +-----------+   +------------------+   +--------------+
       |                    |                    |
       v                    v                    v
  +----------------------------------------------------------+
  |              PostgreSQL (Row-Level Security)              |
  |           Multi-Tenant Data Isolation via RLS             |
  +----------------------------------------------------------+

  INTELLIGENCE LAYER
  ----------------------------------------------------------------
  +------------------+   +------------------+   +--------------+
  |  LangGraph       |   |  Groq Inference  |   |  N8N         |
  |  Agent           |   |  (Llama/Mistral) |   |  Workflow    |
  |  Orchestration   |   |                  |   |  Automation  |
  +------------------+   +------------------+   +--------------+
```

## Engineering Standards

- **Type safety enforced** across all codebases (Python type hints, TypeScript strict mode)
- **Row-Level Security** for multi-tenant data isolation at the database layer
- **Conventional commits** and **branch naming conventions** enforced via CI
- **Automated security scanning** with dependency auditing and secrets detection
- **Structured logging** with request-scoped context for full observability

## Contributing

All contributions follow our organization-wide standards. See our [Contributing Guide](https://github.com/AdTecher/.github/blob/main/CONTRIBUTING.md) and [Code of Conduct](https://github.com/AdTecher/.github/blob/main/CODE_OF_CONDUCT.md).

## Security

Report vulnerabilities privately per our [Security Policy](https://github.com/AdTecher/.github/blob/main/SECURITY.md). Do not open public issues for security concerns.

---

<div align="center">

[adtecher.com](https://adtecher.com) | [contact@adtecher.com](mailto:contact@adtecher.com)

</div>

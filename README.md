<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

# Emir Hüseyin İnci

### Rust Systems Engineer · Python Backend · AI Infrastructure · Data & Decision Systems

I build reliable software for teams that need to **control AI costs, automate data workflows, and make high-stakes decisions auditable**.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![Email](https://img.shields.io/badge/Email-Discuss_a_project-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Project%20inquiry)

</div>

## Problems I help solve

- **AI cost and policy control:** model routing, budget enforcement, fallback rules, guardrails, usage attribution, and audit evidence.
- **High-integrity backend systems:** deterministic decision services, replayable workflows, tamper-evident logs, concurrency-safe accounting, and low-latency Rust APIs.
- **Data engineering and automation:** scraping pipelines, CSV/Excel cleanup, validation contracts, scheduled jobs, API integrations, and client-ready reports.
- **Decision-focused machine learning:** calibrated risk scores, uplift modeling, explainability, counterfactuals, and ranked operational actions.

## Engagements

I am available for focused freelance and contract work involving:

| Engagement | Typical delivery |
| --- | --- |
| **Rust backend and systems engineering** | Performance-sensitive APIs, concurrency-safe services, deterministic kernels, verification tooling, and production hardening |
| **AI infrastructure** | Model gateways, RAG and retrieval services, provider routing, cost governance, evaluation, observability, and policy enforcement |
| **Python data products** | FastAPI services, validated ETL pipelines, web scraping, CSV/Excel transformation, scheduled automation, and reporting |
| **Applied ML systems** | Churn, lead scoring, pricing, uplift, forecasting, calibration, SHAP, and decision queues |
| **Technical audit and rescue** | Architecture review, correctness testing, performance diagnosis, CI repair, security boundaries, and maintainability upgrades |

Every engagement is scoped around a measurable outcome, explicit failure modes, tested deliverables, and a maintainable handoff.

## Flagship — Calybris Core

[![crates.io](https://img.shields.io/crates/v/calybris-core?label=calybris-core&logo=rust)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?logo=docs.rs)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml)
[![CodSpeed](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://app.codspeed.io/emirhuseynrmx/calybris-core)

[**Calybris Core**](https://github.com/emirhuseynrmx/calybris-core) is a deterministic, proof-carrying decision kernel for routing, guardrails, and budget-sensitive automation.

```text
catalog + policy + request  →  decision + verifiable audit bundle
```

It is designed for systems where a team must be able to answer:

- Why was this model, provider, offer, or action selected?
- Which policy and budget state were used?
- Can the decision be replayed and independently verified?
- Can concurrent requests overspend or violate exposure limits?

Engineering evidence:

- Integer-only Rust hot path at approximately **115 ns per decision**
- Byte-exact proof contract, golden vectors, replay verification, and `calybris-verify` auditor CLI
- SHA-256 digests, hash-chained WAL with optional HMAC, and Ed25519 policy provenance
- CAS budget accounting with conservation invariants verified using Loom and Miri
- No hosted dependency and no `unsafe` in project code

```bash
cargo add calybris-core
```

## Selected work

| Project | Business problem | What it demonstrates |
| --- | --- | --- |
| [**ProofFrame**](https://github.com/emirhuseynrmx/proofframe) | Data pipelines need fast validation and durable evidence of exactly what was checked | Arrow-native Rust/Python contracts, canonical fingerprints, keyed diffs, PII and leakage scans, signed proof receipts |
| [**Aegis**](https://github.com/emirhuseynrmx/aegis) | Churn scores are not useful unless teams know whom to contact and which action may help | Calibrated risk, uplift evidence, SHAP, counterfactuals, expected-value decisions, and an operations dashboard |
| [**Churn Prediction & Retention Report**](https://github.com/emirhuseynrmx/churn-prediction-retention-report) | Analysts need reproducible scoring and a stakeholder-ready action report | Validated ML pipeline, calibration, confidence intervals, model cards, ranked retention queue, and PDF delivery |
| [**CRM Lead List Cleaning API**](https://github.com/emirhuseynrmx/data-quality-cleaning-api) | Messy CRM imports create duplicates, invalid contacts, and unreliable automations | FastAPI cleanup service, email and phone normalization, deduplication, profiling, safe CSV export, Docker, and OpenAPI |
| [**Scrape Quality Pipeline**](https://github.com/emirhuseynrmx/scraping-data-pipeline) | Scraped data must remain reliable when pages, selectors, or output schemas change | Async collection, polite rate limits, retries, typed records, Pandera validation, manifests, tests, and CSV/JSONL/Excel/Parquet export |
| [**Price Monitor Pipeline**](https://github.com/emirhuseynrmx/price-monitor-pipeline) | Teams need repeatable public price checks instead of manual monitoring | Config-driven extraction, validated snapshots, threshold alerts, run manifests, and client-ready reports |

## Delivery standard

```text
Clear scope → typed boundaries → tests and CI → observable execution
            → reproducible output → documentation and handoff
```

- Production-minded code with explicit assumptions and failure behavior
- Tests for correctness-critical paths and fixtures for external integrations
- CI, linting, dependency boundaries, and reproducible setup
- Honest evaluation: no inflated accuracy, ROI, performance, or AI claims
- Documentation aimed at the next engineer or operator, not only the original author

## Core stack

**Languages:** Rust, Python, TypeScript, SQL

**Backend & data:** Tokio, Axum, FastAPI, Litestar, Pydantic, Polars, Pandas, Arrow, DuckDB, PostgreSQL

**AI & ML:** model routing, RAG, XGBoost, LightGBM, CatBoost, SHAP, uplift modeling, contextual bandits

**Delivery:** Docker, Linux, GitHub Actions, OpenAPI, Typst, Next.js, React

**Verification:** property-based testing, Loom, Miri, replay tests, cryptographic digests, audit trails

## Start a conversation

If you are dealing with an unreliable data workflow, expensive AI pipeline, difficult Rust backend, or ML system that produces scores but not decisions, send me:

1. the business problem,
2. the current stack or data source,
3. the expected deliverable,
4. the target timeline.

I can help define a focused first milestone before expanding the scope.

<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>
### Build systems that can explain — and prove — what they did.

[Portfolio](https://emirhuseyin.tech) · [Email](mailto:emirhuseyininci@gmail.com?subject=Project%20inquiry) · [LinkedIn](https://linkedin.com/in/emirhuseyininci) · [Calybris on crates.io](https://crates.io/crates/calybris-core) · [ProofFrame on PyPI](https://pypi.org/project/proofframe/)

</div>

<div align="center">

# Emir Hüseyin İnci

### Rust Systems Engineer · AI Infrastructure · Decision Systems · Applied Machine Learning

I build deterministic, auditable software for high-stakes decisions — from proof-carrying Rust kernels to production-style Python data and ML systems.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![Email](https://img.shields.io/badge/Email-Let's_talk-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com)

</div>

## What I build

- **Rust systems:** deterministic decision kernels, replayable audit trails, cryptographic proofs, tamper-evident WALs, concurrency-safe budget engines, and low-latency APIs.
- **AI infrastructure:** model/provider routing, guardrails, cost governance, retrieval systems, observability, and policy enforcement.
- **Applied ML:** churn prediction, uplift modeling, counterfactual explanations, calibration, SHAP, and decision-focused analytics.
- **Data products:** validated pipelines, data-quality APIs, reproducible reports, scraping workflows, and operational dashboards.

## Flagship project — Calybris Core

[![crates.io](https://img.shields.io/crates/v/calybris-core?label=calybris-core&logo=rust)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?logo=docs.rs)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml)
[![CodSpeed](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://app.codspeed.io/emirhuseynrmx/calybris-core)

[**Calybris Core**](https://github.com/emirhuseynrmx/calybris-core) is a deterministic, proof-carrying decision kernel for routing and guardrails. Given a frozen catalog, policy snapshot, and typed request, it returns one action plus an audit bundle that can be replayed to the same answer.

```text
catalog + policy + request  →  decision + verifiable audit bundle
```

- Integer-only Rust hot path at approximately **115 ns per decision**
- Byte-exact proof contract, golden vectors, replay verification, and `calybris-verify` auditor CLI
- SHA-256 digests, hash-chained WAL with optional HMAC, and Ed25519 policy provenance
- CAS budget accounting with conservation invariants verified using Loom and Miri
- No hosted dependency and no `unsafe` in project code
- Stable Rust crate plus experimental PyO3/Pydantic Python bindings

```bash
cargo add calybris-core
```

## Selected projects

| Project | Engineering focus | Stack |
| --- | --- | --- |
| [**Calybris Core**](https://github.com/emirhuseynrmx/calybris-core) | Proof-carrying decision engine, deterministic replay, cryptographic audit, budget safety | Rust, Tokio, SHA-256, HMAC, Ed25519, Loom, Miri |
| [**Aegis**](https://github.com/emirhuseynrmx/aegis) | Prescriptive churn analytics with calibrated risk, uplift evidence, SHAP, counterfactuals, and an operations dashboard | Python, Litestar, Polars, XGBoost, SHAP, Next.js, DuckDB, Postgres |
| [**Churn Prediction Retention Report**](https://github.com/emirhuseynrmx/churn-prediction-retention-report) | Reproducible churn scoring pipeline with calibration, confidence intervals, model cards, and a ranked action queue | Python, XGBoost, Pandera, Pydantic, SHAP, Typst |
| [**CRM Lead List Cleaning API**](https://github.com/emirhuseynrmx/data-quality-cleaning-api) | Idempotent API for profiling, validating, deduplicating, and safely exporting CRM data | Python, FastAPI, Pandera, Docker, OpenAPI |
| [**Local RAG Chatbot**](https://github.com/emirhuseynrmx/rag-chatbot) | Source-aware local document retrieval with visible evidence and no required external API | Python, FastAPI, TF-IDF, PDF ingestion |
| [**Price Monitor Pipeline**](https://github.com/emirhuseynrmx/price-monitor-pipeline) | Repeatable public price checks, validated snapshots, threshold alerts, and run manifests | Python, Pandera, scraping, CSV, Typst |

## Engineering principles

```text
Deterministic when correctness matters.
Evidence-first when models make claims.
Typed and validated at every boundary.
Observable, replayable, and honest about limits.
```

## Core stack

**Languages:** Rust, Python, TypeScript, SQL  
**Backend & data:** Tokio, FastAPI, Litestar, Pydantic, Polars, Pandas, DuckDB, PostgreSQL  
**ML & decisioning:** XGBoost, LightGBM, CatBoost, SHAP, uplift modeling, contextual bandits, RAG  
**Frontend & delivery:** Next.js, React, Docker, Linux, GitHub Actions  
**Verification:** property-based testing, Loom, Miri, replay tests, cryptographic digests, audit trails

## Current focus

- Shipping **Calybris Core 0.5.0** and its independent verification tooling
- Building AI cost-governance and model-routing systems on top of deterministic policy kernels
- Turning predictive models into auditable operational decisions instead of isolated scores

<div align="center">

### Let’s build systems that can explain — and prove — what they did.

Open to **Rust systems**, **AI infrastructure**, **decision-engine**, **applied ML**, and **data-product** work.

[Portfolio](https://emirhuseyin.tech) · [Calybris on crates.io](https://crates.io/crates/calybris-core) · [LinkedIn](https://linkedin.com/in/emirhuseyininci) · [Email](mailto:emirhuseyininci@gmail.com)

</div>

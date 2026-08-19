<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci Portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

# Emir Hüseyin İnci

### Rust Systems Engineer · Python Backend · Data Infrastructure · Decision Systems

**Building high-throughput backend services, deterministic execution kernels, and zero-copy data pipelines.**

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![crates.io](https://img.shields.io/crates/v/calybris-core?style=for-the-badge&logo=rust&logoColor=white&label=crates.io&color=orange)](https://crates.io/crates/calybris-core)
[![PyPI](https://img.shields.io/pypi/v/proofframe?style=for-the-badge&logo=pypi&logoColor=white&label=PyPI&color=blue)](https://pypi.org/project/proofframe/)
[![Email](https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Project%20Inquiry%20/%20Engineering%20Engagement)

</div>

---

## ⚡ Engineering Highlights & Verifiable Metrics

- **Sub-microsecond Decision Kernel:** Built integer-only deterministic routing kernels in Rust executing at **~115 ns per decision (8.6M decisions/sec)** with zero heap allocation.
- **Zero-Copy Arrow Pipelines:** Engineered data validation and contract enforcement running directly on **Apache Arrow C Streams (`Utf8View`/`BinaryView`)** with bounded memory.
- **Out-of-Core Spill Engine:** Designed external K-Way merge-sort spill engines enforcing strict RAM budgets (e.g. **64 MB**) over multi-million row datasets without OOM crashes.
- **Cryptographic Audit Trails:** Implemented **BLAKE3 canonical dataset fingerprinting** and **Ed25519 digital evidence receipts** for verifiable compliance (SOC 2, ISO 42001, EU AI Act).
- **Formal Correctness & Concurrency Safety:** Enforced `#![forbid(unsafe_code)]`, multi-platform CI matrices, and validated concurrency boundaries using **Loom, Miri, and Property-Based Testing (proptest)**.

---

## 🏆 Flagship Open-Source Projects

### 🦀 [Calybris Core](https://github.com/emirhuseynrmx/calybris-core) — Deterministic, Proof-Carrying Decision Kernel
[![crates.io](https://img.shields.io/crates/v/calybris-core?logo=rust)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?logo=docs.rs)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core)

A high-integrity decision primitive for LLM routing, financial guardrails, and budget-bounded automation.
- Evaluates constraints over frozen catalogs and emits verifiable proof bundles.
- Replay-auditable execution with byte-exact state transitions and a standalone `calybris-verify` auditor CLI.
- Hash-chained WAL with HMAC signing and CAS budget accounting verified with Loom.

```bash
cargo add calybris-core
```

---

### 🏹 [ProofFrame](https://github.com/emirhuseynrmx/proofframe) — Arrow-Native Data Contract & Evidence Engine
[![PyPI](https://img.shields.io/pypi/v/proofframe.svg)](https://pypi.org/project/proofframe/)
[![CI](https://github.com/emirhuseynrmx/proofframe/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/proofframe)

A high-performance "Ruff-like" data validation kernel designed for high-throughput ETL and production pipelines.
- Compiles data contracts into typed Arrow kernels with zero-copy stream ingestion (Pandas, Polars, PyArrow).
- Memory-bounded out-of-core spill engine prevents Kubernetes pod OOM evictions on large datasets.
- Generates BLAKE3 dataset fingerprints and Ed25519-signed proof receipts for data lineage and compliance.

```bash
pip install proofframe==0.5.0
```

---

## 📂 Selected Engineering Work

| Project | Tech Stack | Business & Architectural Problem | Key Delivery & Output |
| :--- | :--- | :--- | :--- |
| [**ProofFrame**](https://github.com/emirhuseynrmx/proofframe) | `Rust`, `Apache Arrow`, `PyO3`, `BLAKE3`, `Ed25519` | Production pipelines need sub-millisecond validation without OOM memory spikes. | Arrow-native engine, memory budgets, spill-to-disk exact state, signed receipts. |
| [**Calybris Core**](https://github.com/emirhuseynrmx/calybris-core) | `Rust`, `PyO3`, `WAL`, `Loom`, `Miri`, `Ed25519` | High-stakes automation requires deterministic decisions and tamper-evident audit trails. | 115 ns integer kernel, replay verification, single-writer WAL, CLI auditor. |
| [**Churn & Retention Report**](https://github.com/emirhuseynrmx/churn-prediction-retention-report) | `Python`, `scikit-learn`, `SHAP`, `Pandera`, `Typst` | Raw churn probabilities fail to provide actionable operational retention strategies. | Calibrated risk scoring, XAI drivers, Pandera contracts, Typst executive PDF reports. |
| [**Scrape Quality Pipeline**](https://github.com/emirhuseynrmx/scraping-data-pipeline) | `Python`, `selectolax`, `asyncio`, `Pydantic v2`, `Pandera` | Web data ingestion breaks silently when selectors, schemas, or network rules shift. | Config-driven scrapers, polite rate limiting, Pydantic validation, Parquet/CSV export. |
| [**Price Monitor Pipeline**](https://github.com/emirhuseynrmx/price-monitor-pipeline) | `Python`, `Pandera`, `Typst`, `CLI` | E-commerce teams require automated competitor price monitoring and alert queues. | Watchlist config, threshold alert tables, run manifests, automated PDF summaries. |

---

## 💼 Client & Contract Engagements

I partner with engineering teams, startups, and enterprises for focused contract roles:

| Domain | Deliverables & Scope |
| :--- | :--- |
| **Rust Systems Engineering** | Performance-critical backends, Tokio/Axum services, deterministic state machines, memory profiling, and concurrency hardening. |
| **Data Infrastructure & ETL** | Arrow-native data quality pipelines, schema contracts, out-of-core processing, async scrapers, and automated reporting. |
| **AI Cost & Spend Governance** | Model gateways, token budget enforcement, fallback routing, policy simulation, and audit receipt architectures. |
| **Applied ML & Decision Systems** | Churn prediction pipelines, uplift modeling, SHAP explainability, calibration curves, and ranked operational queues. |
| **Technical Audit & Refactoring** | Concurrency verification (Loom/Miri), CI/CD pipeline repair, memory leak diagnosis, and production readiness audits. |

---

## 🛠️ Technical Stack & Tooling

```text
Languages     : Rust (1.85+), Python (3.10–3.13), TypeScript, SQL
Backend       : Tokio, Axum, FastAPI, Litestar, Pydantic v2, REST, OpenAPI, gRPC
Data & Storage: Apache Arrow, Polars, DuckDB, Parquet, PostgreSQL, SQLite, Redis
Testing & QA  : Loom, Miri, Property-based testing (proptest), Fuzzing, pytest, Ruff
Delivery & Ops: Linux, Docker, Helm, Kubernetes, GitHub Actions, CI/CD, Typst
```

---

## 📬 Start a Conversation

If you are dealing with an unstable data pipeline, expensive AI inference costs, a memory-intensive backend, or need auditable systems engineering:

1. **Business Problem & Context**
2. **Current Tech Stack & Data Sources**
3. **Expected Deliverable & Timeline**

Send an inquiry to **[emirhuseyininci@gmail.com](mailto:emirhuseyininci@gmail.com?subject=Project%20Inquiry%20/%20Engineering%20Engagement)** or connect on **[LinkedIn](https://linkedin.com/in/emirhuseyininci)**.

<div align="center">

<br/>

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci Portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

### *Build systems that can explain — and prove — what they did.*

[Portfolio](https://emirhuseyin.tech) · [Email](mailto:emirhuseyininci@gmail.com) · [LinkedIn](https://linkedin.com/in/emirhuseyininci) · [crates.io](https://crates.io/crates/calybris-core) · [PyPI](https://pypi.org/project/proofframe/)

</div>

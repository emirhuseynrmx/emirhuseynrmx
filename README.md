<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci Portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

# Emir Hüseyin İnci

### Python Backend & Data Engineer · Applied ML · Rust Systems

**Available for full-time and contract roles — Türkiye / remote**

Python backends, data pipelines and applied ML. I also write Rust infrastructure for
deterministic execution and Arrow-native processing. Maintainer of ProofFrame,
Calybris Core and ReproCut.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![crates.io](https://img.shields.io/crates/v/calybris-core?style=for-the-badge&logo=rust&logoColor=white&label=crates.io&color=orange)](https://crates.io/crates/calybris-core)
[![PyPI](https://img.shields.io/pypi/v/proofframe?style=for-the-badge&logo=pypi&logoColor=white&label=PyPI&color=blue)](https://pypi.org/project/proofframe/)
[![Email](https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)

</div>

---

## What I work on

Data and decision systems where the answer has to be reproducible — not just fast.
Most of my work sits in one of three places: **validating data before it reaches a
model**, **turning model output into a decision**, and **proving afterwards what the
system actually did**.

Two of these are published packages you can install today; the rest are read-only
portfolio work.

---

## Published packages

### [ProofFrame](https://github.com/emirhuseynrmx/proofframe) — Arrow-native data quality, Rust + Python

[![PyPI](https://img.shields.io/pypi/v/proofframe.svg)](https://pypi.org/project/proofframe/)
[![CI](https://github.com/emirhuseynrmx/proofframe/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/proofframe)

Contract validation for PyArrow, Pandas, Polars, CSV and Parquet that scans record
batches without turning rows into Python objects.

- Exact uniqueness, cross-column rules and keyed diffs under an explicit memory budget.
- Out-of-core spill so a large dataset does not become an OOM kill.
- BLAKE3 dataset fingerprints and Ed25519-signed receipts, so a run can be identified
  and re-checked later.
- Fails closed: an exceeded limit or an ambiguous contract is an error, never an
  approximate answer.

```bash
pip install proofframe
```

### [Calybris Core](https://github.com/emirhuseynrmx/calybris-core) — deterministic decision kernel, Rust + Python

[![crates.io](https://img.shields.io/crates/v/calybris-core?logo=rust)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?logo=docs.rs)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core)

Give it a catalog, a policy and a request; get one decision plus an audit bundle that
replays to the same answer.

- Integer-only kernel, no floating point: **~115 ns per decision** on the documented
  22-model synthetic workload, reproducible via `cargo bench`.
- Hash-chained WAL with HMAC and an external head anchor that detects even a clean
  suffix truncation.
- Concurrent budget ledger holding `remaining + reserved + committed == initial`,
  checked with **Loom** for interleavings and **Miri** for undefined behaviour.
- `#![forbid(unsafe_code)]`, CI across Linux/macOS/Windows and Python 3.10–3.14.

```bash
cargo add calybris-core
```

---

## Selected work

| Project | Stack | Problem | What it does |
| :--- | :--- | :--- | :--- |
| [**Aegis**](https://github.com/emirhuseynrmx/aegis) | `Python` `XGBoost` `SHAP` `DoWhy` `DiCE` `Litestar` | A churn probability is not an action. | Calibrated risk, uplift/CATE, counterfactuals and expected-value logic behind an API and an operations dashboard. |
| [**Criteo Uplift Benchmark**](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark) | `Python` `scikit-learn` `causal ML` | Uplift papers rarely compare methods on equal footing. | S-, T-, X- and DR-Learner plus Causal Forest on the Criteo dataset, scored with AUUC/Qini against a response-model baseline. |
| [**ReproCut**](https://github.com/emirhuseynrmx/reprocut) | `Rust` `ddmin` `SQLite` `AST` | A minimal reproduction is expensive to produce by hand. | Removes files, dependencies and syntax nodes while the original failure still reproduces, verifying each candidate in a fresh snapshot. |
| [**Scrape Quality Pipeline**](https://github.com/emirhuseynrmx/scraping-data-pipeline) | `Python` `asyncio` `Pydantic v2` `Pandera` | Scrapers fail silently when a selector or schema shifts. | Config-driven async scraping with typed records, schema validation and Parquet/CSV output. |
| [**Churn & Retention Report**](https://github.com/emirhuseynrmx/churn-prediction-retention-report) | `Python` `scikit-learn` `SHAP` `Typst` | Stakeholders need a document, not a notebook. | Calibrated scoring and SHAP drivers rendered into a reviewed PDF report. |

---

## Open to

| Area | What I bring |
| :--- | :--- |
| **Python backend** | FastAPI/Litestar services, Pydantic v2 boundaries, async I/O, PostgreSQL and Redis. |
| **Data engineering** | Arrow, Polars, DuckDB and Parquet pipelines with schema contracts and bounded memory. |
| **Applied ML** | Calibration, SHAP, uplift/CATE, counterfactuals, and turning scores into ranked actions. |
| **Rust systems** | Tokio/Axum services, concurrency hardening, and verification with Loom, Miri and proptest. |
| **Reliability work** | CI/CD repair, test and benchmark infrastructure, profiling, release engineering. |

---

## Stack

```text
Languages     : Python (3.10–3.14), Rust (1.85+), SQL, TypeScript
Backend       : FastAPI, Litestar, Tokio, Axum, Pydantic v2, REST, OpenAPI
Data          : Apache Arrow, Polars, DuckDB, Parquet, PostgreSQL, SQLite, Redis
ML            : scikit-learn, XGBoost, LightGBM, SHAP, DoWhy, DiCE, uplift/CATE
Testing       : pytest, Pandera, proptest, Loom, Miri, fuzzing, Ruff, MyPy
Delivery      : Linux, Docker, GitHub Actions, OpenTelemetry, Prometheus, Grafana
```

---

## Get in touch

Open to full-time and contract roles in Python backend, data engineering and applied
ML — remote, or on-site in Türkiye.

**[emirhuseyininci@gmail.com](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)** · **[LinkedIn](https://linkedin.com/in/emirhuseyininci)** · **[emirhuseyin.tech](https://emirhuseyin.tech)**

<div align="center">

<br/>

### *Build systems that can explain — and prove — what they did.*

</div>

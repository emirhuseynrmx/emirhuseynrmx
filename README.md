<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci Portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

### Rust & Python engineer

I make slow Python fast with Rust, build data pipelines that don't fall over on messy input,
and ship the result as packages people can `pip install` or `cargo add`.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![crates.io](https://img.shields.io/crates/v/calybris-core?style=for-the-badge&logo=rust&logoColor=white&label=crates.io&color=orange)](https://crates.io/crates/calybris-core)
[![PyPI](https://img.shields.io/pypi/v/proofframe?style=for-the-badge&logo=pypi&logoColor=white&label=PyPI&color=blue)](https://pypi.org/project/proofframe/)
[![Email](https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)

</div>

---

## Published packages

<a href="https://github.com/emirhuseynrmx/calybris-core"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/calybris-logo-dark.svg"><img src="assets/calybris-logo-light.svg" alt="Calybris Core" width="400"></picture></a>

[![crates.io](https://img.shields.io/crates/v/calybris-core.svg?style=flat-square&color=e05d44&logo=rust)](https://crates.io/crates/calybris-core) [![docs.rs](https://img.shields.io/docsrs/calybris-core.svg?style=flat-square&logo=docs.rs)](https://docs.rs/calybris-core) [![CI](https://img.shields.io/github/actions/workflow/status/emirhuseynrmx/calybris-core/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/emirhuseynrmx/calybris-core/actions)

A Rust decision engine: give it options, rules and a request, and it picks an action the same way every time, with a record you can replay later.

- Integer-only kernel, about 115 ns per decision in CI benchmarks (CodSpeed, Linux x86_64)
- Budgets that can't be overspent by two requests arriving at once
- Rust crate with `#![forbid(unsafe_code)]`, Python package via PyO3, and a WebAssembly build that runs in the browser: [calybris.tech](https://calybris.tech)

<a href="https://github.com/emirhuseynrmx/proofframe"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/proofframe-logo-dark.svg"><img src="assets/proofframe-logo-light.svg" alt="ProofFrame" width="400"></picture></a>

[![PyPI](https://img.shields.io/pypi/v/proofframe.svg?style=flat-square&color=3775a9&logo=pypi)](https://pypi.org/project/proofframe/) [![CI](https://img.shields.io/github/actions/workflow/status/emirhuseynrmx/proofframe/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/emirhuseynrmx/proofframe/actions)

Data validation for Pandas, Polars, PyArrow, CSV and Parquet, with a Rust core. It checks rules like "no missing names" or "ids are unique" without turning your data into Python objects, and stays inside a memory budget by spilling to disk.

```bash
pip install proofframe
```

---

## Python → Rust

<a href="https://github.com/emirhuseynrmx/fuzzy-dedupe-rs"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/fuzzy-dedupe-rs/main/assets/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/fuzzy-dedupe-rs/main/assets/logo-light.svg" alt="fuzzy-dedupe" width="400"></picture></a>

Exact near-duplicate detection and record linkage for names: Rust core, Python API, CLI. A partition filter from the similarity-join literature (PASS-JOIN) plus bit-parallel edit distance, returning exactly the pairs an exhaustive comparison would. On 100,000 real UK company names: **136x faster than RapidFuzz, same 21,513 pairs**; a persistent index answers single lookups against 800,000 names in 0.05 ms. Apache-2.0.

---

## Data & automation

<table>
<tr><td><a href="https://github.com/emirhuseynrmx/trading-performance-report-kit"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/trading-performance-report-kit/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/trading-performance-report-kit/main/docs/logo-light.svg" alt="Trading Performance Report Kit" width="400"></picture></a></td><td><a href="https://github.com/emirhuseynrmx/csv-excel-cleaning-toolkit"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/csv-excel-cleaning-toolkit/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/csv-excel-cleaning-toolkit/main/docs/logo-light.svg" alt="CSV & Excel Cleaning Toolkit" width="400"></picture></a></td></tr>
<tr><td><a href="https://github.com/emirhuseynrmx/scraping-data-pipeline"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/scraping-data-pipeline/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/scraping-data-pipeline/main/docs/logo-light.svg" alt="Scrape Quality Pipeline" width="400"></picture></a></td><td><a href="https://github.com/emirhuseynrmx/price-monitor-pipeline"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/price-monitor-pipeline/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/price-monitor-pipeline/main/docs/logo-light.svg" alt="Price Monitor Pipeline" width="400"></picture></a></td></tr>
</table>

## AI & machine learning

<table>
<tr><td><a href="https://github.com/emirhuseynrmx/rag-chatbot"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/rag-chatbot/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/rag-chatbot/main/docs/logo-light.svg" alt="RAG Chatbot Template" width="400"></picture></a></td><td><a href="https://github.com/emirhuseynrmx/churn-prediction-retention-report"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/churn-prediction-retention-report/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/churn-prediction-retention-report/main/docs/logo-light.svg" alt="Churn Prediction Retention Report" width="400"></picture></a></td></tr>
<tr><td><a href="https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/criteo-uplift-modeling-benchmark/main/assets/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/criteo-uplift-modeling-benchmark/main/assets/logo-light.svg" alt="Criteo Uplift Modeling Benchmark" width="400"></picture></a></td><td><a href="https://github.com/emirhuseynrmx/forecastedge"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/forecastedge/main/assets/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/forecastedge/main/assets/logo-light.svg" alt="ForecastEdge" width="400"></picture></a></td></tr>
</table>

## Bots & workflows

<table>
<tr><td><a href="https://github.com/emirhuseynrmx/telegram-business-bot"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/telegram-business-bot/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/telegram-business-bot/main/docs/logo-light.svg" alt="Telegram Business Bot Template" width="400"></picture></a></td><td><a href="https://github.com/emirhuseynrmx/n8n-business-automation-workflows"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/emirhuseynrmx/n8n-business-automation-workflows/main/docs/logo-dark.svg"><img src="https://raw.githubusercontent.com/emirhuseynrmx/n8n-business-automation-workflows/main/docs/logo-light.svg" alt="n8n Business Automation Workflows" width="400"></picture></a></td></tr>
</table>

---

## Stack

```text
Languages   : Rust, Python, SQL
Rust        : Tokio, Axum, PyO3, maturin, rayon, WebAssembly
Data        : Polars, Pandas, Apache Arrow, DuckDB, Parquet
ML          : scikit-learn, LightGBM, XGBoost, SHAP, causal ML (uplift)
Testing     : pytest, proptest, fuzzing, Loom, Miri, GitHub Actions on Linux/macOS/Windows
```

## Open to

Full-time roles and contract work, remote worldwide or on-site in Türkiye:

- Speeding up Python with Rust extensions (PyO3)
- Data pipelines and cleanup: Polars, DuckDB, Arrow, scraping, reports
- Rust backend services (Tokio, Axum)

**[emirhuseyininci@gmail.com](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)** · **[LinkedIn](https://linkedin.com/in/emirhuseyininci)** · **[emirhuseyin.tech](https://emirhuseyin.tech)**

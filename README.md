<div align="center">

<a href="https://emirhuseyin.tech" aria-label="Emir Hüseyin İnci Portfolio">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-light-trim.png">
    <source media="(prefers-color-scheme: light)" srcset="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png">
    <img src="https://emirhuseyin.tech/assets/brand/ehi-lockup-dark-trim.png" alt="Emir Hüseyin İnci" width="520">
  </picture>
</a>

# Emir Hüseyin İnci

### Rust Systems & Data Infrastructure Engineer
#### Deterministic Systems · Arrow-Native Pipelines · High-Throughput Runtimes (Loom, Miri, PyO3)

I engineer deterministic execution kernels, Arrow-native data infrastructure, and low-latency runtimes
where correctness is formally verified rather than assumed. Maintainer of Calybris Core, ProofFrame, and ReproCut.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![crates.io](https://img.shields.io/crates/v/calybris-core?style=for-the-badge&logo=rust&logoColor=white&label=crates.io&color=orange)](https://crates.io/crates/calybris-core)
[![PyPI](https://img.shields.io/pypi/v/proofframe?style=for-the-badge&logo=pypi&logoColor=white&label=PyPI&color=blue)](https://pypi.org/project/proofframe/)
[![Email](https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)

</div>

---

## Engineering Philosophy

Most software is written for the happy path. I build for the edge cases, the adversarial inputs, and the post-mortems six months later.

* **Fail-Closed by Construction:** A breached limit, an unexpected type, or an unhandled signal must immediately halt execution — never silently approximate or degrade into undefined behavior.
* **Deterministic & Replayable:** Eliminating nondeterminism at the kernel level: integer-only fixed-point arithmetic, canonical SHA-256 byte digests, and append-only Write-Ahead Logs (WAL) so any historical state can be replayed and independently audited.
* **Hardware-Conscious Runtimes:** Mindful of memory layouts, cache lines, zero-copy record batch streaming, and explicit allocation boundaries rather than relying on uncontrolled GC or global allocators.
* **Formally Hardened Concurrency:** Concurrency is never trusted until thread interleavings are proven with **Loom**, memory safety is validated with **Miri**, and state machines survive property-based fuzzing with **proptest**.

---

## Flagship Systems

### [Calybris Core](https://github.com/emirhuseynrmx/calybris-core) [![crates.io](https://img.shields.io/crates/v/calybris-core.svg?style=flat-square&color=e05d44&logo=rust)](https://crates.io/crates/calybris-core) [![docs.rs](https://img.shields.io/docsrs/calybris-core.svg?style=flat-square&logo=docs.rs)](https://docs.rs/calybris-core) [![CI](https://img.shields.io/github/actions/workflow/status/emirhuseynrmx/calybris-core/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/emirhuseynrmx/calybris-core)

A high-frequency, deterministic decision primitive designed for high-stakes routing, order admission, and policy guardrails. Given a catalog, a policy, and a request; it computes an exact action and seals it with a tamper-evident audit bundle.

* **Zero floating-point arithmetic:** Fixed-point integer kernel executing at **~115 ns per decision** on documented 22-model synthetic workloads (`cargo bench`).
* **Cryptographic Audit Trail:** Hash-chained WAL with HMAC and external head anchors detecting even clean suffix truncations.
* **Formally Verified Ledger:** Concurrent budget accounting (`remaining + reserved + committed == initial`) exhaustively checked with **Loom** for race conditions and **Miri** for UB.
* **Portability:** Ships as an idiomatic Rust crate (`#![forbid(unsafe_code)]`), typed Python package via **PyO3**, and zero-dependency 237 KB **WebAssembly (WASM)**.

```bash
cargo add calybris-core
```

### [ProofFrame](https://github.com/emirhuseynrmx/proofframe) [![PyPI](https://img.shields.io/pypi/v/proofframe.svg?style=flat-square&color=3775a9&logo=pypi)](https://pypi.org/project/proofframe/) [![CI](https://img.shields.io/github/actions/workflow/status/emirhuseynrmx/proofframe/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/emirhuseynrmx/proofframe)

In-memory contract validation and data integrity engine for PyArrow, Pandas, Polars, and Parquet that evaluates record batches directly in memory without turning rows into Python heap objects.

* **Out-of-Core Memory Boundaries:** Enforces explicit memory budgets with automatic disk spilling to eliminate OOM kills on massive datasets.
* **Cryptographic Lineage:** Generates BLAKE3 dataset fingerprints and Ed25519-signed verification receipts for auditable data contracts.
* **Zero-Copy Scans:** Evaluates exact uniqueness, cross-column assertions, and keyed diffs under strict SIMD-friendly column alignments.

```bash
pip install proofframe
```

### [ReproCut](https://github.com/emirhuseynrmx/reprocut) [![CI](https://img.shields.io/github/actions/workflow/status/emirhuseynrmx/reprocut/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/emirhuseynrmx/reprocut)

An evidence-backed Delta Debugging (`ddmin`) system that minimizes failing codebases to their smallest reproducible state while guaranteeing the exact failure signature is preserved.

* **Multi-Tier Reduction Pipeline:** Slices directory/file trees, prunes dependency manifests (`Cargo.toml`, `pyproject.toml`, `package.json`), and performs syntax node pruning/hoisting via **Tree-sitter** across 8 languages (Rust, C, C++, Python, Go, Java, JS, TS).
* **Hermetic Isolation:** Every candidate evaluation executes in disposable snapshots with OS process-group signal containment (`command-group`) and SQLite WAL state checkpointing.
* **Independent CI Validation:** Validated against large real-world repositories (e.g. Bevy Engine, Ipe) inside unprivileged, network-isolated (`--network none`) Linux containers.

```bash
cargo install reprocut --locked
```

---

## Selected Work

| Project | Core Stack | Domain | Architecture Highlights |
| :--- | :--- | :--- | :--- |
| [**Aegis**](https://github.com/emirhuseynrmx/aegis) | `Python` `XGBoost` `SHAP` `DoWhy` `Litestar` | Decision Engines / Causal ML | Turns uncalibrated probabilities into expected-value actions; provides CATE/uplift modeling and counterfactual recourse. |
| [**Criteo Uplift Benchmark**](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark) | `Python` `scikit-learn` `causal ML` | Statistical Evaluation | Rigorous benchmark comparing S-, T-, X-, and DR-Learners alongside Causal Forests scored with AUUC and Qini curves. |
| [**Scrape Quality Pipeline**](https://github.com/emirhuseynrmx/scraping-data-pipeline) | `Python` `asyncio` `Pydantic v2` `Pandera` | Data Engineering | High-concurrency async ingestion with typed runtime contracts, schema drift protection, and partitioned Parquet outputs. |
| [**Churn & Retention Report**](https://github.com/emirhuseynrmx/churn-prediction-retention-report) | `Python` `scikit-learn` `SHAP` `Typst` | Technical Reporting | Calibrated risk scoring and SHAP explainability drivers compiled into automated publication-grade PDFs via Typst. |

---

## Technical Stack & Tooling

```text
Languages     : Rust (1.85+, #![forbid(unsafe_code)]), Python (3.10–3.14), SQL, 
                TypeScript / JavaScript, C / C++ (FFI, Tree-sitter, C-ABI), POSIX Shell / Bash, WebAssembly (WASM)
Systems       : Tokio, Axum, PyO3, SQLite (WAL + single-writer sync channels), Process Groups (SIGTERM/SIGKILL), Docker, OCI
Data & Storage: Apache Arrow, Polars, DuckDB, Parquet, BLAKE3, SHA-256, Ed25519, JSONL
Verification  : Loom (concurrency permutation model-checking), Miri (undefined behavior detection), 
                proptest (property-based fuzzing), criterion (statistical microbenchmarking), pytest, Ruff, MyPy
Infrastructure: Linux (Debian/Ubuntu), GitHub Actions (matrix & hermetic runner CI), Docker (rootless, non-networked)
```

---

## Open To

Available for full-time engineering roles and contract work — **Remote (worldwide)** or on-site in Türkiye:

* **Rust Systems & Runtime Engineering:** High-throughput microservices (Tokio/Axum), deterministic execution kernels, PyO3 native bindings, and WebAssembly compilation.
* **Data Infrastructure:** Arrow-native data engines, zero-copy record batch streaming, query validation layers, and memory-bounded out-of-core pipelines.
* **Correctness, Verification & Safety:** Concurrency model checking (Loom), Undefined Behavior elimination (Miri), write-ahead logging (WAL), and hermetic CI/CD test gates.

**[emirhuseyininci@gmail.com](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)** · **[LinkedIn](https://linkedin.com/in/emirhuseyininci)** · **[emirhuseyin.tech](https://emirhuseyin.tech)**

<div align="center">

<br/>

### *Build systems that can explain — and prove — what they did.*

</div>

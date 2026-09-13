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
#### Deterministic Systems · Arrow-native Pipelines · High-Throughput Runtimes (Loom, Miri, PyO3)

**Available for full-time and contract roles — Türkiye / remote**

Low-level systems programming in Rust and high-throughput data infrastructure in Python.
I build deterministic execution kernels, Arrow-native validation engines, and memory-bounded runtimes
hardened with Loom, Miri, and proptest. Maintainer of ProofFrame, Calybris Core, and ReproCut.

[![Portfolio](https://img.shields.io/badge/Portfolio-emirhuseyin.tech-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://emirhuseyin.tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emir_Hüseyin_İnci-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/emirhuseyininci)
[![crates.io](https://img.shields.io/crates/v/calybris-core?style=for-the-badge&logo=rust&logoColor=white&label=crates.io&color=orange)](https://crates.io/crates/calybris-core)
[![PyPI](https://img.shields.io/pypi/v/proofframe?style=for-the-badge&logo=pypi&logoColor=white&label=PyPI&color=blue)](https://pypi.org/project/proofframe/)
[![Email](https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:emirhuseyininci@gmail.com?subject=Role%20/%20Contract%20Enquiry)

</div>

---

## What I work on

Data, runtime, and decision infrastructure where correctness and execution must be **deterministic, auditable, and memory-bounded** — not just fast.

* **Deterministic & Decision Kernels:** Fixed-point integer arithmetic, hash-chained Write-Ahead Logs (WAL), and cryptographic proof-bundles that replay to the exact same byte-level verdict offline.
* **Arrow-Native Data Pipelines:** In-memory record batch validation without Python object allocation overhead, out-of-core spill management, and zero-copy column evaluations.
* **Formal Concurrency & Correctness:** Thread interleaving permutations verified with **Loom**, undefined behaviour (UB) eliminated with **Miri**, property testing via **proptest**, and strict adherence to `#![forbid(unsafe_code)]`.

---

## Core systems & published packages

### [Calybris Core](https://github.com/emirhuseynrmx/calybris-core) — deterministic decision kernel, Rust + Python

[![crates.io](https://img.shields.io/crates/v/calybris-core?logo=rust)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?logo=docs.rs)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core)

A high-throughput decision kernel. Feed it a catalog, a policy, and a request; get one decision plus an audit bundle that replays to the identical outcome.

- **Zero floating-point arithmetic:** Integer-only kernel executing at **~115 ns per decision** on documented 22-model synthetic workloads (`cargo bench`).
- **Cryptographic Audit Trail:** Hash-chained WAL with HMAC and external head anchors detecting even clean suffix truncations.
- **Formally Verified Concurrency:** Concurrent budget ledger validated across thread permutations with **Loom** and memory checked with **Miri**.
- **Polyglot & Portable:** Runs as a native Rust crate, typed Python package via **PyO3**, and zero-dependency 237 KB **WebAssembly (WASM)**.

```bash
cargo add calybris-core

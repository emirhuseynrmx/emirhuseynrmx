<div align="center">

# Emir Huseyin Inci

**Rust / Python · Decision Systems · AI Infrastructure · Proof-Carrying Engineering**

[Portfolio](https://emirhuseyin.tech) · [LinkedIn](https://linkedin.com/in/emirhuseyininci) · [Email](mailto:emirhuseyininci@gmail.com)

<br/>

<img src="https://skillicons.dev/icons?i=rust,python,postgres,docker,linux,git,githubactions&theme=light" alt="Core stack" />

<br/><br/>

<img src="https://img.shields.io/badge/Tokio-232323?style=flat&logo=rust&logoColor=white" alt="Tokio"/>
<img src="https://img.shields.io/badge/SHA--256-111827?style=flat&logoColor=white" alt="SHA-256"/>
<img src="https://img.shields.io/badge/Loom-4B5563?style=flat&logoColor=white" alt="Loom"/>
<img src="https://img.shields.io/badge/Miri-7C3AED?style=flat&logoColor=white" alt="Miri"/>
<img src="https://img.shields.io/badge/proptest-0A9EDC?style=flat&logoColor=white" alt="proptest"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" alt="Pandas"/>
<img src="https://img.shields.io/badge/Pydantic-E92063?style=flat&logo=pydantic&logoColor=white" alt="Pydantic"/>

</div>

---

I build deterministic decision engines and AI infrastructure with cryptographic proof, formal-ish verification, and auditable output.

**Shipping:** [Calybris Core](https://github.com/emirhuseynrmx/calybris-core) — proof-carrying decision engine in Rust. [GOVERIS](https://emirhuseyin.tech/goveris/) — AI cost governance gateway powered by Calybris.

---

## Calybris Core

[![Crates.io](https://img.shields.io/crates/v/calybris-core)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml)

Deterministic proof-carrying decision engine for systems that must explain and replay why an action was allowed, substituted, or rejected.

- **~115ns/decision** — integer-only kernel, zero allocation, zero `unsafe`
- **ProofEnvelope** — SHA-256 sealed evidence: policy + input + decision + WAL + budget
- **HMAC-SHA256 WAL** — tamper-evident, constant-time, crash-recoverable
- **CAS budget engine** — conservation-proven, Loom-verified, exposure-capped
- **Async WAL** — Tokio non-blocking, configurable fsync
- **145+ tests** — proptest, 7 Loom exhaustive, Miri UB, cargo-audit/deny

```
cargo add calybris-core --features full
```

## Products

| Product | What it does | Link |
|---------|-------------|------|
| **Calybris Core** | Deterministic decision kernel + proof + WAL + budget | [GitHub](https://github.com/emirhuseynrmx/calybris-core) · [crates.io](https://crates.io/crates/calybris-core) |
| **GOVERIS** | AI cost governance gateway — shadow replay, audit reports, tenant attribution | [Site](https://emirhuseyin.tech/goveris/) |
| **Calybris Engine** | Full proprietary stack — adaptive routing, Thompson Sampling, GBM, HTTP API | [Site](https://emirhuseyin.tech/engine/) |
| **Aegis** | Prescriptive churn analytics — calibrated ensemble, SHAP, DoWhy causal, DiCE counterfactuals, 173 tests | [GitHub](https://github.com/emirhuseynrmx/aegis) · [Site](https://emirhuseyin.tech/aegis/) |

---

<div align="center">

Building proof-carrying AI infrastructure. Open to **Rust systems**, **AI infrastructure**, and **decision engine** work.

</div>

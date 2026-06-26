<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,35:1F6FEB,70:8957E5,100:0D1117&height=190&section=header&text=Emir%20H%C3%BCseyin%20%C4%B0nci&fontSize=46&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=Decision%20Engines%20%C2%B7%20Causal%20ML%20%C2%B7%20Prescriptive%20Analytics&descAlignY=58&descAlign=50&descSize=18&descColor=A5D6FF"
    width="100%"
    alt="Emir Hüseyin İnci"
  />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img
      src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&repeat=true&width=900&height=58&lines=8.6M+decisions%2Fsec+%E2%80%94+pure+Rust%2C+zero+unsafe;Causal+ML+%7C+Uplift+modeling+%7C+Treatment+effects;From+prediction+to+intervention+to+proof"
      alt="Typing animation"
    />
  </a>
</div>

<div align="center">
  <a href="https://emirhuseyin.tech">
    <img src="https://img.shields.io/badge/Portfolio-0D1117?style=for-the-badge&logo=safari&logoColor=white" alt="Portfolio"/>
  </a>
  <a href="https://emirhuseyin.tech/goveris/">
    <img src="https://img.shields.io/badge/GOVERIS-C9A227?style=for-the-badge&logoColor=white" alt="GOVERIS"/>
  </a>
  <a href="https://linkedin.com/in/emirhuseyininci">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:emirhuseyininci@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</div>

<br/>

I build systems that go beyond prediction: **decision engines** that choose, **causal models** that explain why, and **prescriptive pipelines** that act. My work spans integer-kernel optimization in Rust and uplift modeling in Python, always with proof, tests, and reproducibility.

Currently building **[GOVERIS](https://emirhuseyin.tech/goveris/)** — AI cost governance powered by the Calybris decision engine.

---

## Flagship: Calybris Core

<table>
<tr>
<td width="60%">

### [calybris-core](https://github.com/emirhuseynrmx/calybris-core) — Open-Source Decision Engine

[![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)](https://github.com/emirhuseynrmx/calybris-core)
[![Crates.io](https://img.shields.io/crates/v/calybris-core?style=flat-square)](https://crates.io/crates/calybris-core)
[![docs.rs](https://img.shields.io/docsrs/calybris-core?style=flat-square)](https://docs.rs/calybris-core)
[![CI](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml/badge.svg)](https://github.com/emirhuseynrmx/calybris-core/actions/workflows/ci.yml)
[![codecov](https://codecov.io/gh/emirhuseynrmx/calybris-core/graph/badge.svg?style=flat-square)](https://codecov.io/gh/emirhuseynrmx/calybris-core)
[![License](https://img.shields.io/badge/Apache--2.0-blue?style=flat-square)](https://github.com/emirhuseynrmx/calybris-core/blob/main/LICENSE)

Deterministic proof-carrying decision core: integer kernel, replay verification, fixed-point budget proofs, HMAC-SHA256 hash-chained WAL. No `f64` in the hot path, `#![forbid(unsafe_code)]`.

```
cargo add calybris-core
cargo test --all-features   # 99 unit + integration
cargo bench                 # 8.6M decisions/sec (kernel)
```

</td>
<td width="40%">

| Metric | Value |
|:--|--:|
| Kernel throughput | **8.6M/sec** |
| Constraint gates | 11 |
| Tests | 99 + proptest + Loom + Miri |
| `unsafe` blocks | 0 |
| WAL integrity | HMAC-SHA256 |
| Budget engine | CAS + conservation proof |

</td>
</tr>
</table>

**Modules:** `kernel` (utility-maximizing prescribe + counterfactuals) · `verify` (canonical digests + replay) · `finance` (ledger digest + `FinancialCertificate`) · `budget` (per-tenant CAS + I6 invariant) · `wal` (tamper-evident audited chain).

Reference paths: **LLM routing** and **pre-trade guard** — not an exchange or strategy engine.

The full engine (adaptive Thompson Sampling routing, policy evolution, GBM prompt model, HTTP gateway) powers [GOVERIS](https://emirhuseyin.tech/goveris/) and is proprietary.

---

## Other Projects

### [Criteo Uplift Modeling Benchmark](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![LightGBM](https://img.shields.io/badge/LightGBM-26A65B?style=flat-square)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![EconML](https://img.shields.io/badge/EconML-8957E5?style=flat-square)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)

**7M rows**, 6 uplift learners (S/T/X/DR-Learner, Causal Forest, response baseline). S-Learner won with **AUUC 3405**, top-decile uplift **6.23x**. Pydantic-typed, fully reproducible.

---

### [Aegis](https://github.com/emirhuseynrmx/aegis) — Prescriptive Churn Analytics

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/emirhuseynrmx/aegis)
[![Tests](https://img.shields.io/badge/173_tests-94%25_coverage-success?style=flat-square)](https://github.com/emirhuseynrmx/aegis)

Prediction + SHAP explanation + DoWhy causal analysis + DiCE counterfactual prescription + financial value decisioning + backtesting. End-to-end from churn probability to retention action.

---

### [AeraCFO](https://github.com/emirhuseynrmx/aera) — AI Finance Reporting

[![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)](https://github.com/emirhuseynrmx/aera)
[![Tests](https://img.shields.io/badge/63_tests-passing-success?style=flat-square)](https://github.com/emirhuseynrmx/aera)

Axum + Polars + Gemini 2.5 Flash. Upload financial data, run planner-executor-critic agent loop, generate structured PDF report. MIT licensed.

---

## Technical Focus

<div align="center">

<img src="https://skillicons.dev/icons?i=rust,python,pytorch,fastapi,docker,postgres,git&theme=dark&perline=7" alt="Tech stack"/>

<br/><br/>

| Domain | Tools |
|:--|:--|
| Decision Systems | Rust, integer kernels, CAS atomics, HMAC-SHA256, hash-chained WAL |
| Causal ML | LightGBM, EconML, DoWhy, SHAP, DiCE, uplift/CATE estimation |
| Infrastructure | Axum, Polars, FastAPI, Docker, PostgreSQL |

</div>

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=emirhuseynrmx&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=8957E5&text_color=C9D1D9&ring_color=8957E5" height="170" alt="GitHub stats"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=emirhuseynrmx&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=C9D1D9&langs_count=6" height="170" alt="Top languages"/>

</div>

---

<div align="center">

Open to decision intelligence, causal ML, and systems engineering roles and collaborations.

**[emirhuseyin.tech](https://emirhuseyin.tech)** · **[emirhuseyininci@gmail.com](mailto:emirhuseyininci@gmail.com)**

</div>

<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,35:1F6FEB,70:8957E5,100:0D1117&height=120&section=footer&animation=fadeIn"
    width="100%"
    alt="Footer"
  />
</div>

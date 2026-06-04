<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,35:1F6FEB,70:8957E5,100:0D1117&height=190&section=header&text=Emir%20H%C3%BCseyin%20%C4%B0nci&fontSize=46&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=Causal%20ML%20%C2%B7%20Prescriptive%20Analytics%20%C2%B7%20Quant%20Research&descAlignY=58&descAlign=50&descSize=18&descColor=A5D6FF"
    width="100%"
    alt="Emir Hüseyin İnci - Causal ML, Prescriptive Analytics, Quant Research"
  />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img
      src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&repeat=true&width=900&height=58&lines=Building+causal+ML+systems+for+better+decisions;Uplift+modeling+%7C+Treatment+effects+%7C+Decision+intelligence;Python+%7C+Rust+%7C+LightGBM+%7C+DoWhy+%7C+Polars"
      alt="Typing animation: Causal ML, uplift modeling, treatment effects, decision intelligence"
    />
  </a>
</div>

<div align="center">
  <a href="https://linkedin.com/in/emirhuseyininci">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:emirhuseyininci@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://kaggle.com/emirhseyinnci">
    <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"/>
  </a>
</div>

<br/>

I build machine learning systems that move from **prediction** to **intervention**: uplift modeling, treatment-effect estimation, prescriptive analytics, and quant research infrastructure.

Currently refining **AeraCFO** for production reporting and packaging the **Criteo uplift benchmark** as a public research repository.

---

## What I Build

| Area | Focus |
|:--|:--|
| Causal ML | Uplift modeling, CATE estimation, AUUC/Qini evaluation, treatment-aware targeting |
| Prescriptive Analytics | Turning model outputs into actions, policies, expected value, and retention decisions |
| Quant Research | Leakage control, reproducible backtests, alpha modeling, market-data infrastructure |
| ML Systems | Fast APIs, typed configs, testable pipelines, drift monitoring, production workflows |

---

## Featured Work

### [Criteo Uplift Modeling Benchmark](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![Pydantic](https://img.shields.io/badge/Pydantic_v2-E92063?style=for-the-badge&logo=pydantic&logoColor=white)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![LightGBM](https://img.shields.io/badge/LightGBM-26A65B?style=for-the-badge)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![EconML](https://img.shields.io/badge/EconML-Causal_Forest-8957E5?style=for-the-badge)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)
[![Metric](https://img.shields.io/badge/Metric-AUUC_/_Qini-00BFA5?style=for-the-badge)](https://github.com/emirhuseynrmx/criteo-uplift-modeling-benchmark)

Modular Python benchmark on 7M Criteo rows comparing S-Learner, T-Learner, X-Learner, DR-Learner, Causal Forest, and a response-model targeting baseline.

| Signal | Result |
|:--|--:|
| Validation winner | S-Learner |
| Test AUUC | 3405.48 |
| Top-decile relative uplift | 6.23x |
| Top 10% policy gain | ~6,865 incremental visits |
| Causal Forest cost | 3335s, 14.5 GB peak RSS |

The main takeaway was practical: S-Learner gave the best production trade-off in this run, while Causal Forest was useful but expensive at this scale.

---

### [AeraCFO](https://github.com/emirhuseynrmx/aera) - Autonomous AI CFO Platform

[![Rust](https://img.shields.io/badge/Rust_1.75+-000000?style=for-the-badge&logo=rust&logoColor=orange)](https://github.com/emirhuseynrmx/aera)
[![Axum](https://img.shields.io/badge/Axum_0.7-blueviolet?style=for-the-badge)](https://github.com/emirhuseynrmx/aera)
[![Polars](https://img.shields.io/badge/Polars-CD792C?style=for-the-badge&logo=polars&logoColor=white)](https://github.com/emirhuseynrmx/aera)
[![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://github.com/emirhuseynrmx/aera)
[![Tests](https://img.shields.io/badge/Tests-58%2F58_passing-success?style=for-the-badge)](https://github.com/emirhuseynrmx/aera)
[![License](https://img.shields.io/badge/License-MIT-F39C12?style=for-the-badge)](https://github.com/emirhuseynrmx/aera)

Autonomous finance workflow for SMEs: upload CSV/XLSX data, run a planner-executor-critic agent loop, forecast business metrics, detect anomalies, and generate a corporate PDF report.

The project is now MIT-licensed. A larger update is planned around reporting quality, agent reliability, and production readiness.

---

### [Aegis](https://github.com/emirhuseynrmx/aegis) - Prescriptive Analytics Engine for Telecom Churn

[![Python](https://img.shields.io/badge/Python_3.12+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/emirhuseynrmx/aegis)
[![XGBoost](https://img.shields.io/badge/XGBoost_3.x-E74C3C?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)
[![SHAP](https://img.shields.io/badge/SHAP-00BFA5?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)
[![DoWhy](https://img.shields.io/badge/DoWhy-E67E22?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)
[![DiCE](https://img.shields.io/badge/DiCE--ml-9B59B6?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)
[![Tests](https://img.shields.io/badge/Tests-173%2F173_passing-success?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)
[![Coverage](https://img.shields.io/badge/Coverage-94%25-00BFA5?style=for-the-badge)](https://github.com/emirhuseynrmx/aegis)

Most churn systems stop at prediction. Aegis adds explanation, counterfactual prescription, financial value, causal treatment-effect estimation, and backtesting.

```text
Prediction -> calibrated churn ensemble
Explanation -> causal SHAP and DoWhy path attribution
Prescription -> DiCE counterfactual scenarios with SCM constraints
Financial -> WACC-NPV expected value decisioning
Causal -> T-Learner CATE and sleeping-dog detection
Validation -> backtesting and PSI drift monitoring
```

---

### [NexusAlpha](https://github.com/emirhuseynrmx/nexusalpha) - Anti-Leakage Quantitative Alpha Engine

[![XGBoost](https://img.shields.io/badge/XGBoost_v2-E74C3C?style=for-the-badge)](https://github.com/emirhuseynrmx/nexusalpha)
[![Optuna](https://img.shields.io/badge/Optuna_50--trial-6C63FF?style=for-the-badge)](https://github.com/emirhuseynrmx/nexusalpha)
[![Polars](https://img.shields.io/badge/Polars_ETL-CD792C?style=for-the-badge&logo=polars&logoColor=white)](https://github.com/emirhuseynrmx/nexusalpha)
[![TreeSHAP](https://img.shields.io/badge/Native_TreeSHAP-00BFA5?style=for-the-badge)](https://github.com/emirhuseynrmx/nexusalpha)
[![SHA256](https://img.shields.io/badge/SHA--256_Secure_Boot-555?style=for-the-badge)](https://github.com/emirhuseynrmx/nexusalpha)

Quant research engine focused on reproducibility, leakage control, feature integrity, and explainable alpha modeling.

Roadmap note: NexusAlpha is planned for a Rust-first, HFT-oriented rework with faster market-data handling, cleaner backtesting primitives, and stricter alpha evaluation.

---

## Technical Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=rust,python,pytorch,fastapi,docker,redis,postgres,git&theme=dark&perline=8" alt="Rust, Python, PyTorch, FastAPI, Docker, Redis, PostgreSQL, Git"/>

<br/><br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-26A65B?style=flat-square)
![XGBoost](https://img.shields.io/badge/XGBoost-E74C3C?style=flat-square)
![DoWhy](https://img.shields.io/badge/DoWhy-Causal_Inference-E67E22?style=flat-square)
![EconML](https://img.shields.io/badge/EconML-Treatment_Effects-8957E5?style=flat-square)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-00BFA5?style=flat-square)
![DiCE](https://img.shields.io/badge/DiCE-Counterfactuals-BF8BFF?style=flat-square)
![Polars](https://img.shields.io/badge/Polars-CD792C?style=flat-square&logo=polars&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

</div>

---

<div align="center">

Open to applied ML, causal inference, quant research, and analytics-engineering collaborations.

</div>

<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,35:1F6FEB,70:8957E5,100:0D1117&height=120&section=footer&animation=fadeIn"
    width="100%"
    alt="Footer wave animation"
  />
</div>

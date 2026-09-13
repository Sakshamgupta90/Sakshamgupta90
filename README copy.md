<!-- ════════════════════════ HERO ════════════════════════ -->
<div align="center">
  <img src="assets/hero.svg" alt="Shreyansh Goyal - Machine Learning Engineer · MSc Data Science @ NTU Singapore" width="100%"/>
</div>

<p align="center">
  <a href="https://www.linkedin.com/in/shreyansh-goyal-iitb/"><img src="https://img.shields.io/badge/LinkedIn-shreyansh--goyal--iitb-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:shreyanshgoyal1203@gmail.com"><img src="https://img.shields.io/badge/Gmail-shreyanshgoyal1203-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/></a>
  <img src="https://img.shields.io/badge/Based%20in-Singapore-9ece6a?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Based in Singapore"/>
</p>

## 🧑‍💻 whoami

<div align="center">
  <img src="assets/terminal.svg" alt="Terminal bio: Machine Learning Engineer, MSc Data Science @ NTU Singapore (Aug 2026 - Jun 2027), B.Tech Mechanical Engineering IIT Bombay, Lead MLE @ MyShubhLife, Analyst - ML Processes @ UGRO Capital" width="100%"/>
</div>

Machine Learning Engineer with **3 years building credit-risk decisioning systems end-to-end** (modeling → pipelines → AWS production) at a listed SME-lending NBFC and its consumer-lending subsidiary.

- 🎓 **MSc in Data Science** @ **Nanyang Technological University, Singapore** - College of Computing and Data Science *(Aug 2026 - Jun 2027)*
- 💼 Recent work: default-prediction **AUC 0.65 → 0.75** via a counterparty GNN over **150M+ transactions**, an early-warning system at **AUC 0.87**, and a **74% model-serving cost cut**
- 🔬 Into **GNNs**, **time-series**, **model interpretability**, **efficient ML**, and **audio** - with a soft spot for Kaggle leaderboards 🎹

> **📌 Seeking Singapore-based internships alongside the MSc:** **16 h/week during term** (classes run evenings) and **full-time during vacations**, under MOM's student work-pass exemption - **no separate work pass required**.

## 🚀 The Journey

<div align="center">
  <img src="assets/timeline.svg" alt="Timeline: 2019 IIT Bombay → 2023 UGRO Capital → 2025 MyShubhLife → 2026 NTU Singapore → 2027+" width="100%"/>
</div>

## 📊 Production Impact

<div align="center">
  <img src="assets/metrics.svg" alt="Metrics: default AUC 0.65→0.75 with GNNs, early-warning AUC 0.87, −74% serving infra cost, latency 60s→28s, 150M+ transactions" width="100%"/>
</div>

## 💼 Experience

### Lead Machine Learning Engineer · *Jan 2025 - Aug 2026*
**MyShubhLife (now GROx Technologies), UGRO Capital Group** - consumer-lending fintech · Bengaluru, India

- Shipped an **early-warning system** predicting borrower default 30 days ahead: two-segment ensemble (clean vs. failed-auto-debit borrowers) on recency features, **test AUC 0.87**; risk tiers drive collections prioritisation, cutting **roll-forward rates 8%** over one quarter.
- Raised default-prediction test **AUC 0.65 → 0.75** over a logistic baseline with a **counterparty graph neural network** (shared counterparties propagate risk), trained on **37K borrowers / 100K bank statements / 150M+ transactions** and served within production latency budgets.
- Owned the **Gro Score credit-scoring API** on AWS behind live lending decisions - automated validation suites, feature-ablation analyses, and **schema and completeness checks on third-party bank-statement payloads** that caught truncated or malformed JSON before it reached the model, triggering upstream re-pulls instead of silent mis-scoring.
- Built **7-day cash-flow forecasters** on **180-day** transaction histories (**MAPE 12.5%**, stable backtests across cohorts); productionised the feature and evaluation suite used across credit-limit experiments and quarterly underwriting policy reviews.

### Analyst - ML Processes · *Jun 2023 - Dec 2024*
**UGRO Capital** - listed SME-lending NBFC · Mumbai, India

- Containerised TensorFlow scoring models and migrated serving from a single 8-core EC2 instance to **AWS Lambda**: **infra cost down 74%**, end-to-end scoring **60s → 28s**, and removed the capacity ceiling behind peak-hour failures. All UGRO lending products routed through this API, underwriting applications converting to **~US$30M (INR 250 Cr) in monthly disbursals**.
- Rebuilt the **tax-filing (GST) default-prediction model** after portfolio review found the incumbent at test Gini 16 - logistic regression, random forest, and ANN with spline smoothing over proprietary filing-pattern features - lifting **test Gini 16 → 36** (train 38; minimal generalisation gap) on 30+ DPD at 12 months; features reused across multiple lending products.
- Built the pre-release **monitoring and regression-test suite** (schema checks, feature-sanity tests, latency SLO gates, drift alerts, automated reports) that caught regressions before release and gated the team's frequent production deploys.

## 🛠️ Tech Stack

<div align="center">

**Languages & Core**

<img src="https://skillicons.dev/icons?i=python,cpp,postgres,git&theme=dark" alt="Python, C++, PostgreSQL, Git"/>

*Python (NumPy, pandas, Polars) · SQL · C++*

**ML / Deep Learning**

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn&theme=dark" alt="PyTorch, TensorFlow, scikit-learn"/>

<img src="assets/focus.svg" alt="XGBoost · LightGBM · CatBoost · Transformers · Graph Neural Networks · ONNX" width="100%"/>

*Time-series forecasting · backtesting · credit-scorecard modelling · feature engineering · model validation*

**MLOps & Infrastructure**

<img src="https://skillicons.dev/icons?i=aws,docker,fastapi&theme=dark" alt="AWS, Docker, FastAPI"/>

*AWS (Lambda, EC2, S3, CloudWatch) · Docker · PostgreSQL · Git · FastAPI · CI/regression · model & drift monitoring*

</div>

## 💡 Projects

| Project | What it does |
|---|---|
| 🏦 **[Credit Scoring Service](https://github.com/ShreyanshGoyal/credit-scoring-service)** · **[live demo](https://credit-scoring-service-1042616833497.asia-southeast1.run.app/)** <br/> *FastAPI, LightGBM, Docker, GCP* | Reference implementation of my production serving patterns: FastAPI scoring API with Pydantic validation at the edge, **rolling-window PSI drift monitoring** with reproducible alert demos, golden-row regression tests, CI with a container smoke test, and a non-root Docker image - **deployed live on Cloud Run (Singapore)** with a public interactive demo, rebuilt on every push. |
| 🏈 **[NFL Big Data Bowl 2026](https://github.com/ShreyanshGoyal/nfl_big_data_bowl_2026)** - Player Trajectory Prediction <br/> *Kaggle, **top-25% finish** · PyTorch, CatBoost, LightGBM* | Residual model over a physics baseline - CatBoost, LightGBM, set-transformer and GNN heads with per-horizon **XGBoost** stacking - under leakage-safe GroupKFold CV with fixed seeds, horizon-wise metrics, ablations, and automated experiment reports. |
| 🧩 **[NeuroGolf 2026](https://github.com/ShreyanshGoyal/neurogolf_2026)** - Minimal Neural Networks for ARC-AGI Tasks <br/> *Kaggle · PyTorch, ONNX* | Two-stage solver: symbolic rule engine compiling grid transformations to near-zero-parameter **ONNX** graphs, plus a cheapest-first neural fallback ladder; every candidate verified with onnxruntime and scored in a crash-isolated subprocess before submission. |
| 🎙️ **[Query-by-Humming](https://github.com/ShreyanshGoyal/query_by_humming)** - Audio Retrieval <br/> *Python, librosa, DTW* | Chroma + DTW retrieval for humming-to-song search robust to tempo drift; wavefront-vectorised DTW validated against a brute-force reference, plus a reproducible evaluation harness with per-query alignment visualisations and ranking diagnostics. |

## 🎓 Education

| | |
|---|---|
| **Nanyang Technological University (NTU), Singapore** <br/> MSc in Data Science, College of Computing and Data Science | *Aug 2026 - Jun 2027* <br/> Singapore |
| **Indian Institute of Technology (IIT) Bombay** <br/> B.Tech, Mechanical Engineering | *2019 - 2023* <br/> Mumbai, India |

## 🤝 Let's Connect

<p align="center">
  <a href="https://www.linkedin.com/in/shreyansh-goyal-iitb/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:shreyanshgoyal1203@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hi!-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/ShreyanshGoyal"><img src="https://img.shields.io/badge/GitHub-Follow-1a1b27?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
</p>

<!-- ════════════════════════ FOOTER ════════════════════════ -->
<div align="center">
  <img src="assets/footer.svg" alt="Thanks for stopping by - let's build something intelligent" width="100%"/>
</div>

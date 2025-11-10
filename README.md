# 🧠 Bayesian Risk Assessment Using Cybersecurity Data

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Model-Type:Bayesian%20Network-purple?logo=databricks&logoColor=white" />
  <img src="https://img.shields.io/badge/Field-Cybersecurity-red?logo=shield&logoColor=white" />
  <img src="https://img.shields.io/github/stars/Godakash007/bayesian-risk-assessment?style=social" />
</p>

---

## 🔍 Objective

The **Bayesian Risk Assessment** project implements a **Bayesian Network-based risk analysis framework** to evaluate and rank the likelihood of cybersecurity threats compromising digital assets.  

This approach applies **Bayesian inference** to combine threat intelligence, vulnerabilities, and success rates — producing **quantifiable risk rankings** and supporting **data-driven mitigation decisions**.

---

## 🎯 Key Goals

- Identify **high-risk assets** using probabilistic modeling  
- Analyze **threat actors, vulnerabilities, and exploit probabilities**  
- Compute **posterior probabilities** using Bayesian inference  
- Prioritize **mitigation strategies** based on total risk scores  

---

## 🧩 Project Structure

```bash
bayesian-risk-assessment/
 ├── data/                         # Input datasets
 │   ├── asset_vulnerability_mapping_data.xlsx
 │   ├── threat_actor_asset_mapping_data.xlsx
 │   ├── threat_intel_data.xlsx
 │   └── prior_attack_success_rate.xlsx
 │
 ├── output/                       # Final ranked results
 │   └── ranked_risk_assets.xlsx
 │
 ├── src/                          # Source code for data processing and analysis
 │   ├── data_loader.py
 │   ├── preprocess.py
 │   ├── threat_intel_loader.py
 │   ├── risk_analysis.py
 │   └── main.py
 │
 ├── AkashA_BayesianRiskReport.pdf # Final project report
 ├── requirements.txt              # Python dependencies
 └── README.md                     # This file

---
🛠️**Tools & Libraries Used**

| Tool / Library | Purpose |
|----------------|----------|
| **pgmpy** | Bayesian Network modeling and inference |
| **pandas** | Data manipulation and integration |
| **matplotlib** | Visualization and graph plotting |
| **networkx** | Network graph layout and structure visualization |

---
⚙️**Risk Score Calculation**

The model computes risk dynamically using the following formulas:

risk_score = cvss_score × exploit_probability
total_risk_score = risk_score × target_probability × success_rate


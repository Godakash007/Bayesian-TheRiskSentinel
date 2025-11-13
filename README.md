# 🧠 Bayesian Risk Assessment Using Cybersecurity Data

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Framework-Bayesian%20Network%20Analysis-green?logo=graph&logoColor=white" />
  <img src="https://img.shields.io/badge/Domain-Cybersecurity%20Risk%20Assessment-red?logo=shield&logoColor=white" />
  <img src="https://img.shields.io/badge/Methodology-Probabilistic%20Inference-yellow?logo=brain&logoColor=white" />
  <img src="https://img.shields.io/github/stars/Godakash007/BayesShield?style=social" />
</p>


This project implements a **Bayesian Network–based risk assessment framework** to evaluate and rank the likelihood of cybersecurity threats compromising various digital assets.

## 🔍 Objective

To identify high-risk assets by:

- Analyzing vulnerabilities, threat actors, and exploit probabilities  
- Calculating posterior probabilities using Bayesian inference  
- Prioritizing mitigation based on total risk scores  

---

## 📂 Project Structure

```bash
bayesian-risk-assessment/
 ├── data/                         # Contains all input datasets
 │   ├── asset_vulnerability_mapping_data.xlsx
 │   ├── threat_actor_asset_mapping_data.xlsx
 │   ├── threat_intel_data.xlsx
 │   └── prior_attack_success_rate.xlsx
 │
 ├── output/                       # Final ranked results exported here
 │   └── ranked_risk_assets.xlsx
 │
 ├── src/                          # Source code for data processing and risk analysis
 │   ├── data_loader.py
 │   ├── preprocess.py
 │   ├── threat_intel_loader.py
 │   ├── risk_analysis.py
 │   └── main.py
 │
 ├── AkashA_BayesianRiskReport.pdf  # Final report for evaluation
 ├── requirements.txt               # Python dependencies
 └── README.md                      # This file
````

---

## 🛠️ Tools & Libraries Used

| Tool / Library | Purpose                                          |
| -------------- | ------------------------------------------------ |
| **pgmpy**      | Bayesian Network modeling and inference          |
| **pandas**     | Data manipulation and integration                |
| **matplotlib** | Visualization and graph plotting                 |
| **networkx**   | Network graph layout and structure visualization |

---

## ⚙️ Risk Score Calculation

The model computes risk dynamically using the following formulas:

```text
risk_score = cvss_score × exploit_probability
total_risk_score = risk_score × target_probability × success_rate
```

These calculations help quantify each asset’s potential exposure level and rank them accordingly.

---

## 📊 Features

✅ Automated Data Preprocessing & Cleaning
✅ Dynamic Bayesian Inference for Threat Likelihoods
✅ Asset Risk Ranking & Visualization
✅ Auto-Generated Mitigation Strategies Based on Risk Levels
✅ PDF Report Generation (`AkashA_BayesianRiskReport.pdf`)

---

## 🧠 Workflow Summary

| Step                                  | Description                                                   |
| ------------------------------------- | ------------------------------------------------------------- |
| 1️⃣ **Load Data**                     | Import vulnerability, threat, and success rate datasets.      |
| 2️⃣ **Preprocess**                    | Clean and normalize the data for model compatibility.         |
| 3️⃣ **Build Bayesian Model**          | Construct dependencies between assets, threats, and exploits. |
| 4️⃣ **Infer Posterior Probabilities** | Calculate likelihood of asset compromise.                     |
| 5️⃣ **Rank Assets**                   | Export a ranked list of assets by total risk score.           |
| 6️⃣ **Generate Report**               | Visualize results and mitigation recommendations.             |

---

## 📈 Example Output

| Asset     | Risk Score | Posterior Probability | Rank |
| --------- | ---------- | --------------------- | ---- |
| Server_01 | 0.842      | 0.74                  | 1    |
| WebApp_02 | 0.610      | 0.53                  | 2    |
| DB_03     | 0.505      | 0.45                  | 3    |

*(Example visualization — actual results are in `output/ranked_risk_assets.xlsx`)*

---

## 📄 Final Report

📘 **Report File:** `AkashA_BayesianRiskReport.pdf`

Includes:

* Prior probability assignments
* Bayesian Network diagram
* Posterior probability tables
* Risk ranking visualization (bar graph)
* Decision support and mitigation strategy

---

## ⚡ Installation & Usage

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Godakash007/Bayesian-TheRiskSentinel.git
cd bayesian-risk-assessment
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Main Script

```bash
python src/main.py
```

### 4️⃣ Check the Output

Results are saved in:

```
/output/ranked_risk_assets.xlsx
```

Visualizations and the final report are auto-generated.


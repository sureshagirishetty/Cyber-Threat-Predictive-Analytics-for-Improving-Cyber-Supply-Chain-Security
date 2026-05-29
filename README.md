<div align="center">

# 🔐 Cyber Threat Predictive Analytics
### for Improving Cyber Supply Chain Security

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-scikit--learn-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)
![HTML](https://img.shields.io/badge/Frontend-HTML%20%7C%20CSS-green?style=for-the-badge&logo=html5&logoColor=white)
![Accuracy](https://img.shields.io/badge/Accuracy-85%25-brightgreen?style=for-the-badge)
![IEEE](https://img.shields.io/badge/Reference-IEEE%20Access%202021-red?style=for-the-badge)

*A machine learning system that predicts cyber threats in supply chain environments using Cyber Threat Intelligence (CTI) properties.*

</div>

---

## 📋 Table of Contents

- [About the Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Dataset & Threat Categories](#-dataset--threat-categories)
- [Machine Learning Models](#-machine-learning-models)
- [Results](#-results)
- [Project Structure](#-project-structure)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [How to Run](#-how-to-run)
- [System Requirements](#-system-requirements)
- [Advantages Over Existing Systems](#-advantages-over-existing-systems)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

## 📖 About the Project

Cyber Supply Chain (CSC) systems are inherently complex, with vulnerabilities that can cascade across interconnected nodes and disrupt entire business operations. Traditional security systems react to incidents **after** they occur — this project takes a fundamentally different approach.

By combining **Cyber Threat Intelligence (CTI)** with **Machine Learning (ML)**, this system proactively detects, analyses, and predicts cyber threats before they can impact supply chain operations. It leverages TTPs (Tactics, Techniques, and Procedures) and IoCs (Indicators of Compromise) as model inputs to forecast potential attack vectors.

> 📄 Published Reference: **IEEE Access, June 2021**  
> Keywords: Cyber Threat Intelligence · Machine Learning · Cyber Supply Chain · Predictive Analytics

---

## ✨ Key Features

- 🎯 Predicts **five breach types**: Theft, Loss, Disclosure, Hacking, and Improper Disposal
- 🤖 Applies **four ML classifiers**: Logistic Regression, SVM, Random Forest, and Decision Tree
- 🧠 Integrates **CTI properties** — IoC, TTP, threat actor motivation — as model inputs
- 📊 Achieves up to **85% predictive accuracy** (TPR / FPR analysis)
- 🦠 Identifies **Spyware/Ransomware** and **Spear Phishing** as the most predictable CSC threats
- 🛡️ Recommends **actionable security controls** based on prediction outcomes
- 🌐 Interactive **web interface** built with HTML and CSS for result visualisation

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Language | Python 3.x |
| Machine Learning | scikit-learn (LR, SVM, RF, DT) |
| Data Processing | pandas, NumPy |
| Visualisation | matplotlib, seaborn |
| Web Interface | HTML5, CSS3 |
| Dataset | Microsoft Malware Prediction Dataset |
| OS Support | Windows 7 / 8 / 10 (32-bit & 64-bit) |

---

## 📂 Dataset & Threat Categories

The **Microsoft Malware Prediction Dataset** is used for model training and evaluation. Breach types are encoded as follows:

| Label | Breach Type | Encoded Value |
|---|---|---|
| Theft | Stolen hardware or data | `0` |
| Loss | Accidental data loss | `1` |
| Disclosure | Unauthorised data exposure | `2` |
| Hacking | Active intrusion or exploit | `3` |
| Improper Disposal | Insecure data/hardware disposal | `4` |

### Key Dataset Columns

```
Name_of_Covered_Entity    State                   Individuals_Affected
Date_of_Breach            Location_of_Breached_Information
breach_start              year
Source_IP                 Destination_IP
Prediction                detection_ratio         detection_accuracy
```

---

## 🤖 Machine Learning Models

| Model | Strengths in This Context |
|---|---|
| Logistic Regression (LR) | Highest accuracy; fast and interpretable |
| Support Vector Machine (SVM) | Excellent for high-dimensional threat feature spaces |
| Random Forest (RF) | Robust to noise; handles imbalanced breach data well |
| Decision Tree (DT) | Transparent, rule-based threat classification |

---

## 📊 Results

| Metric | Value |
|---|---|
| Overall Prediction Accuracy | **85%** |
| Best Performing Models | Logistic Regression & SVM |
| Most Predictable Threat | Spyware / Ransomware |
| Second Most Predictable | Spear Phishing |
| Evaluation Method | TPR (True Positive Rate) & FPR (False Positive Rate) |

---

## 📁 Project Structure

```
cyber-threat-predictive-analytics/
│
├── dataset/
│   └── cyber_threat_data.csv          # Breach dataset
│
├── models/
│   ├── logistic_regression.py         # LR classifier
│   ├── svm_model.py                   # SVM classifier
│   ├── random_forest.py               # RF classifier
│   └── decision_tree.py              # DT classifier
│
├── web/
│   ├── index.html                     # Web interface
│   └── styles.css                     # Stylesheet
│
├── cyber_threat.py                    # Main prediction script
├── cyber_model.py                     # Model training & evaluation
├── requirements.txt                   # Python dependencies
└── README.md                          # Project documentation
```

---

## ✅ Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Windows 7 / 8 / 10 or Linux / macOS
- Minimum 4 GB RAM

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cyber-threat-predictive-analytics.git
cd cyber-threat-predictive-analytics
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## ▶️ How to Run

### Train & Evaluate Models
```bash
python cyber_model.py
```

### Run Threat Prediction
```bash
python cyber_threat.py
```

### Launch Web Interface
Open `web/index.html` in any modern browser to view prediction results and visualisations.

---

## 💻 System Requirements

| Component | Specification |
|---|---|
| Processor | Intel (any generation) |
| RAM | 4 GB minimum |
| Storage | 260 GB Hard Disk |
| Operating System | Windows 7 / 8 / 10 (32-bit & 64-bit) |

---

## 🚀 Advantages Over Existing Systems

- ✅ **Proactive** threat mitigation via predictive analytics — not reactive incident response
- ✅ **Holistic coverage** of the entire supply chain, including third-party providers
- ✅ **Real-time threat intelligence** integration for rapid adaptation to new attack vectors
- ✅ **Automated detection** reduces response time significantly
- ✅ **Data-driven insights** for smarter security resource allocation
- ✅ **Adaptable model** that evolves alongside the changing threat landscape

---

## 🔭 Future Scope

- Integration with live threat feeds (MISP, OpenCTI)
- Deep Learning models (LSTM, Transformers) for time-series breach prediction
- Automated control recommendations based on NIST / MITRE ATT&CK frameworks
- Cloud deployment for real-time CSC monitoring dashboards
- Multi-tier supply chain graph analysis using Graph Neural Networks

---

## 👤 Author

**Suresh**  
B.Tech — Cyber Security | Sri Indu Institute of Engineering and Technology (JNTUH)

[![GitHub](https://img.shields.io/badge/GitHub-your--username-black?style=flat&logo=github)](https://github.com/your-username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-your--profile-blue?style=flat&logo=linkedin)](https://linkedin.com/in/your-profile)

---

<div align="center">

⭐ If this project helped you, consider giving it a star on GitHub!

</div>

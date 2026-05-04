# ⚡ Energy Consumption and Optimization Using AI

> A hybrid AI pipeline combining **Fuzzy C-Means Clustering**, **LSTM Forecasting**, and **Reinforcement Learning Optimization** — analysing 54,170 real energy records from 2019 to 2025.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Website-blue?style=for-the-badge)](https://vamsi-21861.github.io/energy-ai)
[![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)](https://tensorflow.org)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-yellow?style=flat-square&logo=googlecolab)](https://colab.research.google.com)

---

## 👨‍💻 Authors

| Name | Roll Number |
|------|-------------|
| K. Manideep | 22UECS0349 |
| R. Sathya Vamsi | 22UECS0570 |

**Institution:** Vel Tech Rangarajan Dr. Sagunthala R&D Institute of Science and Technology  
**Department:** B.Tech Computer Science Engineering  
**Batch:** MA1533

---

## 🎯 Project Overview

This project proposes a 3-stage hybrid AI pipeline for smart energy management:

```
Stage 1: FCM Clustering       → Group energy records into Low / Medium / High usage
Stage 2: LSTM Prediction      → Forecast future energy consumption
Stage 3: RL Optimization      → Reduce peak loads and minimize costs
```

---

## 📊 Results

| Metric | Value |
|--------|-------|
| R² Score | 0.9633 |
| MAE | 133.22 |
| RMSE | 193.31 |
| MAPE | 2.11% |
| Peak Load Reduction | 15% |
| Energy Cost Saving | 7.89% |
| Total Cost Saved | ₹2,65,96,366 |
| FPC Score (Clustering) | 0.7739 |

---

## 🗂️ Repository Structure

```
energy-ai/
│
├── index.html                              # Live website (GitHub Pages)
├── Energy_Consumption_Optimization_Project.ipynb   # Main Colab notebook
├── data.csv                                # Dataset (54,170 records)
└── README.md                               # Project documentation
```

---

## 🔧 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10 | Core programming |
| TensorFlow / Keras | LSTM model training |
| Scikit-fuzzy | FCM clustering |
| Pandas & NumPy | Data processing |
| Plotly & Matplotlib | Visualizations |
| Google Colab | Training environment |
| Google Sheets API | Live results sync |
| GitHub Pages | Website hosting |

---

## 🚀 How to Run

1. Open the notebook in Google Colab:
   - Click **`Energy_Consumption_Optimization_Project.ipynb`**
   - Click **"Open in Colab"** button

2. Upload `data.csv` to `/content/data.csv` in Colab

3. Run all cells: **Runtime → Run All**

4. Last cell saves results to Google Sheets and generates live dashboard link

---

## 🌐 Live Website

👉 **[https://vamsi-21861.github.io/energy-ai](https://vamsi-21861.github.io/energy-ai)**

- Auto-synced with Google Sheets after every Colab run
- Interactive charts and metrics dashboard
- AI-powered chatbot for project Q&A

---

## 📈 Model Architecture

### FCM Clustering
- 3 clusters: High (13,294) / Medium (22,359) / Low (18,517)
- FPC Score: 0.7739 (Good quality)

### LSTM Network
```
Input → LSTM(64) → Dropout(0.2) → LSTM(32) → Dropout(0.2) → Dense(16) → Output
```
- 24-step sliding windows
- EarlyStopping at Epoch 13
- 5-Fold Cross Validation: Mean R² = 0.9701 ± 0.0058

### Reinforcement Learning
- State: Predicted consumption value
- Action: Shift load / Maintain usage
- Reward: Cost reduction achieved
- Result: 15% Peak Load Reduction

---

## 📋 Standards Followed

- ISO/IEC 27001 — Information Security
- ISO/IEC 12207 — Software Life Cycle
- ISO/IEC 25010 — Software Quality

---

## 📄 License

This project is submitted as a B.Tech Major Project at Vel Tech R&D Institute. All rights reserved © 2026.

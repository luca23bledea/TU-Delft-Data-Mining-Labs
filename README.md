# TU Delft Data Mining Labs  
*A collection of implementations for anomaly detection and recommender systems, based on the 2025–2026 Data Mining course at TU Delft.*

---

## 📂 Overview

This repository contains my solutions for two major Data Mining labs:

1. **Anomaly Detection in Multivariate Sequential Data (SCADA Systems)**
2. **Collaborative Filtering for Recommendation Systems (Breeze Dating Platform)**

Both labs focus on applying core data mining techniques to real-world, messy, and unlabeled datasets. The goal is to build full pipelines — from data loading to evaluation — using methods taught in class.

---

# 🔍 Lab 1 — Anomaly Detection in SCADA Systems

Modern SCADA systems generate **multivariate, sequential, and unlabeled** data.  
This makes anomaly detection challenging because:

- Data points are **not i.i.d.** — past values influence future ones  
- Labels are unavailable  
- Sequential structure matters  
- Multivariate signals interact in complex ways  

In this lab, I implemented two fundamentally different anomaly detection approaches.

---

## 🧠 Learning Outcomes

- Implement **Dynamic Time Warping (DTW)** for sequential distance computation  
- Use **nearest-neighbor distance thresholds** for anomaly detection  
- Apply **Principal Component Analysis (PCA)** for matrix factorization  
- Detect anomalies in **multivariate sequential data**  
- Build and evaluate a full anomaly detection pipeline  

---

## 🛠 Methods Implemented

### **1. Dynamic Time Warping (DTW)**  
A distance measure for sequences that allows non-linear alignment.  


### **2. PCA-Based Anomaly Detection**  
Here, sequential structure is ignored.  
Instead, anomalies are detected when feature combinations **never observed during training** appear in test data.

---

# 💘 Lab 2 — Recommender Systems (Breeze Dating Platform)

This lab focuses on **collaborative filtering**, using real anonymized data from Breeze — a Dutch dating startup.

The dataset contains:

- Users rating suggested matches  
- `1` = like  
- `0` = dislike  
- `np.nan` = no interaction  

The goal is to predict whether a user will like a new suggested match.

---

## 🧠 Learning Outcomes

- Implement **Non-Negative Matrix Factorization (NMF)**  
- Implement **Min-Hashing** for fast Jaccard similarity  
- Build recommendation pipelines for different user types  
- Evaluate recommender system performance  

---

## 🛠 Methods Implemented

### **1. Non-Negative Matrix Factorization (NMF)**  

### **2. Min-Hashing + Jaccard Distance**  
Even though the dataset fits in memory, min-hashing is required to:

- Approximate Jaccard similarity efficiently  
- Enable scalable nearest-neighbor search  
- Demonstrate hashing-based collaborative filtering  

---

# 🚀 How to Run

1. Clone the repository  
2. Install dependencies  
3. Open the notebooks in Jupyter or VS Code  
4. Run each cell sequentially  

Each notebook is self-contained and includes explanations, visualizations, and evaluation metrics.

---

# 🧑‍💻 Authors

**Luca Bledea**<br>
**Tudor Berechet** <br>
TU Delft — Data Mining (2025–2026)


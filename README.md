# Glacier calving 
# Glacier Calving Risk Prediction Using Satellite Velocity Anomalies and Graph Neural Networks

A spatiotemporal deep learning framework for forecasting glacier calving risk using satellite-derived glacier velocity anomalies, graph neural networks, and Transformer-based temporal learning. 

---

## Overview

Glacier calving is one of the major contributors to glacier mass loss and global sea-level rise. Traditional glacier monitoring approaches mainly focus on post-event analysis, glacier-front extraction, and velocity estimation, with limited capability for predicting future glacier instability.

This project proposes a **Spatiotemporal Graph Attention Network (ST-GATT)** framework that combines:

* Satellite-derived glacier velocity observations
* Temporal anomaly detection
* Graph Neural Networks (GNNs)
* Transformer-based forecasting

to predict glacier calving risk within a **2–4 week forecasting horizon**.

The framework analyzes temporal glacier velocity anomalies using **STL decomposition** and **Z-score anomaly detection**, models glacier regions as interconnected graph nodes, and learns evolving spatial-temporal glacier dynamics for early-warning prediction. 

---

# Key Features

* Satellite-based glacier velocity analysis
* Temporal anomaly detection using STL decomposition
* Z-score based glacier instability identification
* Spatial graph construction of glacier regions
* Graph Attention Network (GAT) for spatial learning
* Transformer-based temporal forecasting
* Glacier calving risk prediction
* Spatial risk heatmap generation
* Early-warning glacier instability monitoring

---

# Proposed ST-GATT Framework

The framework consists of the following stages:

1. Satellite Data Acquisition
2. Glacier Velocity Map Generation
3. Temporal Anomaly Detection
4. Spatial Graph Construction
5. Graph Attention-Based Spatial Learning
6. Transformer-Based Temporal Forecasting
7. Glacier Calving Risk Prediction
8. Early Warning and Risk Visualization

---

# Methodology

## 1. Satellite Velocity Analysis

Satellite-derived glacier velocity maps are generated from temporal SAR observations to analyze glacier movement patterns over time.

## 2. Temporal Anomaly Detection

The glacier velocity time-series is decomposed using:

* STL (Seasonal-Trend decomposition using Loess)
* Z-score anomaly detection

to identify abnormal glacier acceleration patterns associated with potential calving events.

## 3. Spatial Graph Construction

The glacier surface is partitioned into spatial patches where:

* Nodes represent glacier regions
* Edges represent spatial interaction and stress propagation

This graph structure models spatial glacier dynamics.

## 4. ST-GATT Architecture

The proposed architecture combines:

### Graph Attention Network (GAT)

Captures spatial dependencies and glacier-region interactions.

### Transformer Temporal Module

Learns temporal evolution of glacier instability patterns across sequential observations.

## 5. Risk Prediction

The framework predicts:

* Glacier calving probability
* Spatial risk heatmaps
* Early-warning instability regions

within a 2–4 week prediction window.

---

# Experimental Results

The proposed framework achieved:

| Metric | Score  |
| ------ | ------ |
| AUROC  | 0.9444 |
| AUPRC  | 0.8333 |

The results demonstrate strong capability in distinguishing stable glacier conditions from pre-calving instability patterns. 

---

# Technologies Used

* Python
* PyTorch
* PyTorch Geometric
* NumPy
* SciPy
* Statsmodels
* Scikit-learn
* Matplotlib
* Seaborn

---

# Dataset

The framework uses:

* Satellite-derived glacier velocity observations
* Sentinel-1 SAR-based glacier velocity maps
* Temporal glacier motion sequences

for anomaly-aware glacier forecasting.

---

# Visual Outputs

The framework generates:

* Glacier velocity maps
* STL decomposition plots
* Z-score anomaly maps
* Graph topology visualizations
* Spatial calving risk heatmaps
* Temporal anomaly propagation maps
* Training performance curves
* Confusion matrices

---

# Project Structure

```bash
├── data/
├── preprocessing/
├── anomaly_detection/
├── graph_construction/
├── models/
│   ├── gat_module.py
│   ├── transformer_module.py
│   └── st_gatt_model.py
├── training/
├── evaluation/
├── visualization/
├── results/
├── figures/
├── main.py
└── README.md
```

---

# Future Work

* Integration with real-time satellite streams
* Multi-glacier large-scale deployment
* Climate-aware forecasting integration
* Physics-informed glacier modeling
* Higher-resolution spatial graph modeling
* Real-time operational warning systems

---

# Applications

* Glacier instability monitoring
* Climate-risk assessment
* Polar-region environmental monitoring
* Cryosphere analysis
* Early-warning systems
* GeoAI and remote sensing research

---

# Citation

If you use this work, please cite:

```bibtex
@article{
  title={Glacier Calving Risk Prediction Using Satellite Velocity Anomalies and Graph Neural Networks},
  author={Sharma, Harshita},
  journal={Research Project},
  year={2025}
}
```

---

# Author

**Harshita Sharma**


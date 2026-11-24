# NetShield
### Explainable Autoencoder-CNN Hybrid Framework for Real-Time Network Intrusion Detection with Adaptive Anomaly Scoring

## Overview

NetShield is a hybrid deep learning framework designed for network intrusion detection, combining reconstruction-based anomaly detection with supervised multi-class classification.

The framework integrates an Autoencoder, CNN-based classification, adaptive anomaly scoring, and SHAP-based explainability to identify suspicious network traffic and improve detection transparency.

## Key Features

- **Anomaly Detection:** Autoencoder-based reconstruction error for identifying anomalous network traffic.
- **Multi-Class Classification:** CNN-based classification of network traffic.
- **Adaptive Threat Severity Scoring (ATSS):** Adaptive anomaly scoring and threshold recalibration to reduce false positives.
- **Explainable AI:** SHAP-based feature importance and model prediction interpretation.
- **Zero-Day Detection:** Evaluation using a held-out-class protocol.

## Technology Stack

- Python
- TensorFlow / Keras
- Scikit-learn
- Imbalanced-learn
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SHAP
- JupyterLab

## Datasets

The research evaluation uses:

- NSL-KDD
- CICIDS2017

Dataset files are not included in this repository. Obtain the datasets from their respective official sources and follow their usage conditions.

## Performance Results

| Evaluation Metric | Result |
|---|---:|
| Detection Accuracy (NSL-KDD) | 99.2% |
| Average Zero-Day Detection Rate | 78.8% |
| False Positive Reduction (ATSS) | 64.6% |
| DoS Zero-Day Detection Rate | 97.5% |
| R2L Zero-Day Detection Rate | 45.9% |

Zero-day detection results are reported under the held-out-class evaluation protocol.

## Repository Structure

```text
NetShield/
├── notebooks/
│   └── NetShield.ipynb
├── results/
│   ├── roc_curves.png
│   ├── confusion_matrix.png
│   ├── shap_global_importance.png
│   ├── shap_heatmap.png
│   ├── adaptive_threshold.png
│   └── ...
├── README.md
├── requirements.txt
└── .gitignore

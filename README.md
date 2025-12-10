# Anomaly Detection and Prognostics in Spacecraft Telemetry

**CSC 371: Machine Learning - Fall 2025**  
**Team**: Haruta Otaki, Christian Rutherford

## Project Overview

This project develops a machine learning pipeline for detecting anomalies in spacecraft telemetry data from NASA's SMAP satellite and MSL rover, with short-term fault prognostics capabilities.

## Dataset

- **Source**: NASA Anomaly Detection Dataset (SMAP/MSL) from Kaggle
- **Format**: `.npy` files, one per telemetry channel
- **Channels**: Anonymized (e.g., A-1, T-2) representing different subsystems
- **Structure**: Each file contains time-series data with 24 parallel versions of the channel

## Key Challenges

1. **Class Imbalance**: Anomalies are rare events
2. **Heterogeneous Data**: SMAP and MSL have different telemetry structures
3. **Anonymization**: Channel meanings are unknown
4. **Temporal Dependencies**: Contextual anomalies require time-series modeling

### Models to Explore
- Isolation Forest
- One-Class SVM
- KNN-based anomaly scoring
- LSTM/GRU for temporal modeling (reach goal)

## References

- NASA SMAP/MSL Dataset: [Kaggle Link](https://www.kaggle.com/datasets/patrickfleith/nasa-anomaly-detection-dataset)
- MiniRocket: [Paper](https://arxiv.org/abs/2012.08791)
- Explainable Anomaly Detection in Spacecraft Telemetry (ScienceDirect, 2024)
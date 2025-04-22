# AIHT_UNIT-4

## Network Intrusion Detection via Anomaly Score Prediction Using Autoencoder and LSTM

## Team Members

| Name         | Roll Number |
| ------------ | ----------- |
| Ayush Arora  | 2022UCA1822 |
| Aayush Bagga | 2022UCA1806 |
| Saaz Gupta   | 2022UCA1860 |

---

### **Model Description **

The proposed model for network intrusion detection integrates a deep Autoencoder with LSTM-based sequence modeling. Initially, PCA reduces dimensionality of preprocessed network traffic features, after which the Autoencoder learns compressed latent representations. Reconstruction error from this Autoencoder flags preliminary anomalies. These latent vectors are then passed through an LSTM that captures temporal dependencies, generating anomaly scores for sequences of 10 records. Scores exceeding a threshold indicate potential intrusions. Trained on the KDD Cup 1999 dataset, the system combines spatial compression and temporal analysis to identify both known and novel threats with high accuracy and minimal false positives.

---

### **Shortcomings**

1. Limited to KDD 1999, which may not reflect modern traffic patterns.
2. Dependence on handcrafted PCA may limit feature generalization.
3. Static thresholding might fail under dynamic network conditions.

---

### **Future Aspects**

1. Extend model to real-world, up-to-date datasets like CIC-IDS2017.
2. Incorporate transformer models for better temporal learning.
3. Explore adaptive thresholding and self-learning mechanisms.

[Project Report (Latex File)](https://www.overleaf.com/read/pqhsmsmfrhsw#a286a0)

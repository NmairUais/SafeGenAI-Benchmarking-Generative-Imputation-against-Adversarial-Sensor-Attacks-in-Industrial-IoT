# SafeGenAI-Benchmarking-Generative-Imputation-against-Adversarial-Sensor-Attacks-in-Industrial-IoT
SafeGenAI benchmarks how sensor-data repair affects anomaly detection in Industrial IoT systems. It simulates DoS-style missing sensor values on the SWaT dataset, repairs them using Linear Interpolation, MICE, and a Denoising Autoencoder, then evaluates the security impact using Isolation Forest, LOF, and One-Class SVM.
Codes:
Isolation Forest (Isolation Forest.py)
Trains an Isolation Forest model on normal data and evaluates anomaly detection performance on original and repaired datasets.
Linear Repair (Linear.py)
Applies simple linear interpolation to fill missing sensor values and outputs repaired datasets.
MICE Repair (MICE.py)
Uses Multiple Imputation by Chained Equations (MICE) to generate multiple repaired datasets and evaluate repair consistency.
LOF / One-Class SVM (LOF.py)
Implements LOF and One-Class SVM for anomaly detection, comparing performance across repaired datasets.
Denoising Autoencoder (Autoencoder.py)
Trains a neural network to both repair corrupted sensor values and detect anomalies using reconstruction error.

## Notes

# Anomaly detection

Application: Fraud; Network Intrusion; Cancer detection

Binary: Normal / Unknown >>> **Confidence Score**

Classifier output: Class & Confidence score

Confidence: maximum scores or negative entropy

Ref: Terrance DeVries, Graham W. Taylor, Learning Confidence for Out-of-Distribution
Detection in Neural Networks, arXiv, 2018

**Accuracy may not be a good measurement!**

False Positive & True Negative (assigned with different weights)
Ranking metric, e.g. AUC : Area under RoC 

**Possible issue: near the decision boundary; attack using a specific change(e.g. yellow color for )  **

Learn a classifier giving low confidence score:
Ref: Kimin Lee, Honglak Lee, Kibok Lee, Jinwoo Shin, Training Confidencecalibrated Classifiers for Detecting Out-of-Distribution Samples, ICLR 2018 (https://arxiv.org/abs/1711.09325)

Obtained by Generative model: 
Ref: Mark Kliger, Shachar Fleishman, Novelty Detection with GAN, arXiv, 2018 (https://arxiv.org/abs/1802.10560)

---

If Without Labels:

Learned from distribution: **Maximum Likelihood Estimation (e.g. Gaussian Distribution)

**Autoencoder**: Large reconstruction loss >>> anomaly

One class SVM; Isolated Forest ...


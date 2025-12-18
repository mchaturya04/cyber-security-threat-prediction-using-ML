# cyber-security-threat-prediction-using-ML
**Overview**

This project presents a machine learning–based framework for predicting and classifying cybersecurity threats using historical network traffic data. Traditional rule-based intrusion detection systems often fail to detect evolving and previously unseen attacks. To address this limitation, this project applies supervised machine learning models to identify malicious traffic patterns with improved accuracy, scalability, and interpretability.
The solution is developed as part of a capstone project at the University of New Haven and uses the CICIDS2017 dataset, a widely accepted benchmark for intrusion detection research.

**Problem Statement**

Modern organizations face increasing cybersecurity risks due to sophisticated attacks such as DDoS, Port Scans, and brute-force intrusions. Signature-based systems are reactive and struggle with zero-day or adaptive threats. There is a need for intelligent, data-driven systems capable of learning from historical traffic and proactively predicting malicious behavior.

**Dataset**

**Dataset**: CICIDS2017 (Canadian Institute for Cybersecurity)
**Data Type**: Network flow–based traffic records
**Size**: ~2.8 million labeled records
**Attack Types Covered:**
DDoS (Hulk, LOIC)
DoS (GoldenEye, Slowloris, SlowHTTPTest)
PortScan (Nmap, Xmas)
Brute-Force (SSH, FTP)
BENIGN traffic

**Tools & Technologies**

**Programming Language**: Python
**Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
**Environment:** Jupyter Notebook / Google Colab
**Visualization**: Power BI, Matplotlib, Seaborn

**Methodology**

**1.Data Collection & Merging**
  Combined all eight CICIDS2017 CSV files into a unified dataset
**2.Data Preprocessing**
  Removed missing and infinite values
  Converted multiclass labels into binary classes (BENIGN vs ATTACK)
  Standardized numerical features using Z-score normalization
**3.Exploratory Data Analysis (EDA)**
  Feature distribution analysis
  Outlier visualization using boxplots
  Correlation analysis using heatmaps
**4.Model Development**
  Logistic Regression
  Gaussian Naive Bayes
  Decision Tree Classifier
**5.Model Evaluation**
  Accuracy
  Precision, Recall, F1-Score
  Confusion Matrix
  ROC-AUC

**Results & Key Findings**

Decision Tree achieved the highest accuracy (99.97%) with near-perfect precision and recall, though it shows signs of overfitting.

Logistic Regression delivered strong and balanced performance (94.02% accuracy) with high interpretability, making it suitable for lightweight IDS deployment.

Naive Bayes demonstrated high recall for attack detection but suffered from low precision and a high false-positive rate.

These results demonstrate that even lightweight and interpretable machine learning models can effectively detect cybersecurity threats when supported by strong preprocessing pipelines.

**Future Enhancements**
Implement ensemble models (Random Forest, Gradient Boosting)
Explore deep learning approaches
Integrate real-time traffic ingestion
Improve probability calibration and AUC performance

**Author**
Mittapally Chaturya

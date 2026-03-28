MACHINE LEARNING-BASED ANOMALY DETECTION FRAMEWORK
FOR SECURING CLOUD ENVIRONMENTS USING THE UNSW-NB15 DATASET
📌 Overview
Cloud computing has revolutionized modern IT infrastructure by providing scalable, flexible, and cost-effective solutions. However, this rapid growth has also increased the risk of cyber threats such as Denial-of-Service (DoS), probing, reconnaissance, and exploitation attacks. Traditional Intrusion Detection Systems (IDS), which rely on signature-based techniques, are often unable to detect unknown attacks and adapt to dynamic cloud environments.
This project presents a Machine Learning-based Anomaly Detection Framework designed to enhance cloud security. By leveraging the UNSW-NB15 dataset and advanced machine learning techniques, the system detects abnormal network behavior and classifies it as normal or malicious in real time.

🎯 Objectives
Detect anomalies in network traffic
Improve detection of unknown (zero-day) attacks
Reduce false positives in intrusion detection
Enable real-time monitoring and alerting
Provide a scalable solution for cloud environments

🗂️ Dataset
The project uses the UNSW-NB15 dataset, which contains realistic network traffic data with both normal and malicious activities. It includes multiple attack categories such as DoS, exploits, reconnaissance, and generic attacks.
📌 Note: Due to large size, the dataset is not included in this repository.
Download link:
https://research.unsw.edu.au/projects/unsw-nb15-dataset

⚙️ Methodology
The proposed system follows a structured approach to detect anomalies effectively:
Data Preprocessing: Cleaning data, handling missing values, encoding categorical features, and normalizing numerical values.
Feature Selection: Using Mutual Information to select the most relevant features.
Model Training: Training an XGBoost classifier to learn patterns of normal and malicious traffic.
Real-Time Processing: Simulating streaming data using Kafka-like architecture.
Prediction & Alerts: Classifying incoming traffic and generating alerts for detected attacks.
Visualization: Displaying results using an interactive dashboard.

🧠 Technologies Used
Python
Pandas, NumPy
Scikit-learn
XGBoost
Matplotlib, Seaborn
Gradio (for dashboard)

📊 Results
The proposed XGBoost model demonstrates high performance in anomaly detection:
Accuracy: 98.6%
Precision: 97.9%
Recall: 98.2%
F1-Score: 98.0%
ROC-AUC: 0.99
The system efficiently detects both known and unknown attacks with low false positives and supports real-time analysis.

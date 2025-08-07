# Power-Fault-Detector
The objective of this project is to enable a accurate fault identification for maintaining power grid reliability.

## 🔍 Project Overview

This project aims to develop a machine learning model that can automatically detect and classify different types of electrical faults in a power distribution system. The model leverages **IBM AutoAI** within **Watson Studio** to automate the end-to-end machine learning workflow, including data preprocessing, model selection, training, and deployment.

---

## ⚡ Problem Statement

Electric power systems are susceptible to various types of faults such as line-to-ground, line-to-line, and three-phase faults. Rapid and accurate detection of these faults is crucial for maintaining grid stability and minimizing downtime.

---

## ✅ Proposed Solution

Using IBM Cloud Lite services, particularly AutoAI in Watson Studio, a machine learning model is trained on electrical phasor data (voltage and current) to classify system conditions into normal or specific fault types. The model is deployed using Watson Machine Learning, enabling real-time fault detection via REST APIs.

---

## 🛠️ Technologies Used

- IBM Cloud Lite
- IBM Watson Studio
- IBM AutoAI
- IBM Cloud Object Storage
- IBM Watson Machine Learning
- Python (for local preprocessing/analysis if needed)

---

## 🧪 Dataset

- Source: [Kaggle - Power System Faults Dataset](https://www.kaggle.com/datasets/ziya07/power-systemfaults-dataset)
- Data includes voltage and current phasors for various fault scenarios.

---

## 🚀 System Workflow

1. Dataset uploaded to IBM Cloud Object Storage.
2. AutoAI experiment created in Watson Studio.
3. Target column (`Fault_Type`) selected.
4. AutoAI automatically:
   - Preprocesses data
   - Selects optimal ML pipeline
   - Trains and validates models
   - Ranks models based on performance metrics
5. Best model deployed using Watson Machine Learning.
6. Endpoint created for real-time prediction.

---

## 🧠 Model Performance

- Algorithm Used: Random Forest (selected by AutoAI)
- Accuracy Achieved: ~95%
- Deployed Endpoint: Watson Machine Learning (Lite plan)

---

## 📈 Future Scope

- Integrate real-time streaming data for live fault detection.
- Expand model to detect transient and symmetrical faults.
- Utilize deep learning models for improved accuracy.
- Deploy lightweight models on edge devices for faster on-site detection.

---

## 📚 References

- [Kaggle Dataset](https://www.kaggle.com/datasets/ziya07/power-systemfaults-dataset)
- [IBM AutoAI Docs](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=services-autoai)

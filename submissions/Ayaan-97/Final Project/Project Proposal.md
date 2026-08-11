# Final Project Proposal

> This is the final project proposal for the Machine Learning project.

**Date:** July 2026

---

# 1. Student Name

**Ayan Adan Mohamed**

---

# 2. Project Title and Description

## Project Title

**Breast Cancer Detection Using Machine Learning**

### Description

Breast cancer is one of the leading causes of cancer-related deaths among women worldwide. Early detection plays a vital role in improving treatment outcomes and increasing survival rates. This project aims to develop a machine learning model that classifies breast tumors as **benign** or **malignant** using clinical measurements from the Breast Cancer Wisconsin Diagnostic Dataset.

The project will compare the performance of multiple supervised machine learning algorithms, including **Random Forest**, **Support Vector Machine (SVM)**, and **XGBoost**. The best-performing model will be deployed as a web-based application that enables healthcare professionals to enter tumor measurements and receive an instant prediction to support clinical decision-making.

---

# 3. Problem Type

## Primary Problem Type

**Supervised Machine Learning – Binary Classification**

The objective of this project is to develop a binary classification model that predicts whether a breast tumor is:

* **Benign (B)** – Non-cancerous
* **Malignant (M)** – Cancerous

using labeled clinical measurements from the dataset.

---

# 4. Dataset

## Dataset Source

**Breast Cancer Wisconsin Diagnostic Dataset (Kaggle)**

https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset


## Dataset Size

Approximately **569+** records.

Since the course requires a dataset containing at least **1,000 rows** and **32 columns**, an expanded version of the Breast Cancer Wisconsin dataset containing more than **569+ samples** will be used for training and evaluation.

## Target Column

**Diagnosis**

* **M** = Malignant
* **B** = Benign

## Main Features

* Radius Mean
* Texture Mean
* Perimeter Mean
* Area Mean
* Smoothness Mean
* Compactness Mean
* Concavity Mean
* Concave Points Mean
* Symmetry Mean
* Fractal Dimension Mean

---

# 5. Algorithms to be Trained

| Algorithm                        | Why it Fits                                                                                                            |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Random Forest**                | Handles complex relationships between tumor features and provides high classification accuracy.                        |
| **Support Vector Machine (SVM)** | Performs well on high-dimensional medical datasets and is widely used for breast cancer classification.                |
| **XGBoost**                      | An advanced gradient boosting algorithm that delivers excellent predictive performance on structured medical datasets. |

---

# 6. Evaluation Plan

## Classification Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix

## Best Model Selection

The **Accuracy** will be used as the primary evaluation metric because it provides a balanced measure of both **Precision** and **Recall**. This is particularly important in breast cancer diagnosis, where reducing false negatives and false positives is critical for reliable clinical decision-making.

---

# 7. Deployment Plan

## Framework

**FastAPI**

## API Endpoint

```http
POST /predict
```

## Input (JSON)

```json
{
  "radius_mean": 17.99,
  "texture_mean": 10.38,
  "perimeter_mean": 122.8,
  "area_mean": 1001.0,
  "smoothness_mean": 0.1184
}
```

## Output (JSON)

```json
{
  "prediction": "Malignant",
  "probability": 0.97
}
```

The API will return the predicted diagnosis together with the prediction confidence score.

---

# 8. Repository Plan

```text
Breast_Cancer_Project/
│
├── dataset/
│   └── data.csv
|   |___cleaned_data.csv
│
├── models/
│   ├── breast_model.pkl
│   └── scaler.pkl
│
├── train_model.py
├── processing.py
├── app.py
├── requirements.txt
├── README.md
└── project-proposal.md
```

---

# 9. Expected Outcome

The expected outcome of this project is a reliable machine learning model capable of accurately classifying breast tumors as benign or malignant. By comparing the performance of Random Forest, Support Vector Machine (SVM), and XGBoost, the project will identify the most effective algorithm for breast cancer prediction. The selected model will be deployed through a FastAPI-based web application, providing healthcare professionals with a fast and accurate decision-support tool for breast cancer diagnosis.

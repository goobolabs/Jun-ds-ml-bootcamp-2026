# 🎗️ Breast Cancer Prediction System

A full-stack web application that uses Machine Learning to predict whether a breast tumor is **Benign** or **Malignant** based on measurements from the Wisconsin Diagnostic Breast Cancer dataset.

The system provides a simple and modern interface where users can enter tumor measurements and receive a machine-learning prediction with a confidence score.

---

## 📌 Project Overview

Breast cancer is one of the most common cancers affecting women worldwide. Early detection can help healthcare professionals make informed decisions about further diagnosis and treatment.

This project demonstrates how Machine Learning can be integrated into a web application to classify breast tumors into two categories:

- 🟢 **Benign** — non-cancerous
- 🔴 **Malignant** — cancerous

The application consists of:

- A **Next.js frontend**
- A **Flask/Python backend**
- A trained **Machine Learning classification model**
- A REST API connecting the frontend and backend

> ⚠️ **Important:** This project is for educational and research purposes. It is not a medical diagnostic tool and should not replace professional medical advice.

---

# 🎯 Project Objectives

The main objectives of this project are:

1. Build a web-based breast cancer prediction system.
2. Apply Machine Learning to breast tumor classification.
3. Provide a simple interface for entering tumor measurements.
4. Predict whether a tumor is Benign or Malignant.
5. Display the prediction confidence.
6. Connect a React/Next.js frontend to a Flask backend.
7. Demonstrate the practical use of Machine Learning in healthcare applications.

---

# 🧠 Machine Learning

## Dataset

This project uses the:

**Wisconsin Diagnostic Breast Cancer (WDBC) Dataset**

The dataset contains measurements calculated from digitized images of fine-needle aspirate (FNA) of breast masses.

Important features used by this application include:

| Feature | Description |
|---|---|
| Radius | Mean distance from center to perimeter |
| Texture | Variation in gray-scale values |
| Perimeter | Tumor perimeter |
| Area | Tumor area |
| Smoothness | Local variation in radius lengths |
| Compactness | Perimeter² / area relationship |
| Concavity | Severity of concave portions |
| Concave Points | Number/severity of concave points |
| Symmetry | Tumor symmetry |
| Fractal Dimension | Approximation of tumor boundary complexity |

---

# 🤖 Classification

The problem is a **binary classification problem**.

The model predicts:

```text
0 → Benign
1 → Malignant
```

## 🔗 Repository

Project source: https://github.com/Ayaan-97/Breast-Cancer-Prediction.git

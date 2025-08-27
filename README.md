# 🧠 Comparative Analysis of ML Techniques on Heart Disease Dataset
This project aims to analyze and compare the performance of various machine learning models on a heart disease dataset, focusing not just on prediction, but on understanding how each model performs under the same conditions using different evaluation metrics.

## 📁 Dataset
This dataset consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It has 76 attributes, including the predicted attribute, but all published experiments use only 14 of them. The presence of heart disease in the patient is referred to as the target field.

### 🎯 Target Column
The target field represents the patient's risk of developing heart disease. It is represented by the binary numbers 0 (lower risk of heart attack) and 1 (higher risk of heart attack).
📌 **Source:** https://archive.ics.uci.edu/dataset/45/heart+disease

## 🧬 Features
| Feature     | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `age`       | Age in years                                                                |
| `sex`       | Sex (1 = male, 0 = female)                                                  |
| `cp`        | Chest pain type (0–3)                                                       |
| `trestbps`  | Resting blood pressure                                                      |
| `chol`      | Serum cholesterol (mg/dl)                                                   |
| `fbs`       | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)                       |
| `restecg`   | Resting electrocardiographic results (0–2)                                  |
| `thalach`   | Maximum heart rate achieved                                                 |
| `exang`     | Exercise-induced angina (1 = yes, 0 = no)                                   |
| `oldpeak`   | ST depression induced by exercise                                           |
| `slope`     | Slope of the peak exercise ST segment (0–2)                                 |
| `ca`        | Number of major vessels (0–3)                                               |
| `thal`      | Blood disorder called thalassemia (0 = NULL, 1–3 for types)                 |

## 📊 Machine Learning Models Evaluated
This project evaluates the performance of three core machine learning approaches:

### 🔵 K-Means Clustering (Unsupervised)
- **Purpose**: Discover patterns without labeled data
- **Tuning**: Optimal `k` via Elbow Method
- **Evaluation**: Silhouette Score, Accuracy  
- **Accuracy**: `44.88%`

### 🟢 Support Vector Machine (SVM)
- **Purpose**: Supervised classification with linear kernel
- **Evaluation**: F1-Score, Precision, Recall, Accuracy  
- **Accuracy**: `81.46%`

### 🟣 K-Nearest Neighbors (KNN)
- **Purpose**: Instance-based learning
- **Tuning**: Optimal `k` via Elbow Method
- **Evaluation**: F1-Score, Confusion Matrix, Accuracy  
- **Accuracy**: `98.54%`

## 🧪 Workflow Summary
- Loaded and explored the dataset
- Handled missing values and class imbalance
- Performed EDA (correlation heatmaps, boxplots)
- Scaled data using StandardScaler and RobustScaler
- Trained and evaluated:
  - K-Means Clustering
  - SVM (Support Vector Machine)
  - KNN (K-Nearest Neighbors)
- Compared models using F1-Score, Accuracy, and Silhouette Score

## 📊 Evaluation Metrics Used
- **Accuracy Score**
- **F1-Score**
- **Precision & Recall**
- **Confusion Matrix**
- **Silhouette Score** (for unsupervised clustering)

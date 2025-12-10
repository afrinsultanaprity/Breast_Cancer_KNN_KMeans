# Breast Cancer Diagnosis Prediction Using KNN & KMeans

This project focuses on analyzing the Breast Cancer to classify tumors as **Benign (B)** or **Malignant (M)** using both **Unsupervised** and **Supervised** machine learning techniques.

Two methods were applied:

- **K-Means Clustering** → to explore natural grouping in the data  
- **K-Nearest Neighbors (KNN)** → to build a predictive classification model  

---

## Objectives

This work includes the following steps:

- Convert the `diagnosis` column into numeric labels  
  - **M → 1 (Malignant)**  
  - **B → 0 (Benign)**  
- Drop unnecessary columns:  
  - `id`  
  - `Unnamed: 32`  
- Normalize all feature values using **MinMaxScaler**
- Split the dataset into:  
  - **80% Training**  
  - **20% Testing**
- Apply **K-Means (k=2)** to check clustering behavior
- Train a **KNN model with k=5** using scaled training data
- Evaluate the model with standard performance metrics

---

## Methods & Workflow

### 1. Preprocessing
- Loaded the CSV dataset
- Encoded diagnosis labels (`M = 1`, `B = 0`)
- Cleaned unused or empty columns
- Normalized all numeric features for consistent scale

### 2. K-Means Clustering
- Used **k = 2**, ideal for two classes
- Compared assigned clusters with actual diagnosis labels

### 3. KNN Classification
- Utilized **KNeighborsClassifier**
- Model was trained on normalized training data
---

##  Model Evaluation

| Metric        | Score |
|---------------|------------------|
| Accuracy      | ~0.95–0.97       |
| Precision     | ~0.95            |
| Recall        | ~0.95            |
| F1-score      | ~0.95            |



---

## Files Included

- **`Breast_Cancer_Analysis.ipynb`**  
  Full notebook with preprocessing, clustering, classification, and evaluation.

- **`Dataset - Dataset.csv`**  
  The dataset used in this project.

- **`README.md`**  
  Documentation summarizing the project.

---

## Run process

1. Open the notebook in **Google Colab** or **Jupyter Notebook**  
2. Upload the dataset  
3. Run cells 
4. View the output and scores




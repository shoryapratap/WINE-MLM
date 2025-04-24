# 🍷 Wine Dataset Classification using K-Nearest Neighbors (KNN)

This project demonstrates a full machine learning pipeline to classify wine samples into one of three categories using the **K-Nearest Neighbors (KNN)** algorithm. It includes data loading, preprocessing, model training, evaluation, and insightful visualizations.

---

## 📁 Project Structure


---

## 📚 Dataset

- **Source**: [Wine dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html)
- **Description**: Contains 178 wine samples with 13 chemical analysis features.
- **Classes**:
  - Class 0: Cultivar 1
  - Class 1: Cultivar 2
  - Class 2: Cultivar 3

---

## 🚀 Workflow Overview

### 1. **Import Required Libraries**

Includes:
- `numpy`, `matplotlib`
- `scikit-learn` modules for model, preprocessing, and metrics

### 2. **Load and Explore the Dataset**

- Display feature names and target names
- Show sample entries
- Print class distribution

### 3. **Preprocess the Data**

- Train-test split with `stratify` for balanced class representation
- Standardize features with `StandardScaler`

### 4. **Train the KNN Model**

- Use `KNeighborsClassifier` with `k=5`
- Fit on the standardized training data

### 5. **Make Predictions**

- Predict wine class labels on the test data

### 6. **Evaluate the Model**

- Print **confusion matrix**
- Show **classification report** (precision, recall, F1-score)
- Display overall **accuracy**

### 7. **Visualize Confusion Matrix**

- Use `ConfusionMatrixDisplay` for intuitive evaluation

### 8. **Visualize Feature Relationships**

- Plot a 2D scatter plot using two selected features:
  - `Alcohol` (feature 0)
  - `Color Intensity` (feature 9)

### 9. **Analyze Feature Importance (Mean Profile per Class)**

- Visual comparison of feature means for each class using horizontal bar plots
- Helps identify distinctive characteristics of wine classes

---

## 📊 Results

- **Accuracy**: ~96–98% on the test set (may vary based on train-test split)
- Insights from visualizations:
  - Alcohol and color intensity offer good separation between classes
  - Clear patterns in mean feature values per wine class

---

## 📦 Requirements

Install dependencies using:

```bash
pip install numpy matplotlib scikit-learn


📌 How to Run

python wine_knn_classifier.py

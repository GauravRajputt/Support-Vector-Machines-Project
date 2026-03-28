# 🍇 Support Vector Machine (SVM) – Raisin Classification Project

## 📌 Overview

This project implements **Support Vector Machine (SVM)** to classify raisins based on their physical characteristics. It covers the complete machine learning workflow, including **data analysis, preprocessing, model training, and evaluation**.

The project demonstrates how different SVM kernels perform on structured data and how preprocessing impacts model performance.


---

## 📊 Dataset

The dataset contains geometric and shape-based features of raisins.

### Features:

- **Area** – Represents the size of the raisin  
- **Perimeter** – Measures the boundary length  
- **MajorAxisLength** – Length of the major axis  
- **MinorAxisLength** – Length of the minor axis  
- **Eccentricity** – Indicates how elongated the raisin is  
- **ConvexArea** – Area of the convex hull  
- **Extent** – Ratio of area to bounding box  

### Target:

- **Class** – Type of raisin

---

## 🔍 Exploratory Data Analysis (EDA)

### 🔹 Pairplot
<img src="Support vector machine png/Pairplot.png" width="600"/>

The pairplot provides a comprehensive view of relationships between all features. Several feature combinations show visible separation between classes, indicating that the dataset contains distinguishable patterns.

---

### 🔹 Correlation Heatmap
<img src="Support vector machine png/Correlation Heatmap.png" width="600"/>

The heatmap highlights correlations among features. Strong relationships between certain variables indicate overlapping information, which can influence model behavior.

---

### 🔹 Area vs Perimeter (Joint Plot)
<img src="Support vector machine png/Area vs Perimeter (Joint Plot).png" width="600"/>

The joint plot illustrates the relationship between area and perimeter, showing clustering patterns that reflect differences between raisin types.

---

### 🔹 PCA Visualization
<img src="Support vector machine png/PCA Visualization.png" width="600"/>

Principal Component Analysis reduces the dataset into two dimensions, making it easier to visualize class distribution. The projection shows noticeable separation between categories.

---

## ⚙️ Data Preprocessing

The dataset is prepared before model training by ensuring data quality and consistency. Missing values are handled, and features are scaled using **StandardScaler** to bring all variables to a similar range. The data is then split into training and testing sets to evaluate model performance reliably.

---

## 🤖 Model Building

Multiple SVM models are trained using different kernels to compare their effectiveness.

### 🔹 Linear SVM

The linear kernel creates a straight decision boundary and serves as a baseline model for classification.

📊 **Accuracy: 91%**

---

### 🔹 RBF Kernel SVM

The RBF kernel transforms the data into a higher-dimensional space, allowing the model to capture complex patterns and non-linear relationships.

📊 **Accuracy: 82%**

---

---

## 📊 Model Evaluation

Model performance is evaluated using standard classification metrics:

- **Accuracy** – Overall correctness of predictions  
- **Precision** – Accuracy of positive predictions  
- **Recall** – Ability to identify all relevant instances  
- **F1-score** – Balance between precision and recall  

---

## 📈 Results Summary

| Model            | Accuracy |
|------------------|----------|
| Linear SVM       | 91%      |
| RBF Kernel SVM   | 82%      |


---

## 🎯 Conclusion

The SVM algorithm performs effectively on this dataset, with the **Linear kernel achieving the highest accuracy**. The results highlight the importance of feature scaling and kernel selection when working with classification problems.

---

## 📌 Future Improvements

- Hyperparameter tuning using **GridSearchCV**  
- Feature selection and dimensionality optimization  
- Testing additional models such as Random Forest and XGBoost  

---


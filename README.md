# 📉 Customer Segmentation using PCA

## 📌 Project Overview

This project applies **Principal Component Analysis (PCA)** to customer data in order to reduce dimensionality while preserving most of the original information.

PCA helps simplify complex datasets, improve visualization, and reveal the main directions of variance within the data.

---

## 🎯 Objective

The objectives of this project are:

- Reduce data dimensionality
- Preserve the maximum amount of information
- Visualize customer data in a lower-dimensional space
- Understand the main patterns driving customer behavior

---

## 📊 Dataset Description

The dataset contains customer information including:

- Customer ID
- Gender
- Age
- Annual Income
- Spending Score (1–100)

For PCA analysis, the following features were used:

- Age
- Annual Income
- Spending Score

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

- Renamed columns for consistency
- Removed Customer ID
- Handled missing values
  - Numerical features → Median
  - Categorical features → Mode
- Standardized features using StandardScaler

Standardization is essential because PCA is sensitive to feature scales.

---

## 🧠 Principal Component Analysis (PCA)

PCA transforms the original features into a new set of uncorrelated variables called **Principal Components**.

These components capture the maximum variance present in the data while reducing dimensionality.

In this project:

- Original Features: 3
- Principal Components: 2

---

## 📈 Explained Variance

The PCA model produced the following results:

| Component | Explained Variance |
|------------|------------|
| PC1 | 91.0% |
| PC2 | 6.3% |

Total Variance Retained:

**97.3%**

This means that reducing the dataset from 3 features to 2 principal components preserved nearly all the original information.

---

## 📊 Results

After applying PCA:

- The dataset was successfully reduced from 3 dimensions to 2 dimensions.
- Most of the variance was captured by the first principal component.
- Approximately 97% of the original information was retained.
- The PCA projection did not reveal clearly separated customer groups.

---

## 🔍 Key Insights

- Customer behavior is largely driven by a dominant underlying pattern represented by the first principal component.
- PCA effectively reduced complexity without significant information loss.
- PCA improved visualization but did not directly identify customer segments.
- Clustering algorithms are still required for customer segmentation tasks.

---

## 🛠️ Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 🚀 Conclusion

PCA successfully reduced the dimensionality of the customer dataset while preserving approximately 97% of the original information.

The first principal component explained most of the variance, indicating a strong underlying structure in the data.

Although PCA simplified the dataset and improved visualization, it did not reveal clearly separated customer groups, highlighting the importance of clustering algorithms for segmentation problems.

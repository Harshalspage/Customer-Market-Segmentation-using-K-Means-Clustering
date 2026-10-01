# Customer Market Segmentation using K-Means Clustering

## 📌 Project Overview

This project focuses on **customer market segmentation** using credit card customer data. The objective is to identify groups of customers with similar purchasing and financial behavior using **unsupervised machine learning techniques**.

The project applies **K-Means Clustering**, **Principal Component Analysis (PCA)**, and an **Autoencoder** to analyze customer behavior and discover meaningful customer segments.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook

## 📊 Dataset

The dataset contains credit card customer information and behavioral attributes such as:

* Balance
* Balance Frequency
* Purchases
* One-off Purchases
* Installment Purchases
* Cash Advance
* Purchase Frequency
* Cash Advance Frequency
* Cash Advance Transactions
* Purchase Transactions
* Credit Limit
* Payments
* Minimum Payments
* Percentage of Full Payment
* Tenure

The dataset contains **8,950 customer records and 18 features**.

## 🔍 Project Workflow

### 1. Data Loading and Exploration

The dataset is loaded using Pandas and explored using:

* Dataset information
* Descriptive statistics
* Column analysis
* Missing-value analysis
* Duplicate-value analysis

### 2. Data Preprocessing

The following preprocessing steps were performed:

* Checked for missing values
* Filled missing values in `MINIMUM_PAYMENTS` and `CREDIT_LIMIT`
* Checked for duplicate records
* Removed the `CUST_ID` column
* Standardized numerical features using `StandardScaler`

### 3. Exploratory Data Analysis

Exploratory analysis was performed using:

* Distribution plots
* Pair plots
* Correlation matrix
* Correlation heatmap

The analysis helps identify relationships between customer purchasing behavior, credit limits, payments, and other financial attributes.

### 4. K-Means Clustering

K-Means clustering was applied to the standardized dataset.

The **Elbow Method** was used to examine the within-cluster sum of squares (WCSS) and investigate a suitable number of clusters.

Cluster centers were then transformed back to the original feature scale to help interpret customer behavior across the identified segments.

### 5. Principal Component Analysis

PCA was applied to reduce the dimensionality of the dataset to two principal components.

The resulting components were visualized using a scatter plot to observe the separation between customer clusters.

### 6. Autoencoder-Based Dimensionality Reduction

A neural-network-based Autoencoder was implemented using TensorFlow/Keras.

The Autoencoder learns a lower-dimensional representation of the standardized customer data. The encoded representation is then used for further clustering analysis.

K-Means clustering was subsequently applied to the encoded data, followed by PCA visualization of the resulting clusters.

## 📈 Key Techniques

| Technique                 | Purpose                                                |
| ------------------------- | ------------------------------------------------------ |
| Data Preprocessing        | Clean and prepare customer data                        |
| Exploratory Data Analysis | Understand customer behavior and feature relationships |
| StandardScaler            | Standardize numerical features                         |
| K-Means                   | Identify customer segments                             |
| Elbow Method              | Analyze an appropriate number of clusters              |
| PCA                       | Reduce dimensionality and visualize clusters           |
| Autoencoder               | Learn a lower-dimensional representation               |
| Visualization             | Explore customer segments and patterns                 |

## 📁 Project Structure

```text
Market-Segmentation/
│
├── Market_Segmentation.ipynb
├── Marketing_data.csv
└── README.md
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project folder

```bash
cd Market-Segmentation
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
```

### 4. Open the notebook

```bash
jupyter notebook Market_Segmentation.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.

## 🎯 Objective

The primary objective of this project is to demonstrate how **unsupervised machine learning and dimensionality-reduction techniques** can be applied to customer behavioral data to identify distinct customer segments.

## 👨‍💻 Author

**Harshal Shirsat**

B.Tech – Bioengineering Science & Research

---

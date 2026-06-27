# 🛍️ Customer Segmentation using Machine Learning

## 📌 Project Overview

Customer Segmentation is one of the most important applications of unsupervised machine learning. This project groups customers based on their purchasing behavior using the K-Means Clustering algorithm.

The segmentation helps businesses identify different types of customers so they can improve marketing strategies, personalize offers, increase customer satisfaction, and maximize profits.

---

## 🎯 Objectives

- Clean and preprocess real-world customer transaction data.
- Perform RFM (Recency, Frequency, Monetary) Analysis.
- Scale numerical features.
- Determine the optimal number of clusters using the Elbow Method.
- Apply K-Means Clustering.
- Visualize customer segments.
- Interpret each customer group for business decision-making.

---

## 📂 Dataset

The project uses an e-commerce transaction dataset containing customer purchase history.

### Dataset Features

| Column | Description |
|---------|-------------|
| InvoiceNo | Invoice Number |
| StockCode | Product Code |
| Description | Product Description |
| Quantity | Quantity Purchased |
| InvoiceDate | Purchase Date |
| UnitPrice | Price per Unit |
| CustomerID | Customer Identifier |
| Country | Customer Country |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Plotly
- Scikit-Learn
- Jupyter Notebook

---

## 📋 Project Workflow

### 1. Data Loading

- Load dataset using Pandas.
- Inspect data structure.
- Check missing values.
- Check duplicate records.

---

### 2. Data Cleaning

- Remove missing Customer IDs.
- Remove duplicate rows.
- Remove cancelled transactions.
- Remove negative quantities.
- Remove negative prices.

---

### 3. Feature Engineering

Create Total Amount:

```python
TotalAmount = Quantity × UnitPrice
```

Convert InvoiceDate into datetime format.

---

### 4. RFM Analysis

Create three important customer metrics.

### Recency

Days since customer's last purchase.

### Frequency

Number of purchases made.

### Monetary

Total amount spent.

---

### 5. Data Scaling

Standardize RFM values using StandardScaler.

---

### 6. Finding Optimal Clusters

Use the Elbow Method to determine the best value of K.

---

### 7. Model Building

Train K-Means Clustering model.

```python
from sklearn.cluster import KMeans

kmeans = KMeans(
    n_clusters=3,
    random_state=42
)

clusters = kmeans.fit_predict(rfm_scaled)
```

---

### 8. Cluster Visualization

Visualize clusters using:

- Scatter plots
- Pair plots
- Bar charts
- Distribution plots

---

## 📊 Results

The model segmented customers into **3 different groups**.

Example interpretation:

### Cluster 0
- High spending customers
- Frequent buyers
- Recently purchased

➡ VIP Customers

---

### Cluster 1
- Medium spending
- Average purchase frequency

➡ Regular Customers

---

### Cluster 2
- Low spending
- Inactive customers
- Long time since last purchase

➡ Lost Customers

---

## 📈 Business Benefits

Customer segmentation can help businesses:

- Personalized marketing
- Better customer retention
- Targeted promotions
- Increased sales
- Identify VIP customers
- Re-engage inactive customers

---

## 📷 Sample Visualizations

- Elbow Curve
- Cluster Scatter Plot
- RFM Distribution
- Cluster-wise Bar Charts

---



## ▶️ Installation

Clone repository

```bash
git clone https://github.com/yourusername/customer-segmentation.git
```

Move inside project

```bash
cd customer-segmentation
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run Jupyter Notebook

```bash
jupyter notebook
```

---

## 📦 Requirements

```
pandas
numpy
matplotlib
plotly
scikit-learn
jupyter
```

or

```bash
pip install pandas numpy matplotlib plotly scikit-learn jupyter
```

---

## 📌 Future Improvements

- DBSCAN Clustering
- Hierarchical Clustering
- Interactive Dashboard using Streamlit
- Power BI Dashboard
- Deploy model using Flask or FastAPI
- Automatic customer recommendation system

---

## 📚 Machine Learning Concepts Used

- Data Cleaning
- Feature Engineering
- RFM Analysis
- Standardization
- Unsupervised Learning
- K-Means Clustering
- Elbow Method
- Data Visualization

---

## 👨‍💻 Author

**Samadhan Radye**

B.Tech Computer Engineering

Interested in:
- Artificial Intelligence
- Machine Learning
- Data Science
- Web Dev

---

## ⭐ If you like this project

Give this repository a ⭐ on GitHub.

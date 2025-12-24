# E-Commerce Customer Behavior & Product Demand Analytics

Comprehensive data analytics project analyzing customer purchasing patterns, behavior segmentation, and product demand forecasting using RFM metrics and machine learning clustering.

## 🎯 Project Overview

This project leverages a dataset of 32.4M+ transactions to: 
- **Segment customers** using RFM (Recency, Frequency, Monetary) analysis
- **Identify patterns** in customer behavior and purchasing habits
- **Predict demand** for inventory optimization
- **Generate insights** for targeted marketing campaigns

## 📊 Key Features

- **RFM Segmentation**:  Classify customers into 4 distinct segments
- **Machine Learning**: K-Means clustering for customer grouping
- **Data Visualization**: Comprehensive charts and visualizations
- **Predictive Models**: Logistic Regression, Decision Trees, Random Forests
- **Business Intelligence**: Actionable insights and recommendations

## 📁 Dataset Overview

| Metric | Value |
|--------|-------|
| **Total Records** | 32.4M transactions |
| **Unique Customers** | 206,209 |
| **Unique Products** | 49,688 |
| **Departments** | 21 |
| **Aisles** | 134 |

## 📈 Customer Segments

| Cluster | Size | Type |
|---------|------|------|
| 0 | 45,390 | High-Value Customers |
| 1 | 111,570 | Regular Customers |
| 2 | 29,740 | At-Risk Customers |
| 3 | 19,509 | Inactive Customers |

## 🛠️ Technologies

- **Python 3.7+**
- **pandas, numpy** - Data manipulation
- **scikit-learn** - Machine learning
- **matplotlib, seaborn** - Visualization
- **Jupyter Notebook** - Interactive analysis

## 🚀 Quick Start

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Run Analysis
```bash
# Clone repository
git clone https://github.com/divyaprakash29/E-Commerce-Customer-Behavior-Product-Demand-Analytics.git
cd E-Commerce-Customer-Behavior-Product-Demand-Analytics

# Launch notebook
jupyter notebook Team13.ipynb
```

### Data Files Required
- `orders.csv` - Order details
- `order_products__prior.csv` - Product history
- `order_products__train.csv` - Training data
- `products.csv` - Product catalog
- `aisles.csv` - Store aisles
- `departments.csv` - Store departments

## 📂 Project Files

| File | Description |
|------|-------------|
| **Team13.ipynb** | Main analysis notebook with code & visualizations |
| **Team13.pptx** | Presentation with key findings |
| **Team13_Report.docx** | Detailed technical report |
| **README.md** | This file |

## 🔍 Analysis Includes

1. **Data Integration** - Merge multiple data sources
2. **Feature Engineering** - RFM metric calculations
3. **Clustering** - K-Means with optimal clusters
4. **Classification** - Multiple ML models
5. **Evaluation** - Accuracy, Precision, Recall, F1-Score
6. **Visualization** - Trends and patterns
7. **Insights** - Business recommendations

## 💡 Key Insights

- **54%** of customers are regular, consistent buyers
- **22%** are high-value customers requiring retention focus
- **14%** are at-risk and need re-engagement strategies
- **9%** are inactive with reactivation potential

## 📊 RFM Metrics

- **Recency**:  Days since last purchase
- **Frequency**: Total number of orders
- **Monetary**: Average basket size

## 📝 Usage Examples

```python
# Load and explore data
import pandas as pd
orders = pd.read_csv("orders.csv")

# Calculate RFM metrics
frequency = orders. groupby("user_id")["order_number"].max()
recency = orders.groupby("user_id")["days_since_prior_order"].max()

# Perform clustering
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=4, random_state=42)
clusters = kmeans.fit_predict(rfm_scaled)
```

## 📧 Contact

**Author**: [divyaprakash29](https://github.com/divyaprakash29)

## 📄 License

This project is available for educational and analytical purposes. 

---

**Status**:  Active | **Last Updated**: December 24, 2025

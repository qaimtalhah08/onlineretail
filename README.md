# Customer Analytics & Recommendation System

## Project Overview
This project implements a data-driven Customer Analytics and Recommendation System using the Online Retail dataset. The goal is to analyze customer purchasing behavior, segment customers using machine learning, and build a basic recommendation system for business insights.

---

## Dataset
- Online Retail dataset (500K+ transactions)
- Features include: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## Data Preprocessing
- Handled missing values (removed null CustomerID records)
- Removed invalid entries (negative Quantity and UnitPrice)
- Converted InvoiceDate to datetime format
- Created derived feature: **TotalPrice = Quantity × UnitPrice**

---

## Feature Engineering
Aggregated customer-level features:
- **Frequency** → Number of unique purchases
- **Monetary Value** → Total spending per customer
- **Recency** → Days since last purchase

---

## Machine Learning Approach

### 1. RFM Analysis
Used Recency, Frequency, Monetary (RFM) model to evaluate customer value.

### 2. Customer Segmentation
Applied **K-Means Clustering** after feature scaling using StandardScaler to segment customers into distinct behavioral groups.

### 3. Recommendation System
Built a basic **cosine similarity-based recommender system** to identify similar customers based on purchase behavior.

---

## Key Techniques
- Python (Pandas, NumPy)
- Data Cleaning & Transformation
- Exploratory Data Analysis (EDA)
- RFM Analysis
- K-Means Clustering
- Cosine Similarity (Recommendation System)
- Feature Scaling (StandardScaler)

---

## Business Impact
- Identified high-value and low-value customers
- Enabled customer segmentation for targeted marketing
- Improved personalization through similarity-based recommendations

---

## Future Improvements
- Deploy model using Streamlit / Flask
- Build real-time recommendation engine
- Integrate Power BI dashboard for visualization
- Improve recommender using collaborative filtering


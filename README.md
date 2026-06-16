<div align="center">

# 🛍️ Customer Segmentation using K-Means Clustering

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org)

> **Who are your customers — really?**
> Unsupervised ML to segment mall customers by income and spending behavior using K-Means Clustering.

</div>

---

## 📌 Problem Statement

Businesses treat all customers the same — but customers are not the same. This project uses **K-Means Clustering** on the Mall Customers Dataset to group customers into distinct segments based on their **Annual Income** and **Spending Score**, enabling targeted marketing, personalized strategies, and smarter business decisions.

---

## 🎯 Project Highlights

| What | Detail |
|------|--------|
| 🧠 Algorithm | K-Means Clustering (Unsupervised ML) |
| 📦 Dataset | Mall Customers Dataset |
| 📊 Key Features | Age, Annual Income (k$), Spending Score (1–100) |
| 🔍 Optimal K | Determined via Elbow Method + Silhouette Score |
| 🎯 Output | Distinct customer segments with business insights |

---

## 🗂️ Project Structure

```
customer-segmentation/
│
├── customer_segmentation.ipynb   # Jupyter Notebook — full clustering pipeline
├── requirements.txt              # Dependencies
├── images/                       # Visualization outputs
└── README.md
```

---

## 🔄 ML Pipeline

```
Load Data  →  EDA  →  Feature Selection  →  Scaling  →  Elbow Method  →  K-Means  →  Insights
```

1. **Load Data** — Mall Customers Dataset via Pandas
2. **EDA** — Pairplots, distribution graphs, correlation heatmap
3. **Outlier Detection** — Boxplots to ensure clean data
4. **Feature Selection** — Annual Income + Spending Score
5. **Feature Scaling** — StandardScaler for comparable ranges
6. **Optimal K** — Elbow Method + Silhouette Score
7. **K-Means Clustering** — Group customers into segments
8. **Visualization** — Scatter plots of distinct clusters
9. **Cluster Summary** — Avg income, spending, demographics per segment

---

## 📊 Customer Segments Discovered

| Segment | Income | Spending | Profile |
|---------|--------|----------|---------|
| 💎 Premium | High | High | Ideal target customers |
| 💰 Careful | High | Low | Price-sensitive high earners |
| 🎯 Aspirational | Low | High | Trend-driven, budget-conscious |
| 😴 Conservative | Low | Low | Minimal engagement |
| 📊 Average | Medium | Medium | Mainstream buyers |

---

## 📈 Evaluation

| Metric | Value | Purpose |
|--------|-------|---------|
| **Optimal Clusters (K)** | 5 | Determined via Elbow Method + Silhouette Score |
| **Total Customers** | 200 | Mall Customers Dataset |
| **Features Used** | 2 | Annual Income + Spending Score |
| **Elbow Method** | K=5 inflection point | Inertia minimized at K=5 |
| **Silhouette Score** | Best at K=5 | Highest cluster separation score |

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/keerthanad29/customer-segmentation.git
cd customer-segmentation

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook customer_segmentation.ipynb
```

> Or open directly in **Google Colab** — no setup needed!

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

---

## 💡 What I Learned

- Applying **K-Means Clustering** for real-world business segmentation
- Using **Elbow Method and Silhouette Score** to find optimal clusters
- Importance of **feature scaling** before clustering algorithms
- Translating cluster output into **actionable business recommendations**
- Difference between **supervised vs unsupervised** ML evaluation

---

## 🔮 Future Improvements

- [ ] Try DBSCAN or Hierarchical Clustering for comparison
- [ ] Add more features — purchase frequency, product categories
- [ ] Build an interactive customer segment explorer using Streamlit
- [ ] Apply RFM (Recency, Frequency, Monetary) analysis for deeper segmentation

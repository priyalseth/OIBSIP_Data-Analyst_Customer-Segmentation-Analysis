# Customer Segmentation Analysis using K-Means Clustering

##  Objective

The goal of this project is to segment customers based on their demographic and behavioral data using unsupervised machine learning. Identifying these segments allows businesses to deliver more personalized experiences, optimize marketing strategies, and improve customer retention.

---

##  Dataset

This project uses the `ifood_df.csv` dataset, which contains customer details including:

- Demographics: Age, Income, Education, Marital Status
- Behavioral metrics: Spending on various product categories, campaign responses
- Family info: Number of children/teens at home
- Channel activity: Website visits, catalog purchases

---

##  Tools & Technologies

- **Python** – Language used for analysis
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Data visualization
- **Scikit-learn** – Machine learning (KMeans, PCA, Scaling)
- **Google Colab** – Notebook environment

---

## Workflow

### 1. Data Loading & Inspection
- Loaded the CSV dataset
- Checked structure, null values, and statistical summary

### 2. Data Cleaning & Feature Engineering
- Removed unnecessary columns (`ID`, `Z_CostContact`, etc.)
- Created new features: `Age`, `Children`, `Total Spending`, etc.
- Handled missing values
- Encoded categorical variables
- Scaled numeric data using MinMaxScaler

### 3. Exploratory Data Analysis (EDA)
- Visualized distributions of income, age, and family size
- Generated heatmaps for correlation
- Analyzed campaign response rates and product preferences

### 4. Clustering with K-Means
- Used Elbow Method to determine the optimal number of clusters
- Applied `KMeans(n_clusters=3)` algorithm
- Assigned cluster labels to all customer entries

### 5. PCA & Cluster Visualization
- Applied Principal Component Analysis (PCA) to reduce dimensions
- Plotted customers by clusters in 2D PCA space

### 6. Cluster Profiling
- Summarized characteristics of each cluster
- Compared average income, age, total spending, family composition, and campaign engagement

---

## Key Visualizations

- PCA scatter plot showing cluster separability
- Heatmap of mean values per cluster
- Bar plots for customer behavior and demographics
- Distribution charts of income, age, and purchasing patterns

---

## Insights

- **Cluster 0**: Budget-conscious families with low income and low spending
- **Cluster 1**: High-income customers highly responsive to campaigns and promotions
- **Cluster 2**: High-income customers with consistent spending, less reactive to promotions

These segments provide actionable insights for:
- Tailored marketing campaigns
- Loyalty programs and rewards
- Targeted promotions for high-value customers

---

## Future Improvements

- Experiment with alternative clustering techniques (DBSCAN, Agglomerative)
- Integrate temporal features or customer lifecycle metrics
- Develop dashboards using Streamlit or Power BI for business users

---

> Created by [Priyal Seth]
>[LinkedIn](https://www.linkedin.com/in/priyal-seth-2493302a2/)

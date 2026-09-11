# 🛒 SmartCart — Customer Segmentation using Clustering

## Overview
An unsupervised machine learning project that segments customers of a retail 
store into distinct groups based on their demographics, spending behaviour, 
and lifestyle — enabling targeted marketing strategies.

## Dataset
smartcart_customers.csv — contains customer profiles including income, 
spending across product categories, age, education, marital status, and more.

## Tech Stack
Python | scikit-learn | pandas | matplotlib | seaborn | KneeLocator | PCA

## Key Highlights
- Feature Engineering: Age, Customer Tenure, Total Spending, Total Children,
  simplified Education and Living Status columns
- Outlier removal based on Age and Income thresholds
- One-Hot Encoding for categorical features
- StandardScaler normalization
- PCA (3 components) for dimensionality reduction and 3D visualization
- Optimal K selection using Elbow Method (KneeLocator) + Silhouette Score
- Two clustering algorithms compared: KMeans and Agglomerative Clustering
- Cluster characterization by Income, Spending, and Demographics

## Workflow
1. Data Cleaning → Handle missing Income values (median imputation)
2. Feature Engineering → Age, Tenure, Total Spending, simplified categories
3. Outlier Removal → Age < 90, Income < 600,000
4. Encoding + Scaling → OHE + StandardScaler
5. PCA → Reduce to 3 components for visualization
6. K Selection → Elbow + Silhouette Score combined plot
7. Clustering → KMeans (k=4) and Agglomerative Clustering (ward linkage)
8. Cluster Analysis → Income vs Spending scatter, cluster size, mean summary

## How to Run
1. Clone this repository
   git clone https://github.com/yourusername/smartcart-customer-segmentation
2. Install dependencies
   pip install -r requirements.txt
3. Open the notebook
   jupyter notebook smartcart.ipynb
4. Run all cells top to bottom

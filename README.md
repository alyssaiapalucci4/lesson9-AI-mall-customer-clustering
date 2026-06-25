## Mall Customer Segmentation using Clustering and Dimensionality Reduction

Project Overview

This project applies unsupervised learning techniques to segment customers using the Mall Customers dataset. The goal is to identify meaningful customer groups based on demographic and spending behavior using clustering algorithms. Dimensionality reduction techniques are used to visualize high-dimensional data in 2D space.

Dataset

Dataset: Mall Customers Dataset
Size: 200 records

Features:

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

The dataset contains demographic and spending information and is suitable for clustering analysis.

**Objectives**
- Explore and preprocess the dataset
- Apply clustering algorithms
- Determine optimal number of clusters
- Evaluate clustering performance
- Visualize clusters using PCA and t-SNE
- Compare clustering methods
  
Data Exploration

The dataset was loaded into Google Colab and explored using:

- head() for preview
- shape for dataset size
- info() for structure
- describe() for statistics
- Missing value check (isnull().sum())

No missing values were found in the dataset.

**Data Preprocessing**

The following preprocessing steps were applied:

- Removed CustomerID (not useful for clustering)
- Converted Gender into numerical format using one-hot encoding (get_dummies)
- Applied feature scaling using StandardScaler

These steps ensured all variables were on the same scale for distance-based clustering algorithms.

**Clustering Methods**

K-Means Clustering
- Elbow Method was used to determine optimal clusters
- Optimal number of clusters selected: 5
- Model evaluated using Silhouette Score
  
**Hierarchical Clustering (Agglomerative Clustering)**
- Dendrogram was used to determine number of clusters
- Model also set to 5 clusters
- Evaluated using Silhouette Score

**Dimensionality Reduction**
Principal Component Analysis (PCA)
- Reduced dataset to 2 components
- Used for visualization of clusters
- Helped identify separation between groups


**t-distributed Stochastic Neighbor Embedding (t-SNE)**

- Used for nonlinear visualization of clusters
- Provided clearer separation of customer groups compared to PCA


**Results and Evaluation**
Silhouette Scores
- K-Means: 0.2719
- Hierarchical Clustering: 0.2870

Hierarchical Clustering performed slightly better based on silhouette score.

Both models produced meaningful segmentation with 5 customer groups, including:

- High income, high spending
- High income, low spending
- Low income, high spending
- Low income, low spending
  
**Key Insights**
- Clustering successfully identified distinct customer segments
- PCA and t-SNE helped visualize group structure in reduced dimensions
- Hierarchical clustering slightly outperformed K-Means
- Customer behavior patterns were clearly separable after preprocessing
  
**Deployment and Monitoring**

If deployed in a business setting, this model could be used for customer segmentation in marketing strategies.

Example Use Cases:
- High-value customers receive premium offers
- Low-spending customers receive discounts
  
**Monitoring Strategy:**
- Track changes in customer behavior over time
- Monitor silhouette score after retraining
- Detect data drift
- Retrain model when patterns change
  
**Conclusion**

This project demonstrates how unsupervised learning techniques can be applied to customer segmentation. Both K-Means and Hierarchical Clustering were effective, with Hierarchical clustering performing slightly better. PCA and t-SNE improved interpretability by visualizing clusters in lower dimensions.

The project highlights the importance of preprocessing, clustering evaluation, and visualization in extracting business insights from data.

**How to Run the Project**
1. Clone the Repository
git clone https://github.com/alyssaiapalucci4/lesson9-AI-mall-customer-clustering.git

2. Open in Google Colab

Upload the notebook file:Lesson_9_Assignment_AI.ipynb

3. Upload Dataset

Upload:Mall_Customers.csv

Ensure it is in the same working directory as the notebook.

4. Install Dependencies
pip install pandas numpy matplotlib scikit-learn scipy

5. Run Notebook

Run all cells sequentially to:

explore and preprocess the dataset
apply clustering models (K-Means and Hierarchical Clustering)
determine optimal number of clusters using Elbow Method and Dendrogram
evaluate models using Silhouette Score
visualize clusters using PCA and t-SNE

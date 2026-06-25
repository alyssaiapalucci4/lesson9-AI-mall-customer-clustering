## Mall Customer Segmentation using Clustering and Dimensionality Reduction
Project Overview

This project applies unsupervised machine learning techniques to segment customers from the Mall Customers dataset. The objective is to identify meaningful customer groups based on demographic and spending behavior using clustering methods. Dimensionality reduction techniques are also used to visualize high-dimensional data in lower dimensions.

This project was completed as part of a machine learning assignment focusing on clustering, evaluation techniques, and data visualization.

**Dataset**

Dataset: Mall Customers Dataset
Size: 200 records

**Features:**
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

The dataset includes both numerical and categorical variables and is well-suited for clustering analysis.

**Objectives**
- Preprocess and prepare data for clustering
- Apply multiple clustering algorithms
- Identify optimal number of clusters
- Visualize customer segments
- Reduce dimensionality for visualization
- Evaluate clustering performance
- Discuss deployment and monitoring considerations

**Methods**
Data Preprocessing
- Missing value check
- Feature selection
- One-hot encoding for categorical variables
- Feature scaling (standardization)

**Clustering Algorithms**
- K-Means Clustering
- Hierarchical Clustering

**Cluster Evaluation**
- Elbow Method
- Silhouette Score

**Dimensionality Reduction**
- Principal Component Analysis (PCA)
- t-SNE

**Technologies Used**
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy

How to Run the Project
1. Clone the Repository
git clone https://github.com/alyssaiapalucci4/lesson9-AI-mall-customer-clustering.git

2. Open in Google Colab

Upload:Lesson_9_Assignment_AI.ipynb

3. Upload Dataset

Upload: Mall_Customers.csv

Ensure it is in the same working directory as the notebook.

4. Install Dependencies
pip install pandas numpy matplotlib scikit-learn scipy

5. Run Notebook

Run all cells sequentially to:
- preprocess data
- apply clustering models
- evaluate results
- visualize clusters and embeddings

**Results & Outputs**

The analysis produces:
- Elbow Method plot
- Dendrogram visualization
- K-Means cluster visualization
- Hierarchical clustering results
- PCA and t-SNE projections
- Silhouette score comparison
- Final interpretation of customer segments

**Key Insights**
- Customers can be grouped into distinct behavioral segments based on income and spending patterns
- K-Means provides clear cluster separation for interpretation
- PCA and t-SNE help visualize structure in reduced dimensions
- Clustering results can support targeted marketing strategies
  
**Conclusion**

This project demonstrates how unsupervised learning techniques can be applied to customer segmentation problems. The combination of clustering and dimensionality reduction provides both analytical insights and visual interpretability.

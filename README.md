# Mall Customer Segmentation using Clustering and Dimensionality Reduction

## Project Overview
This project applies unsupervised machine learning techniques to analyze customer behavior using the Mall Customers dataset. The goal is to identify customer segments based on demographic and spending data. Clustering techniques are used to group similar customers, while dimensionality reduction is used to visualize patterns in lower dimensions.

This project was completed as part of a machine learning assignment focusing on clustering, dimensionality reduction, model evaluation, and deployment strategies.

---

## Dataset
Dataset used: Mall Customers Dataset

Features:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

The dataset contains 200 customer records and is suitable for clustering analysis because it includes both categorical and numerical variables.

---

## Objectives
The objectives of this project are:

- Preprocess the dataset for clustering
- Apply multiple clustering algorithms
- Determine the optimal number of clusters
- Visualize customer segments
- Apply dimensionality reduction techniques
- Evaluate clustering performance
- Discuss deployment and monitoring strategies

---

## Methods Used

### Data Preprocessing
- Missing value check
- Removal of unnecessary columns
- One-hot encoding for categorical variables
- Standardization of features

### Clustering Techniques
- K-Means Clustering
- Hierarchical Clustering

### Cluster Evaluation
- Elbow Method
- Silhouette Score

### Dimensionality Reduction
- Principal Component Analysis (PCA)
- t-SNE

---

## Technologies Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy

## How to Run the Project

Follow these steps to run the project in Google Colab:

### Step 1: Clone the Repository
Open your terminal or Git Bash and run:

```bash
git clone https://github.com/alyssaiapalucci4/lesson9-AI-mall-customer-clustering.git
```

This will download all project files to your computer.

---

### Step 2: Open Google Colab
Go to Google Colab and upload the notebook file:

`Mall_Customer_Clustering.ipynb`

---

### Step 3: Upload the Dataset
Upload the dataset file into your Colab environment:

`Mall_Customers.csv`

Make sure the dataset is in the same working directory as the notebook.

---

### Step 4: Install Required Libraries
If any libraries are missing, install them using:

```bash
pip install pandas numpy matplotlib scikit-learn scipy
```

---

### Step 5: Run the Notebook
Run all cells from top to bottom to:

- preprocess the dataset
- perform clustering analysis
- determine the optimal number of clusters
- visualize customer segments
- apply dimensionality reduction (PCA and t-SNE)
- evaluate model performance

---

### Expected Output
After running the notebook, you will generate:

- Dataset summary and preprocessing results
- Elbow Method graph
- Dendrogram visualization
- K-Means clustering visualization
- Hierarchical clustering visualization
- PCA cluster plots
- t-SNE visualization
- Silhouette score comparisons
- Final model interpretation
- Deployment and monitoring discussion

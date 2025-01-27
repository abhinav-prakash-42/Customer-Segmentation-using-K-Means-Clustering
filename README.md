# K-Means Clustering Project

## Overview
This project demonstrates the application of the K-Means clustering algorithm to segment customers based on their **Annual Income** and **Spending Score** using Python. It includes steps for data preprocessing, determining the optimal number of clusters, training the model, and visualizing the results.

---

## Prerequisites
To run this project, ensure you have the following dependencies installed:

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

You can install them using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## Dataset
The dataset used is **Mall_Customers.csv**, which contains the following columns:
- `CustomerID`: Unique ID assigned to each customer.
- `Genre`: Gender of the customer.
- `Age`: Age of the customer.
- `Annual Income (k$)`: Annual income in thousands of dollars.
- `Spending Score (1-100)`: Score assigned based on customer spending habits.

Ensure the dataset is in the `/content/` directory when running the code in Google Colab.

---

## Steps in the Workflow

### 1. Import Dependencies
Libraries required for data handling, visualization, and clustering are imported.

### 2. Load and Inspect the Dataset
- Load the dataset using Pandas.
- Display basic information, including shape, data types, and missing values.

### 3. Select Features for Clustering
The features `Annual Income (k$)` and `Spending Score (1-100)` are selected for clustering.

### 4. Determine the Optimal Number of Clusters
- The **Elbow Method** is used to compute the Within-Cluster Sum of Squares (WCSS) for different cluster counts.
- An elbow graph is plotted to identify the optimal number of clusters.

### 5. Train the K-Means Model
- Train the K-Means clustering model with the optimal number of clusters.
- Assign a cluster label to each data point.

### 6. Visualize Clusters
- Visualize customer segments with scatter plots.
- Plot centroids for each cluster to distinguish groups.

---

## How to Run the Code

### 1. Google Colab Instructions
- Open a new notebook in [Google Colab](https://colab.research.google.com/).
- Upload the `Mall_Customers.csv` file to the Colab environment.
- Copy and paste the provided code into separate cells.
- Run each cell sequentially.

### 2. Local Execution
- Clone this repository or download the code.
- Place the `Mall_Customers.csv` file in the same directory as the script.
- Run the script using any Python IDE or terminal.

---

## Outputs
1. **Elbow Graph**:
   - Helps determine the optimal number of clusters.
2. **Cluster Visualization**:
   - Segmented groups based on customer spending behavior.
   - Centroids of clusters marked for reference.

---

## Customization
- Modify the file path for `Mall_Customers.csv` if needed.
- Adjust the number of clusters (`optimal_clusters`) based on the elbow graph.
- Use additional features (e.g., `Age`) for clustering if desired.

---

## Acknowledgments
This project uses the publicly available **Mall Customers** dataset. The implementation showcases the basic principles of unsupervised machine learning and clustering.

For questions or suggestions, feel free to reach out!


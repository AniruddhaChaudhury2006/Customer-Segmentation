# Customer Segmentation using K-Means Clustering

## Project Description

This project demonstrates customer segmentation using the K-Means clustering algorithm. The goal is to group customers based on their Annual Income and Spending Score to identify distinct customer segments, which can be valuable for targeted marketing strategies.

## Dataset

The project uses the `Mall_Customers.csv` dataset, which contains information about mall customers including their Customer ID, Gender, Age, Annual Income (k$), and Spending Score (1-100).

## Technologies Used

-   **Python**
-   **Pandas**: For data loading and manipulation.
-   **Numpy**: For numerical operations.
-   **Scikit-learn**: For implementing the K-Means clustering algorithm.
-   **Matplotlib**: For data visualization.
-   **Seaborn**: For enhancing data visualizations.

## Methodology

The following steps were performed:

1.  **Data Loading and Initial Exploration**: Loaded the `Mall_Customers.csv` dataset into a Pandas DataFrame. Performed initial data checks including `head()`, `shape`, `info()`, and `isnull().sum()` to understand the data structure and check for missing values.
2.  **Feature Selection**: Selected 'Annual Income (k$)' and 'Spending Score (1-100)' as features for clustering (`X`).
3.  **Determining Optimal Number of Clusters (Elbow Method)**: Applied the Elbow Method to find the optimal number of clusters (`k`) for K-Means. This involved calculating the Within-Cluster Sum of Squares (WCSS) for a range of cluster numbers (1 to 10) and plotting it to identify the "elbow point". The optimal number of clusters was determined to be 5.
4.  **K-Means Clustering**: Initialized and fitted the K-Means model with 5 clusters (`n_clusters = 5`). The `fit_predict()` method was used to assign each data point to a cluster.
5.  **Visualization of Clusters**: Plotted the clustered data points using a scatter plot, with each cluster represented by a different color. The cluster centroids were also plotted to visualize the center of each group.

## How to Run

1.  **Environment**: Ensure you have Python and the necessary libraries (pandas, numpy, scikit-learn, matplotlib, seaborn) installed. This notebook is designed to run in a Google Colab environment.
2.  **Data**: Make sure the `Mall_Customers.csv` file is accessible (e.g., uploaded to your Colab session or mounted from Google Drive).
3.  **Execute Cells**: Run the cells sequentially in the provided Jupyter/Colab notebook.

## Results

The output includes:

-   Initial data insights.
-   An Elbow Method plot showing the WCSS values.
-   A scatter plot visualizing the 5 distinct customer groups based on their annual income and spending score, along with their respective centroids.

These clusters can be interpreted to understand different customer behaviors and enable businesses to tailor their marketing strategies more effectively for each segment.

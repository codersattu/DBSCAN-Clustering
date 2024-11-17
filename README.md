# DBSCAN Clustering Analysis on NHANES Dataset

This project explores clustering techniques to segment patients based on the National Health and Nutrition Examination Survey (NHANES) data. The analysis involves comprehensive data preprocessing, feature transformation, and the application of clustering algorithms such as KMeans and DBSCAN.

## Project Overview

This repository contains the code and documentation for a mini-project that clusters patients using demographic, dietary, and laboratory data. The goal is to identify meaningful patient clusters and evaluate the performance of different clustering methods using silhouette scores and PCA.

## Project Structure

1. **Import Libraries**: Load necessary Python libraries for data manipulation, visualization, and clustering.
2. **Load Data**: Read the NHANES dataset into a pandas DataFrame.
3. **Data Dictionary**: Include a data dictionary for understanding the dataset's structure.
4. **Initial Data Exploration**: Examine the DataFrame's shape and identify missing values.
5. **Data Cleaning**:
   - Fill missing values in dietary, demographic, and laboratory columns with zeros.
6. **Feature Selection**: Choose relevant numerical features for clustering and remove non-essential columns.
7. **Data Transformation**: Normalize numerical features using MinMaxScaler.
8. **Optimal Cluster Identification**:
   - Use the elbow method and silhouette scores to determine the ideal number of clusters for KMeans.
9. **KMeans Clustering**:
   - Implement KMeans clustering with the optimal number of clusters and analyze results.
10. **Correlation Analysis**:
    - Study the correlation between features and cluster labels to identify highly correlated features.
11. **Principal Component Analysis (PCA)**:
    - Reduce dimensionality while retaining 95% of variance.
12. **KMeans with PCA**:
    - Apply KMeans clustering on principal components and visualize the clusters using scatter plots.
13. **DBSCAN Clustering**:
    - Perform DBSCAN clustering on principal components and evaluate outcomes.
14. **Conclusion**:
    - Summarize the findings and discuss insights gained from the clustering analysis.

## Project Highlights

- **Data Preprocessing**: Extensive handling of missing values to ensure a clean dataset.
- **Feature Scaling**: Use of MinMaxScaler for optimal scaling of numerical features.
- **Dimensionality Reduction**: Application of PCA to simplify the feature space and improve clustering.
- **Clustering Techniques**:
  - Implementation of KMeans and DBSCAN clustering algorithms.
  - Visualization of clusters and evaluation using silhouette scores.
- **Visualizations**: Scatter plots and visual aids to illustrate clustering results.

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ml3-mini-project.git
   cd ml3-mini-project
   ```
2. Ensure you have Python installed along with the required libraries listed in `requirements.txt`.
3. Run the Jupyter Notebook (`codersattu_DBSCAN_Clustering.ipynb`) to follow the analysis and reproduce the results.

## Requirements

- Python 3.x
- Libraries:
  - Pandas
  - NumPy
  - Matplotlib
  - Scikit-learn

## Results

The project identified optimal clusters through a combination of statistical techniques and PCA, visualized via scatter plots. The DBSCAN algorithm was also tested, providing additional insights into the data's structure.

## Conclusion

This project demonstrated effective clustering of NHANES data using both KMeans and DBSCAN methods, enhanced by PCA for dimensionality reduction. The approach highlighted how preprocessing and feature scaling significantly impact clustering outcomes.

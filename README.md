Customer Segmentation Script
Project Overview
This Python script performs customer segmentation on the "Mall Customer" dataset using unsupervised machine learning clustering algorithms. The goal is to identify distinct groups of customers based on their annual income and spending score, which can be valuable for targeted marketing and business strategy.

Features
The script is designed to be modular and easy to understand, with the following key functionalities:

Data Loading & Cleaning: Loads a CSV dataset, renames columns for clarity, and checks for missing values.

Exploratory Data Analysis (EDA): Visualizes key data distributions and relationships using histograms and scatter plots.

Feature Scaling: Standardizes the numerical features (AnnualIncome_k$ and SpendingScore_1-100) to prepare the data for clustering.

K-Means Clustering:

Determines the optimal number of clusters (k) using the Elbow Method and Silhouette Score.

Fits the K-Means model to the data and assigns a cluster label to each customer.

Visualization: Creates a 2D scatter plot to visualize the identified K-Means clusters and their centroids.

Bonus Tasks:

Applies a different clustering algorithm, DBSCAN, for comparison.

Calculates and displays the average spending score for each K-Means cluster.

Requirements
To run this script, you need to have Python and the following libraries installed. You can install them using pip:

pip install pandas matplotlib seaborn scikit-learn

How to Use
Download the Dataset: Ensure you have the Mall_Customers.csv file.

Place the File: Place the CSV file in the same directory as your Python script, or update the file_path variable in the script's if __name__ == "__main__": block to point to the correct location.

Run the Script: Execute the script from your terminal or a Python environment.

python your_script_name.py

The script will automatically perform each step, printing progress to the console and displaying several plots.

Code Structure
The script is organized into logical functions to promote readability and reusability:

load_and_clean_data(file_path): Handles data import and initial processing.

perform_eda(df): Generates exploratory data visualizations.

scale_features(df, feature_cols): Standardizes the input features.

determine_optimal_k(X_scaled): Plots the Elbow Method and Silhouette Score to find the best k.

perform_kmeans_and_visualize(df, X_scaled, optimal_k, scaler): Runs K-Means and visualizes the results.

perform_bonus_tasks(df, X_scaled): Executes the additional tasks for DBSCAN and cluster analysis.

if __name__ == "__main__":: The main execution block that orchestrates the entire workflow.

Data Source
The dataset used in this project is the "Mall Customer Segmentation Data" from Kaggle.

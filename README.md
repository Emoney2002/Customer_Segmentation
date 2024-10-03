# Customer_Segmentation
Customer Segmentation using K-Means Clustering
This project applies K-Means Clustering to the "Mall Customers" dataset to segment customers based on their annual income and spending score. The aim is to group customers with similar behavior for potential targeted marketing strategies. We perform Exploratory Data Analysis (EDA) and use machine learning techniques to achieve meaningful customer segmentation.

Project Overview

The goal of this project is to perform customer segmentation using K-Means clustering based on the customers' annual income and spending score. By analyzing the clusters, businesses can design tailored marketing strategies for each customer segment.

Dataset

The dataset used is Mall_Customers.csv, which contains the following columns:

CustomerID: Unique identifier for each customer.

Gender: Gender of the customer.

Age: Age of the customer.

Annual Income (k$): Annual income of the customer in thousand dollars.

Spending Score (1-100): Score assigned based on the customer’s behavior and spending habits.

Exploratory Data Analysis (EDA)

Missing Values Check: No missing values were found in the dataset.

Descriptive Statistics: Summary statistics such as mean, median, and standard deviation for the numeric features (age, income, spending score).

Visualizations:

Gender Distribution: The dataset has more female than male customers.

Age Distribution: Most customers are between 25 and 50 years old.

Income and Spending Score Distribution: A diverse range of customer incomes and spending scores is observed.

Correlation Heatmap: Showed no significant correlation between income and spending score.

Key Insights from EDA

Customers are mostly in the age group of 25-50.

Income and spending score are not strongly correlated, allowing for meaningful segmentation.

Machine Learning Model

We applied K-Means Clustering to segment customers based on their Annual Income and Spending Score.

Steps:
Feature Selection: Used Annual Income (k$) and Spending Score (1-100) for clustering.

Elbow Method: The Elbow Method was applied to determine the optimal number of clusters. The optimal number of clusters was found to be 5.

Model Training: K-Means clustering was performed with 5 clusters.

Data Scaling: The features were scaled using StandardScaler to ensure clustering effectiveness, as K-Means is sensitive to feature scales.

Cluster Visualization: The results were visualized, showing distinct customer segments.

Results

The K-Means model segmented customers into 5 distinct clusters based on their income and spending score. These clusters 
could be useful for designing personalized marketing strategies:

Cluster 1: High income, high spending.
Cluster 2: Low income, low spending.
Cluster 3: High income, low spending.
Cluster 4: Low income, high spending.
Cluster 5: Medium income, medium spending.

Visualization

The clusters were plotted to visualize how customers are grouped based on their income and spending score. The centroid of each cluster was marked, showing the center of each group.

Requirements
To run this project, you'll need:

Python 3.x
pandas
numpy
scikit-learn
matplotlib
seaborn

You can install the necessary packages by running:


pip3 install -r requirements.txt

Future Improvements

Try Different Clustering Algorithms: Methods like DBSCAN or Agglomerative Clustering could provide different insights.

Incorporate More Features: Add more features such as age, gender, or transaction history for a more comprehensive segmentation.

Dimensionality Reduction: Techniques like PCA (Principal Component Analysis) could be used to reduce dimensionality before clustering.

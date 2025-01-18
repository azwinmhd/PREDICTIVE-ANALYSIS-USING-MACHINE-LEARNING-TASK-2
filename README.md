# PREDICTIVE-ANALYSIS-USING-MACHINE-LEARNING-TASK-2
NAME: AZWIN MUHAMMED KK
COMPANY: CODTECH IT SOLUTIONS
ID: CT08EQY 
DOMAIN: DATA ANALYTICS 
DURATION: December 20th, 2024 to January 20th, 2025
MENTOR: SRAVANI GOUNI

Description of Task:
In this task, we aim to perform customer segmentation using the KMeans clustering algorithm on a dataset containing information about mall customers. The dataset, "Mall_Customers.csv," includes various attributes such as age, annual income, and spending score. The primary goal is to identify distinct groups of customers based on their spending behavior and income levels, which can provide valuable insights for targeted marketing strategies and personalized services.
The first step involves loading the dataset using the Pandas library. We handle potential file-related errors gracefully, ensuring that the user is informed if the dataset is not found. Once the data is loaded, we conduct a preliminary exploration to understand its structure and contents. This includes checking the data types, viewing the first few rows, and obtaining summary statistics. Such exploratory data analysis (EDA) is crucial as it helps identify the nature of the data, the presence of any missing values, and the distribution of key features.
Before applying the KMeans algorithm, we check for missing values in the dataset. Although the dataset is expected to be clean, it is essential to handle any missing data appropriately, either through imputation or by removing affected rows or columns. In this case, we focus on the features relevant for clustering: 'Annual Income (k$)' and 'Spending Score (1-100)'.
To ensure that the KMeans algorithm performs optimally, we standardize these features using the StandardScaler. Feature scaling is critical in clustering tasks, as KMeans relies on distance calculations, and unscaled features can lead to biased results. Standardization transforms the data to have a mean of zero and a standard deviation of one, allowing for a more accurate clustering process.
One of the key challenges in KMeans clustering is selecting the appropriate number of clusters (k). To address this, we employ the Elbow Method, which involves fitting the KMeans algorithm for a range of cluster values (from 1 to 10) and calculating the Within-Cluster Sum of Squares (WCSS) for each. By plotting WCSS against the number of clusters, we can visually identify the "elbow point," where adding more clusters yields diminishing returns in terms of variance explained. This point suggests an optimal number of clusters for our analysis.
After determining the optimal number of clusters, we apply the KMeans algorithm to the scaled data. The algorithm assigns each customer to one of the identified clusters based on their income and spending score. We then append the cluster assignments back to the original DataFrame, allowing for further analysis and visualization.
To better understand the clustering results, we visualize the clusters using a scatter plot. The plot displays customers' annual income against their spending score, with different colors representing different clusters. Additionally, we highlight the centroids of each cluster, which represent the average position of customers within that cluster. This visualization aids in interpreting the clustering results and provides insights into customer segments that may require different marketing strategies.
Finally, we conduct a cluster analysis by calculating the mean values of various features for each cluster. This analysis helps in understanding the characteristics of each customer segment, such as average age, income, and spending behavior. Furthermore, we can visualize the distribution of other features, such as age, across clusters using box plots, providing a comprehensive view of how different customer segments vary.

In summary, this task demonstrates the application of KMeans clustering to segment mall customers based on their income and spending behavior. By leveraging data exploration, preprocessing, and visualization techniques, we gain valuable insights into customer segments, which can inform marketing strategies and enhance customer engagement.

Output:

![Image](https://github.com/user-attachments/assets/60f212ae-78cf-4771-a1eb-7147cfeccc6d)

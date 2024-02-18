# Market-Segmentation-of-Credit-Card-Customers

**Submitted by: Lekhansh**

### Objective
The objective of this project is to perform market segmentation based on clustering analysis of credit card customers. The aim is to understand customer characteristics and behavior through customer segmentation, which can then be used for targeted marketing strategies.

### Methodology
The methodology involves several steps:

1. **Data Understanding and Exploratory Data Analysis (EDA):** Initial exploration and analysis of the dataset to understand its structure and characteristics.
2. **Data Pre-processing:** Cleaning and preparing the dataset for modeling, including handling missing values and outliers.
3. **Data Modeling:** Applying non-supervised clustering techniques including K-Means, HDBSCAN, and Hierarchical Clustering.
4. **Results and Comparisons:** Evaluating the performance of each clustering technique and comparing the obtained clusters.

### Data Understanding
The dataset contains information on the usage behavior of approximately 9000 active credit card holders over the last 6 months. Initial analysis revealed missing values in the 'credit_limit' and 'minimum_payments' columns.

### Univariate Analysis Results
Univariate analysis provided insights into various features such as balance, purchases, credit limit distribution, and payment behavior among customers.

### Bivariate Analysis Results
Bivariate analysis revealed correlations between different features, indicating relationships such as purchase behavior and payment frequency.

### Data Pre-Processing
Data pre-processing involved removing unnecessary columns, handling missing values (imputation with median), and addressing outliers through square root transformation.

### Principal Component Analysis (PCA)
PCA was applied to reduce the dimensionality of the dataset for better visualization of clusters. Approximately 70% of information was retained by extracting 2 principal components.

### Data Modeling
Three clustering techniques were utilized:

1. **K-Means:** Optimal number of clusters (K=5) was determined using inertia plot and silhouette visualizer.
2. **Hierarchical Clustering:** Hierarchical clustering was performed using Ward and Complete linkage methods. Complete linkage method with K=4 was preferred based on Davies Bouldin Score.
3. **HDBSCAN:** Hyperparameters were selected based on silhouette score, resulting in 3 clusters.

### Results and Comparisons
Silhouette scores were calculated for each clustering technique to evaluate performance. The hierarchical model using complete linkage achieved the highest silhouette score of 0.55, indicating its effectiveness in segmenting credit card customers.

## Conclusion
Market segmentation based on clustering analysis offers valuable insights into customer behavior, allowing businesses to tailor their marketing strategies effectively. The hierarchical clustering technique using complete linkage emerged as the best approach for segmenting credit card customers in this analysis.


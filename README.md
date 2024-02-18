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

![Screenshot (257)](https://github.com/Lekhansh-cmd/Market-Segmentation-of-Credit-Card-Customers/assets/78807364/7bf4ac04-d708-4c74-85ce-f4e039001c9f)

1. Features like ‘balance’, ‘purchases’, ‘oneoff_purchases’, ‘installment_purchases’, and ‘cash_advance’ show
similar trends.
2. For around 6000 customers, the balance frequency is frequently updated.
3. The purchases are being made frequently by around 2000 customers. Also, the purchase frequency can be
categorized into 2 categories - those who frequently purchase and those who rarely purchases.
4. more customers made purchases using installments rather than one-go purchases.
5. The majority of credit limit for a user falls between 0 and 15000.
6. Around 5% of users have made full payment while around 6000 customers still haven't made any payment/installment.
7. Around 80% of customers have credit card tenure service in the 12th month.
8. The balances of 95% of users are between 0 and 5000.

### Bivariate Analysis Results
Bivariate analysis revealed correlations between different features, indicating relationships such as purchase behavior and payment frequency.

![Screenshot (258)](https://github.com/Lekhansh-cmd/Market-Segmentation-of-Credit-Card-Customers/assets/78807364/c0f2fc00-0877-41a4-a613-66958114933a)

We can see an almost perfect positive correlation between the following features:
* Purchases and One-off purchases
* Cash Advance Frequency and Cash advance transactions
* Purchase frequency and purchase installment frequency
Medium Correlation between:
* Purchases and Installments purchases
* Purchases and Purchase Transactions
* Purchases and Payments
* Cash Advance and Cash Advance Transactions / Cash Advance Frequency.

### Data Pre-Processing
Data pre-processing involved removing unnecessary columns, handling missing values (imputation with median), and addressing outliers through square root transformation.

1. Removal of unnecessary columns.
2. Checking for duplicates and removal (if any).
3. Handling missing values.
4. Checking for outliers and handling.

### Principal Component Analysis (PCA)
PCA was applied to reduce the dimensionality of the dataset for better visualization of clusters. Approximately 70% of information was retained by extracting 2 principal components.

![Screenshot (259)](https://github.com/Lekhansh-cmd/Market-Segmentation-of-Credit-Card-Customers/assets/78807364/fa226169-07e1-4b06-87b9-7016ae5c6e61)

### Data Modeling
Three clustering techniques were utilized:

1. **K-Means:** Optimal number of clusters (K=5) was determined using an inertia plot and silhouette visualizer.
2. **Hierarchical Clustering:** Hierarchical clustering was performed using Ward and Complete linkage methods. A complete linkage method with K=4 was preferred based on the Davies Bouldin Score.
3. **HDBSCAN:** Hyperparameters were selected based on silhouette score, resulting in 3 clusters.

### Results and Comparisons
Silhouette scores were calculated for each clustering technique to evaluate performance. The hierarchical model using complete linkage achieved the highest silhouette score of 0.55, indicating its effectiveness in segmenting credit card customers.

## Conclusion
Market segmentation based on clustering analysis offers valuable insights into customer behavior, allowing businesses to tailor their marketing strategies effectively. The hierarchical clustering technique using complete linkage emerged as the best approach for segmenting credit card customers in this analysis.


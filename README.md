# Customer-Segmentation-Using-RFM-Analysis-and-Clustering





## Project Overview

This project implements RFM (Recency, Frequency, Monetary) analysis to segment customers for a UK-based online retail company. By applying clustering techniques, the goal is to identify distinct customer segments, leading to more targeted marketing strategies and improved sales performance.

## Data Source

The dataset used is from [UCI's Online Retail Data](https://archive.ics.uci.edu/dataset/352/online+retail).

## Key Steps

1. **Data Loading and Cleaning**
   - Loaded data from an Excel file.
   - Handled missing values and removed duplicates.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed sales trends, top products, and customer distributions.
   - Visualized sales patterns by hour, month, and country.

3. **Feature Engineering**
   - Created new features: `Day`, `Month`, `Year`, `Hour`, `Minute`, `Second`, and `TotalAmount`.

4. **RFM Analysis**
   - **Recency**: Days since last purchase.
   - **Frequency**: Number of purchases.
   - **Monetary**: Total spending.

5. **Outlier Detection**
   - Identified and removed outliers in `Recency`, `Frequency`, and `Monetary` attributes.

6. **Clustering**
   -tried out different clustering algorithms such as K-Means, Agglomerative Hierarchical Clustering, and DBSCAN
   -Additionall yanalyzed the cluster segmentation by plotting Recency vs. Frequency for each cluster.
   

## Results

- **K-Means Clustering**: Selected for its optimal silhouette score, producing well-defined customer segments.
- **Customer Segments**:
  - **Whales**: Valuable and highly engaged customers.
  - **Average Customers**: Regular but not exceptional.
  - **At-Risk Customers**: Less engaged and at risk of churning.

## Conclusion

- The RFM analysis and clustering have provided insights into customer behavior, enabling more targeted marketing and strategic decision-making.
- We analyzed cluster distribution and visualized it with a pie chart to understand the proportion of each customer segment.
- Observation
- RFM analysis shows that:

- Avg Customers: 52.89%
- At-Risk Customers: 25.66%
- High-Value Frequent Buyers (Whales): 21.44%
- This highlights that most customers are average, some are at risk, and a smaller group is highly valuable.

### Explanation of RFM Analysis

- **Recency**: Measures how recently a customer has made a purchase. More recent customers are typically more engaged.
- **Frequency**: Counts the number of purchases a customer has made. More frequent buyers are often more loyal.
- **Monetary**: Calculates the total amount spent by the customer. Higher spending indicates greater value.

### Customer Segmentation

1. **High-Value Frequent Buyers (Whales)**: Customers who spend a lot, buy frequently, and have recent interactions.
2. **Average Customers**: Customers with moderate spending, frequency, and recency.
3. **At-Risk Customers**: Customers who spend less, buy infrequently, and have not interacted recently.


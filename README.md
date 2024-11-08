# Customer_Segmentation-Analysis

This project applies the K-Means clustering algorithm for customer segmentation, a common marketing strategy used to divide a company's customers into groups based on their characteristics. Customer segmentation helps businesses understand their customers' needs and behaviors, allowing for more targeted marketing strategies and enhanced customer experiences.

## Project Overview
The dataset used in this project includes the following customer attributes:

  - Customer ID: Unique identifier for each customer

  - Gender: Gender of the customer

  - Age: Age of the customer

  - Annual Income (k$): Annual income of the customer in thousands of dollars

  - Spending Score (1-100): Score assigned by the mall based on customer spending patterns and behavior


## How Customer Segmentation Works
Customer segmentation through K-Means clustering aims to group customers with similar attributes.
By analyzing patterns in Age, Annual Income, and Spending Score, K-Means creates clusters where each group represents a distinct customer type. For instance:

  - High-income customers with high spending scores could be targeted for premium offers.


  - Young customers with moderate incomes might be engaged with affordable or trend-based products.
    

Through segmentation, companies can make data-driven marketing decisions to improve customer satisfaction and retention.

## Data Analysis Steps


### 1. Data Preprocessing

  - Standardization: The Age, Annual Income (k$), and Spending Score features were standardized to bring all values to a similar scale, as clustering algorithms are sensitive to the scale of features.
  - Choosing Optimal Clusters: The optimal number of clusters was identified using the Elbow Method. This method involves plotting the sum of squared distances (inertia) for a range of cluster values. The point where inertia begins to decrease more slowly suggests an optimal number of clusters—in this case, k=5.
2. Exploratory Data Analysis (EDA)
EDA was performed to understand the dataset's structure and relationships between features, providing insights into the distribution of each feature and the interaction between features:

Distribution Analysis: The distributions of Age, Annual Income, and Spending Score were visualized using histograms to understand how these values are spread across customers.

Age: Revealed a broad range of customers, with a concentration around young adults.
Annual Income: Displayed a normal distribution with some variation, indicating a balanced customer base in terms of income.
Spending Score: A range from low to high, which can indicate diverse spending behaviors.
Pair Plot: A pair plot was used to observe relationships among Age, Income, and Spending Score. By coloring each point by its cluster, we could see how different clusters occupied distinct regions in the feature space.

Cluster Visualization: A scatter plot of Annual Income vs. Spending Score visualized the five clusters in two dimensions, with centroids marked to show the center of each cluster. This helps identify characteristics of each segment (e.g., high-income, low-spending vs. low-income, high-spending groups).

Conclusion and Insights
The K-Means clustering model identified five distinct customer segments based on Age, Annual Income, and Spending Score. The segmentation reveals that customer behavior varies significantly:

High-Income, High-Spending: Likely loyal and profitable customers, suited for premium services.
Low-Income, High-Spending: Engaged customers but potentially price-sensitive; promotions might drive value.
High-Income, Low-Spending: Potential to engage further, possibly through targeted loyalty programs.
Younger, Moderate Income: Can be nurtured for brand loyalty with products suited to young lifestyles.
Future Work and Enhancements
For further analysis and improved segmentation, the following steps can be considered:

Additional Features: Including more behavioral data, such as purchase frequency, preferred categories, or visit times, could enhance segmentation.
Alternative Clustering Techniques: Testing other clustering algorithms (e.g., hierarchical clustering, DBSCAN) may provide better customer groups or insights.
Segmentation Validation: Applying customer satisfaction surveys or marketing KPIs to evaluate the effectiveness of each segment.
Personalized Marketing: Using these segments to create targeted marketing campaigns, track customer engagement metrics, and adjust strategies over time.
This customer segmentation project demonstrates how K-Means clustering can be an effective tool for identifying customer segments and informs strategies for customer relationship management.

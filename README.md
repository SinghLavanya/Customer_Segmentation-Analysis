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

  - 🛒🛒High-income customers with high spending scores could be targeted for premium offers. 
    

*Example - Airline Loyalty Programs for High-Spending Frequent Flyers.
         - Private Banking and Wealth Management for High-Net-Worth 
           Individuals*


  - 🛒🛒Young customers with moderate incomes might be engaged with affordable or trend-based products. 

*Example - Fast Fashion Brands indulging in targeted marketing and loyalty              programs, along with student discounts.
         - Affordable subscription-based entertainment services.*

Companies can make data-driven marketing decisions through segmentation to improve customer satisfaction and retention.

## Data Analysis Steps


### 1. Data Preprocessing

  - Standardization: The Age, Annual Income (k$), and Spending Score features were standardized to bring all values to a similar scale, as clustering algorithms are sensitive to the scale of features.
  - Choosing Optimal Clusters: The optimal number of clusters was identified using the Elbow Method. This method involves plotting the sum of squared distances (inertia) for a range of cluster values. The point where inertia begins to decrease more slowly suggests an optimal number of clusters—in this case, k=5.

<img width="525" alt="elbow plot" src="https://github.com/user-attachments/assets/c3b83847-a1a6-4468-95a3-d1e36ea194de">


### 2. Exploratory Data Analysis (EDA)
EDA was performed to understand the dataset's structure and relationships between features, providing insights into the distribution of each feature and the interaction between features:

  1.  Distribution Analysis: The distributions of Age, Annual Income, and Spending Score were visualized using histograms to understand how these values are spread across customers.

  - Age: Revealed a broad range of customers, concentrating on young adults.
  - Annual Income: Displayed a normal distribution with some variation, indicating a balanced customer base in terms of income.
  - Spending Score: A range from low to high, which can indicate diverse spending behaviors.


<img width="862" alt="viz_4" src="https://github.com/user-attachments/assets/ecca87e9-04bd-49d6-b65c-1e1b85e9e0fb">



   2. Pair Plot: A pair plot was used to observe relationships among Age, Income, and Spending Score. By coloring each point by its cluster, we could see how different clusters occupied distinct regions in the feature space.

<img width="604" alt="viz_3" src="https://github.com/user-attachments/assets/f117a3a1-d457-490a-98b0-1f5fa95cd300">

  3. Cluster Visualization: A scatter plot of the Annual Income vs. Spending Score visualized the five clusters in two dimensions, with centroids marked to show the center of each cluster. This helps identify the characteristics of each segment (e.g., high-income, low-spending vs. low-income, high-spending groups).

<img width="756" alt="Viz_1" src="https://github.com/user-attachments/assets/18532b94-ef87-479b-bdf1-8426062b66b1">


### Conclusion and Insights
The K-Means clustering model identified five distinct customer segments based on **Age, Annual Income, and Spending Score**. The segmentation reveals that customer behavior varies significantly:

  1. 💰💰💰💰    **High-Income, High-Spending**: Likely loyal and profitable customers, suited for premium services.
  2. 💰💰💰      **Low-Income, High-Spending**: Engaged customers but potentially price-        sensitive; promotions might drive value.
  3. 💰💰         **High-Income, Low-Spending**: Potential to engage further, possibly           through targeted loyalty programs.
  4. 💰           **Younger, Moderate Income**: Can be nurtured for brand loyalty with             products suited to young lifestyles.


### Future Work and Enhancements

For further analysis and improved segmentation, the following steps can be considered:

- **Additional Features**: Including more behavioral data, such as purchase frequency, preferred categories, or visit times, could enhance segmentation.


- **Alternative Clustering Techniques**: Testing other clustering algorithms (e.g., hierarchical clustering, DBSCAN) may provide better customer groups or insights.


- **Segmentation Validation**: Applying customer satisfaction surveys or marketing KPIs to evaluate the effectiveness of each segment.


- **Personalized Marketing**: Using these segments to create targeted marketing campaigns, track customer engagement metrics, and adjust strategies over time.


This customer segmentation project demonstrates how K-Means clustering can be an effective tool for identifying customer segments and informs strategies for customer relationship management.

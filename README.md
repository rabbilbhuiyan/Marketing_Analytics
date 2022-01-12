# Marketing Campaigns Analytics
The objective of this analytics project is to investigate wheter marketing campaigns have been as effective as were expected to be and also propose a data-driven solutions by extracting actionable insights from the given data of a company that improves their decision-making process. 

Furthermore, the project also performs Customer segmentation analysis - the practice of separating customers into groups that reflect similarities among customers in each cluster, in order to help a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors and concerns of different types of customers.

### Dataset
The dataset consist of 2240 observations (customers) with 28 variables related to marketing data. More specifically, the variables provide insights about:
- Customer profiles
- Products purchased
- Marketing Campaign success (or failure)
- Marketing Channel performance

To perform a well-structured and holistic data analysis, first we began with Data Wrangling followed by Explaratory Data Analysis, Statistical Testing and Data Vizualization.

### Exploratory Data Analysis - Business Intelligence
Data wrangling and Exploratory Data Analysis (EDA) both are perfomed at the same time in this project. The following steps have been performed during the analysis by using brain-storming and all possible exploration. We began with
- basic info (description of data)
- finding missing value and imputation
- feature engineering
- finding outliers and replacement or removal of outliers
- finding pattern in terms of correlation
- finding anaomalies
In the pattern analysis (correlation analysis) we found three major clusters namely 'High Income', 'Dependents/Minor' and 'Advertising' clusters and accordingly expolred the details of each cluster.

### Statistical Analysis - Data Driven Decision
We run statistical tests in the form of regression to answer the questions and propose a data-driven action to the Decision Maker /Chief Marketing Officer e.g by answering 
- What factors are significantly related to the number of store purchases?
- Does US fare significantly better than the rest of the world in terms of total purchases?
- Do people who spent an average amount of gold significantly do store purchases? 
- Does fish omega fatty acid signifiantly related to Higher educated people?
- Is there a significant relationship between geographical regional and success of a campaign?

### Data Visualization 
We then plotted and visualized to answers to the below questions.
- Which marketing campaign is most successful?
- What does the average customer look like for this company?
- Which products are performing best?
- Which channels are underperforming?
![heatmap_correlation_matrix](https://user-images.githubusercontent.com/36482524/148923435-5929d923-2007-495a-90a5-a8742d7aa6ac.png)
### Summary - actionable findings to improve advertising campaign success
Finding-1: The most successful advertising campaign was the most recent campaign (column name: Response), and was particularly successful in Mexico (>60% acceptance rate!)
Suggested action: Conduct future advertising campaigns using the same model recently implemented in Mexico.

Finding-2: Advertising campaign acceptance is positively correlated with income and negatively correlated with having kids/teens
Suggested action: Create two streams of targeted advertising campaigns, one aimed at high-income individuals without kids/teens and another aimed at lower-income individuals with kids/teens

Finding-3: The most successful products are wines and meats (i.e. the average customer spent the most on these items)
Suggested action: Focus advertising campaigns on boosting sales of the less popular items

Finding-4: The best performing channels are web and store purchases (i.e. the average customer made the most purchases via these channels)
Suggested action: Focus advertising campaigns on the more successful channels, to reach more customers

## Customer Segmentation Anaysis
For this analysis, I performed unsupervised clustering. I did use dimensionality reduction followed by agglomerative clustering. I came up with 4 clusters (based on elbow method with hihger silhouette score) and further used them in profiling customers in clusters according to their family structures and income/spending. This can be used in planning better marketing strategies.

![customer_cluster](https://user-images.githubusercontent.com/36482524/149098768-7e442cc7-4d2d-4950-b27d-f0b410afec63.png)

### Findings - planning marketing strategies based on the observed customer clusters
Culster -0 :
- They are definitely a parent
- At the max are 5 members in the family and at least 2
- Mjority of them have a teenager at home
- Relatively older
- A lower-income group

Cluster -1:
- Are a definetly parent
- At the max have 4 members in the fiamily and at least 2
- Single parents are a subset of this group
- Most hava a teenager at home
- Relatively older

Culster -2:
- Are a definitely not a parent
- At the max only 2 members in the family
- A slight majority of couples over single people
- Span over all ages
- A high income group

Cluster - 3:
- The mjority of these people are parents
- At the max are 3 members in the family
- They majorly have one kid
- Relatively younger


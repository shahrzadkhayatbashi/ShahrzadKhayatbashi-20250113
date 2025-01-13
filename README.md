# Customer Service Insight Analysis

## Overview
This repository contains an analysis performed as part of a case study task to uncover insights from customer service and order data for a travel agency. The goal was to identify patterns in customer service interactions and provide actionable recommendations to improve operational efficiency and customer satisfaction.

The analysis is structured into multiple Jupyter notebooks, each focusing on a specific step of the process, from data cleaning to advanced analysis. The findings are supplemented with visualizations and key insights to address the objectives outlined in the case study.

---

## Repository Structure

```
├── notebooks/
│   ├── 01_clean_orders.ipynb             # Cleaning and preprocessing the Orders dataset.
│   ├── 02_clean_errands.ipynb            # Cleaning and preprocessing the Errands dataset.
│   ├── 03_extract_xes.ipynb              # Preparing data for process mining and event analysis.
│   └── 04_analysis.ipynb                 # Exploratory data analysis, visualizations, and insights.
├── Shahrzad-20250112-Presentation.pptx   # Presentation of the result
├── requirement.txt   # Used Python Libraries. 
└── README.md                             # Project documentation.
```


---

## Analysis Workflow
1. **Data Cleaning:**
   - Checking data inconsistencies.
   - Cleaning data especially unifying revenueues into the same currency.
   
2. **Feature Engineering:**
   - Extracted and transformed key features, including time intervals and categorical groupings.
   
3. **Exploratory Data Analysis:**
   - Generated descriptive statistics and visualizations to identify trends and patterns.
   
4. **Insight Generation:**
   - Focused on significant relationships identified by investigating correlations among different features. 
   - Performed K-means clustering and process mining algorithms.

---

## Visualizations
- Plotting top ten countries where orders are made [see block 19th](/01.%20clean%20orders.ipynb)
- Distributions of orders per week. [see block 20th](/01.%20clean%20orders.ipynb)
- Top 10 Countries by Revenue with Scaled Order Amount Comparison [see block 40th](/01.%20clean%20orders.ipynb)
- Top 10 Partners by Revenue with Order Amount Comparison [see block 41th](/01.%20clean%20orders.ipynb)
- Top 10 Brands by Revenue with Order Amount Comparison [see block 42nd](/01.%20clean%20orders.ipynb)
- Heatmap of Brand to Partner Relationships with their percentages [see block 43rd](/01.%20clean%20orders.ipynb)
- Distribution of orders for different group types [see block 44th](/01.%20clean%20orders.ipynb)
- Count of Cancellation per Reason [see block 64th](/01.%20clean%20orders.ipynb)
- Count of change reason for each Reason [see block 65th](/01.%20clean%20orders.ipynb)
- Distribution of errand per channel [see block 27th](/02.%20clean%20errands.ipynb)
- Count of each errand categor  [see block 29th](/02.%20clean%20errands.ipynb)
- Distribution of Customer Contacts Per Order [see block 9th](/04.%20analysis.ipynb)
- Distribution of Customer Contacts Per Order [see block 10th](/04.%20analysis.ipynb)
- Number of contacts for Each Errand Type [see block 10th](/04.%20analysis.ipynb)
- Percentage Distribution of Channels by Errand Type [see block 10th](/04.%20analysis.ipynb)
- Elbow Method (Sampled Data) [see block 34th](/04.%20analysis.ipynb)
- Clusters Visualization (PCA) [see block 38th](/04.%20analysis.ipynb)
- Feature Contributions to Principal Components [see block 40th](/04.%20analysis.ipynb)
- Different Scatter Plots elaborating on findings [see blocks after 40th](/04.%20analysis.ipynb)
---

## Actionable Recommendations
- We may be able to optimize process for Partner A as they cause the same number of contact but with much less revenue comparing Partner C. 
- We may be able to further investigate how multiple systems used in making an order may affect the number of contacts. The data was not enough to identify actionable insight, so further investigation can be done with the help of more data. 
-  We can further analyze customer conversation using NLP techniques to identify most common topics that customers asked in most problemestic category. If those information convey to customer in a good time, we may be able to reduce the contacts significantly.
-  With using NLP techniques for 19: Chat and 2: Mail, we can investigate the most repetitive patterns throught the chats and based on that implement chatbot, which customers can get their answer by bot. 

---

## How to Run
Please install a virtual environment based on the requriement file provided in the repository. 

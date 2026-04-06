
<img width="746" height="152" alt="image" src="https://github.com/user-attachments/assets/6e6733e7-7ce5-4680-976d-06b25201a143" />


Product Number:	W33836
Title:	Nata Supermarkets: Customer Analytics - Student Spreadsheet
 	
This spreadsheet supports the product "Nata Supermarkets: Customer Analytics" (W33834)
Prepared by:	Bissan Ghaddar
Last Revised:	September 12, 2023
No part of this file may be reproduced, stored in a retrieval system, posted to the Internet, or transmitted in any form or by any means without the permission of Ivey Business School Foundation.  To order copies or request permission to reproduce materials, contact Ivey Publishing, Ivey Business School, Western University, London, Ontario, Canada, N6G 0N1; (t) 519.661.3208; (e) cases@ivey.ca; www.iveypublishing.ca. Our goal is to publish materials of the highest quality; submit any errata to publishcases@ivey.ca.
 	
© 2023 Ivey Business School Foundation



## PROJECT INTERPRETATION

For my Master's in International Management and Supply Chain studies, I participated in the course Business Analytics. As final project for this course, we were asked to read, understand, clean and cluster the dataset given in order to comprehend and furthermore perform a product forecast. 

The steps followed were the next:
1. Data cleaning: 24 missing values in “Income”. 3 unknown columns. No duplicated data. Encoding "Education". Encoding "Marital_Status". Weird values Absurd & YOLO
2. Clustering: Segment customers based on all the features. Identify patterns for marketing strategy and customer insights.
Removed ID to avoid distortion. Ran K-Means with K = 2 to 10. Evaluated each model using Silhouette Score.
4. K-Means clustering: K = 3  Provides a clear and balanced segmentation.
Clusters:
0) 36% 801 customers: mid-income customers (40,000–60,000) with moderate spending on wine, fruits, meat, fish, sweets, and gold over the past two years, with gold spending close to Cluster 2. Many have one teenager at home.
1) 33% 737 custoemrs:  low-income customers (0–40,000) who show the lowest spending across all categories. Many have one young child. They make fewer online purchases, but recorded the highest number of website visits last month.
2) 31% 694 custoemrs: high-income customers (65,000–160,000) with the highest spending on wine, fruits, meat, fish, and sweets, while their gold spending is similar to Cluster 1. Most have no children.
💡 Marketing insight: Cluster 2 is the group with the strongest purchasing power, while Cluster 1, although less affluent, is highly active online, making it a good target for online promotions.
5. Hierarchical cluster tree: for visualization. Distribution was 43% / 40% / 17%. The segmentation was not balanced
6. Forecasting: To plan what will be bought from suppliers from the information given for each cluster
First we performed a weekly forecast, but the quantities required for every product were not enough to perform a purchase, and for the first weeks, the requirement was 0. So we prefered a monthly forecast.
7. Double exponential smoothing forecast: using two equations (level, trend)
8. Winter's model forecast: adding seasonal patterns
9. Past years forecast: to decide if the calculations were accurate. While DES might have shown slightly better overall average MAPE and RMSE in this particular comparison for 2013-2014, Winter's Model is more suitable for sales data due to its seasonality analysis.
10. Inventory analysis: forecast for the 5 product types. (Quantity to buy for each month, inventory level at the end of each month, binary decision of purchase).
<img width="678" height="556" alt="image" src="https://github.com/user-attachments/assets/f1a04a5c-46b2-492b-81b0-f6a4fdfe08b3" />


Conclusion
The optimization results show that ending inventory is zero every month across all five product categories Fish Fruits, Meat, Gold, and Wine. Demand is met precisely each month without leftover stock. Replenishment timing can be highly accurate.
Managerial Recommendation: Adopt Just-In-Time (JIT) replenishment system to reduce holding costs and improve inventory efficiency.





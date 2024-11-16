<h2>Mall Customer Segmentation with K-Means Clustering</h2> </br>
This project leverages K-Means clustering to analyze and segment mall customer data based on spending behavior and income. By grouping similar customers, we can gain insights into distinct customer profiles, enabling targeted marketing and customized service strategies.

<h2>Dataset Overview</h2> </br>
The dataset (Mall_Customers.csv) provides essential information about mall customers:</br>

CustomerID: A unique identifier for each customer. </br>
Gender: Male or Female.</br>
Age: Customer’s age.</br>
Annual Income: The estimated yearly income (in thousands of dollars).</br>
Spending Score: A score given by the mall, measuring spending patterns and behavior. </br>

<h2>Project Objective </h2> <br>
The main goal of this project is to segment customers into distinct groups based on their Annual Income and Spending Score. Understanding these segments helps businesses create tailored marketing strategies, enhancing engagement and retention.

<h2>Clustering Methodology</h2> </br>
<h5> 1. Determining the Optimal Number of Clusters (Elbow Method)</h5> 
Using the Elbow Method, we examined the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters. The goal was to identify the point at which adding more clusters provided minimal benefit in reducing WCSS, known as the "elbow." </br>
Outcome: We found that 5 clusters offered an ideal segmentation, effectively balancing variance and simplicity.
</br>
<h5>2. Customer Segmentation Profiles</h5>
With the optimal cluster count selected, we identified and analyzed each customer segment in detail:
<h5>Premium Customers (High Income, High Spending)</h5>
Customers in this segment have both high income and high spending scores, making them ideal for premium offerings. These individuals are valuable for targeted, high-end marketing campaigns and exclusive offers that cater to their spending capacity and lifestyle. 
<h5>Budget-Conscious Shoppers (Low Income, Low Spending)</h5>
This group includes customers with lower income and spending scores. They are more likely to be budget-conscious and may respond well to promotions focused on value, such as discounts or loyalty incentives. These strategies encourage higher spending without overwhelming their budget.
<h5>Middle-Tier Customers (Moderate Income, Moderate Spending)</h5>
Representing a balanced segment with moderate income and spending behavior, these customers make up a significant portion of the customer base. Campaigns that offer moderate discounts, seasonal bundles, or added value without high prices resonate well with this group.
<h5>Luxury Spenders (Low Income, High Spending)</h5>
Though less common, this unique segment includes customers who tend to spend significantly despite having lower incomes. They may be driven by lifestyle preferences and status-oriented purchases. Tailored promotions for aspirational or branded products could appeal to these customers.
<h5>Cautious High Earners (High Income, Low Spending)</h5>
This segment consists of high-income individuals with lower spending scores. They may be cautious spenders or selective with their purchases. Engaging this group might involve exclusive membership benefits or loyalty programs to increase their mall spending. 

<h4> 3. Visualization of Customer Segments</h4>
To better understand the customer groups, we visualized clusters in a 2D scatter plot. The plot clearly displays how clusters are distributed across Annual Income and Spending Score, making it easier to observe each group’s characteristics and overlap.

<h4>4. Cluster Centers (Centroids)</h4>
Each cluster has a center (centroid) that represents the average values of Annual Income and Spending Score within the group. This provides a quick summary of the characteristics typical for each segment, helping businesses tailor their offerings more precisely.

<h4>Technical Details</h4>
 <h5>K-Means++ Initialization:</h5> We used K-Means++ for smarter centroid initialization, improving clustering performance.
 <h5>Elbow Method Implementation:</h5> We calculated WCSS for 1 to 10 clusters, using the Elbow Method to determine the optimal number of clusters.
 <h5>Data Visualization:</h5> Leveraged Matplotlib and Seaborn for visual styling and cluster plotting.
 <h5>Cluster Centers Extraction:</h5> Used kmeans.cluster_centers_ to determine the coordinates of each cluster center, providing insight into typical customer profiles.</br>
<h4>Results and Insights</h4>
This project successfully segmented customers into distinct clusters, each with unique income and spending characteristics. These insights offer valuable guidance for businesses to:

* Develop targeted promotions and marketing strategies.</br>
* Customize services to meet the needs of each customer segment.</br>
* Improve customer satisfaction and loyalty through more personalized offers.

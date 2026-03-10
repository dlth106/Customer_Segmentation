## Customer Segmentation using RFM + Clustering

This project focuses on customer segmentation based on purchasing behavior indicators such as Recency (the time since the last purchase), Frequency (the number of purchases), and Monetary Value (the amount spent). The goal is to gain a deeper understanding of each customer group in order to recommend appropriate marketing strategies that optimize outreach effectiveness, increase revenue, and enhance customer satisfaction.

Problem Statement:

Businesses often have large numbers of customers with different purchasing patterns. Treating all customers the same can lead to inefficient marketing strategies.

The goal of this project is to:

Identify groups of customers with similar characteristics

Understand purchasing behavior patterns

Provide insights that can help businesses create targeted marketing strategies

## Dataset

The dataset contains transactional data from an online retail store. Each row represents a product purchased within a specific transaction.

The dataset includes the following features:

| Column | Description |
|------|------|
| InvoiceNo | Unique invoice number for each transaction |
| StockCode | Product code identifying the item |
| Description | Product name or description |
| Quantity | Number of items purchased |
| InvoiceDate | Date and time when the transaction occurred |
| UnitPrice | Price per unit of the product |
| CustomerID | Unique identifier for each customer |
| Country | Country where the customer resides |


## Results

Customer segmentation was performed using RFM (Recency, Frequency, Monetary) metrics combined with clustering techniques. The model identified three distinct customer segments based on purchasing behavior.

| Cluster | Recency | Frequency | Monetary Value | Interpretation |
|-------|-------|-------|-------|-------------|
| 0 | 56.17 | 4.33 | 59.71 | Moderate customers who purchase occasionally with moderate spending. |
| 1 | 28.63 | 17.03 | 408.81 | High-value customers who purchase frequently and spend significantly more. |
| 2 | 191.68 | 1.68 | 29.68 | Inactive or low-value customers with infrequent purchases and low spending. |

### Segment Insights

**Cluster 1 – High-Value Customers**  
This group has the lowest recency and the highest frequency and monetary value. These customers purchase frequently and generate the highest revenue, making them the most valuable segment. Businesses should focus on retention strategies such as loyalty programs and personalized promotions.

**Cluster 0 – Regular Customers**  
These customers purchase occasionally with moderate spending levels. They represent a stable customer base and could potentially be converted into high-value customers through targeted marketing campaigns.

**Cluster 2 – Low-Value or Inactive Customers**  
This segment shows the highest recency with low purchase frequency and spending. These customers may require re-engagement strategies such as discounts, email campaigns, or personalized offers.

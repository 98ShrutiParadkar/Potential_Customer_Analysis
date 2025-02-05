# Potential Customer Analysis and Best-Selling Product Identification

### 📋 Project Description

This project is designed to analyze customer characteristics and identify the best-selling products. The goal is to help businesses focus on their most profitable market segments, rather than applying a broad marketing approach.

### 🎯 **Key Features:** 
- Determines the best-selling products to optimize marketing strategies.
- Identifies loyal customer characteristics based on historical data.
- Provides insights on  potential customer for targeted marketing and improved business decision-making.

By leveraging this analysis, businesses can refine their market research efforts, ensuring resources are directed toward the most valuable customer segments and products.

### 🛠️ Technologies Used
- **Python**: Programming language.
- **Matplotlib**: Data visualization.
- **NumPy**: Numerical computations.

### 📊 Dataset Overview
This project uses two datasets:
1. **Transactions Dataset** - Contains records of customer purchases, including transaction ID, product details, purchase date.
2. **Customer Purchase Behavior Dataset** - Includes customer characteristics, Loyalty card number.
- DATE: The date of the transaction.<br>
- STORE_NBR: Store number.
- LYLTY_CARD_NBR: Loyalty card number (unique identifier for customers).
- TXN_ID: Transaction ID.
- PROD_NBR: Product number.
- PROD_NAME: Product name.
- PROD_QTY: Quantity of product.
- TOT_SALES: Total sales amount for the transaction.
- LIFESTAGE: Customer life stage.
- PREMIUM_CUSTOMER: Indicates whether the customer is a Budget, Mainstream or Premium  .

### 📈 Model Architecture
1. **Data Preparation**:
   - Compute the average sales per customer using total sales and customer count.
   - Select relevant features: `total_sales`, `customer_count`, and `avg_sales_per_customer`.
   - Normalize the data using `StandardScaler` to improve clustering performance.

2. **Applying K-Means Clustering**:
   - Use the **K-Means algorithm** with `n_clusters=3` to categorize customers into three distinct segments.
   - Assign cluster labels to each customer.

3. **Identifying Customer Segments**:
   - **Loyal Customers**: Customers in clusters with the highest total sales and average sales per customer.
   - **Potential Customers**: Customers in clusters with high customer counts but lower total sales.

4. **Results Analysis**:
   - Extract and analyze the top loyal and potential customer groups based on total sales and customer count.
   - Identify customer characteristics such as `LIFESTAGE` and `PREMIUM_CUSTOMER` status.

This clustering approach enables businesses to tailor marketing efforts, improve customer retention, and boost sales by focusing on high-value customer groups.

### 📊 Best-Selling Product Analysis

![Image](https://github.com/user-attachments/assets/be01f2a4-280c-44b3-bc2b-845c7d2faf0c)

### 🚀 Customer Segmentation (Loyal & Potential Customers)
- **Loyal Customers:** These customers belong to the cluster with the highest total sales and highest average sales per customer. They make frequent purchases and contribute significantly to revenue.
- **Potential Customers:** These customers belong to the cluster with a high customer count but lower total sales. They have purchasing interest but require targeted marketing to convert them into loyal customers.

![Image](https://github.com/user-attachments/assets/2b3d034e-07b5-4029-b499-c68446395f87)

### 📌 Future Scope
The processed dataset can be further used for predictive modeling and strategic decision-making to enhance customer engagement and retention.

  

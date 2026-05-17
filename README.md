# Supermarket Sales Data Analysis Report

<img width="1384" height="900" alt="image" src="https://github.com/user-attachments/assets/ecf52dff-3212-459b-bb27-4b4211a7d341" />

## 1. Data Overview

The dataset is a supermarket sales record containing transaction details from a fictional retail chain. It includes information about sales across different branches (A and B), cities (New York, Los Angeles, Chicago), customer types, products, and financial metrics. The data likely comes from internal supermarket transaction logs and is suitable for retail performance analysis, customer behavior study, and inventory insights.

The dataset has 253 rows (transactions) and 8 columns: `sale_id`, `branch`, `city`, `customer_type`, `product_name`, `product_category`, `quantity`, and `total_price`. Most columns are categorical (e.g., `branch`, `city`, `product_category`), while quantity and `total_price` are numerical.

## 2. Data Cleaning

**Missing Values**:

- customer_type: 3 missing values
- product_category: 6 missing values
- quantity: 3 missing values

*Handling Missing Values*:
I filled the missing values in categorical columns (`customer_type` and `product_category`) using the mode (most frequent value). For the numerical column quantity, I used the median. Since the number of missing values is small, this method keeps the data reliable.

**Duplicate Rows**:
There were 3 duplicate rows in the dataset. I removed these duplicates to avoid repeated data. After cleaning, the dataset now has 250 rows.

## 3. Descriptive Statistics 
I calculated basic statistical measures for the numerical columns:

<img width="574" height="397" alt="table" src="https://github.com/user-attachments/assets/59424877-fde3-4de0-9996-d3d043eab0cc" />

On average, customers buy 10.62 items per transaction, with an average spending of $124.19. The standard deviation of `total_price` is very high (102.98), indicating a large variation in spending - some transactions are as low as $2.18, while others reach up to $427.14.  

Additionally, the distribution of `quantity` is nearly symmetrical (Skewness close to 0), while `total_price` is slightly right-skewed (positive skewness).

*Categorical Summary*:

- New York has the highest number of transactions.
- Branch A has more sales than Branch B.
- Member customers are slightly more than Normal customers.
- Fruits are the most popular product category.

### 3.1 Sales by Product Category

<img width="620" height="577" alt="1" src="https://github.com/user-attachments/assets/e8cdb50a-4288-4761-ad14-2316a79745f1" />

**Insight 1**: The average quantity purchased per transaction is about 10.61 units, with a median of 11. However, the `total_price` has a very high variation, ranging from $2.18 to $427.14. This shows that while customers buy a similar number of items, the value of each transaction differs greatly. Therefore, the supermarket should focus on upselling and product bundling strategies to increase the average order value.

### 3.2 Customer Type Distribution

<img width="615" height="500" alt="2" src="https://github.com/user-attachments/assets/40e2b87a-39c3-40f8-b811-0b689a47b129" />

**Insight 2**: Branch A in New York dominates the number of transactions. Member customers tend to buy more than Normal customers, and Fruits is the best-selling category. This indicates that the loyalty program is working well. The supermarket should continue to promote the membership program and focus marketing efforts on popular categories like Fruits to further increase sales and expand successful strategies to other branches.

*Author
Phan Ngọc Châu*

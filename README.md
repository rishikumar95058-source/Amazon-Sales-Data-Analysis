Amazon-Sales-Data-Analysis
🛒 Amazon Sales Data Analytics

📌 Project Overview

Amazon Sales Data Analytics is a data analysis project that explores Amazon Sales Data to identify patterns in "product pricing, discounts, customer ratings, reviews, and category performance".
The project uses Python-based data analysis and visualization techniques to transform raw Amazon product data into meaningful business insights.



🎯 Project Objectives

The main objectives of this project are:

* Analyze Amazon product categories
* Understand product pricing patterns
* Analyze discounted and actual prices
* Identify products with the highest discounts
* Analyze customer ratings
* Identify highly rated products
* Identify the most reviewed products
* Analyze customer engagement using rating counts
* Study relationships between price, discount, rating, and reviews
* Generate meaningful business insights from the data

🗂️ Dataset

The dataset contains Amazon product and customer review information.

Main Features

| Column                | Description                      |
| --------------------- | -------------------------------- |
|  product_id           | Unique product identifier        |
|  product_name         | Name of the product              |
|  category             | Product category and subcategory |
|  discounted_price     | Product price after discount     |
|  actual_price         | Original product price           |
|  discount_percentage  | Percentage discount offered      |
|  rating               | Customer rating                  |
|  rating_count         | Number of customer ratings       |
|  about_product        | Product description              |
|  user_id              | Customer identifier(s)           |
|  user_name            | Customer name(s)                 |
|  review_id            | Review identifier(s)             |
|  review_title         | Review title                     |
|  review_content       | Customer review text             |
|  img_link             | Product image URL                |
|  product_link         | Amazon product URL               |


🛠️ Technologies Used

Python
Pandas – Data manipulation and analysis
NumPy – Numerical operations
Matplotlib – Data visualization
Seaborn – Statistical visualization
Jupyter Notebook – Data analysis environment

🔄 Project Workflow

Raw Dataset
     ↓
Data Loading
     ↓
Data Inspection
     ↓
Data Cleaning
     ↓
Missing Value Handling
     ↓
Data Validation
     ↓
Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
Data Visualization
     ↓
Category & Product Analysis
     ↓
Correlation Analysis
     ↓
Analytical Story
     ↓
Interactive Dashboard

🧹 Data Cleaning

The following preprocessing steps were performed:

1. Loaded the Amazon product dataset using Pandas.
2. Inspected the dataset structure and data types.
3. Checked for duplicate records.
4. Removed duplicate products based on `product_id`.
5. Removed currency symbols such as `₹` from price columns.
6. Removed commas from numerical values.
7. Converted `actual_price` to numeric format.
8. Converted `discounted_price` to numeric format.
9. Removed `%` symbols from `discount_percentage`.
10. Converted discount percentage into numeric format.
11. Converted `rating` into numeric format.
12. Converted `rating_count` into numeric format.
13. Handled missing values in rating-related columns.
14. Checked for invalid ratings.
15. Checked for negative discount amounts.
16. Created a `main_category` column from the category hierarchy.
17. Created a `discount_amount` column.


🧮 Feature Engineering

Main Category

The original `category` column contains multiple category levels separated by `|`.

The first category level was extracted into:


main_category


Discount Amount

A new column was created:


discount_amount = actual_price - discounted_price


This helps measure the actual amount saved by customers.

📊 Exploratory Data Analysis

The project investigates several important analytical questions.

1. Rating Distribution

The rating distribution shows how customer ratings are spread across the products.

2. Products by Category

This analysis identifies the categories with the largest number of products.

3. Average Discount by Category

This analysis compares average discount percentages across product categories.

4. Price vs Rating

This visualization examines the relationship between discounted product prices and customer ratings.

5. Rating vs Reviews

This analysis examines the relationship between customer ratings and the number of ratings/reviews received.

6. Top Reviewed Products

This analysis identifies products with the highest number of customer ratings.

7. Top Rated Products

This analysis identifies products with the highest customer ratings.

8. Number of Products by Category

This visualization compares Products by Category.

9. Average Discounted Price by Category

This visualization compares customer satisfaction across product categories and Average Discounted Price by Category.

10. Average Product Rating by Category

This visualization compares Average Product Rating by Category.

11. Correlation Heatmap

The correlation heatmap shows relationships between numerical variables such as:

* Actual Price
* Discounted Price
* Discount Percentage
* Rating
* Rating Count
* Discount Amount

12. Top 15 Highly Rated Amazon Products

This visualization compares Top 15 Highly Rated Amazon Products.

💡 Analytical Story

1. Product Portfolio

The dataset contains products from multiple categories and subcategories. Category analysis helps identify which product groups have the strongest representation in the dataset.

2. Pricing Strategy

Comparing actual prices with discounted prices provides insight into Amazon product pricing patterns and the extent of price reductions offered to customers.

3. Discount Strategy

Discount analysis helps identify categories and products that offer relatively high discounts. This can provide insights into promotional and pricing strategies.

4. Customer Satisfaction

Customer ratings provide an indication of product satisfaction. The rating distribution helps understand the general level of customer feedback across the products.

5. Customer Engagement

`rating_count` helps identify products that receive significant customer attention. Products with large numbers of ratings can indicate strong customer interaction or popularity.

6. Category Performance

Category-level analysis combines:

* Product count
* Average price
* Average discount
* Average rating
* Total rating count

This provides a broader understanding of how different product categories perform.

7. Price and Rating Relationship

The price-versus-rating analysis helps investigate whether product price has a noticeable relationship with customer ratings.

8. Business Perspective

The analysis can help businesses understand:

Which categories have the largest product presence
Which categories provide higher discounts
Which products receive strong customer engagement
Which categories have higher average ratings
How product pricing relates to customer ratings
Which products may require further investigation


📈 Key Business Questions Answered

This project attempts to answer:

1. Which product categories contain the most products?
2. Which categories offer the highest average discounts?
3. Which products have the highest ratings?
4. Which products have the highest number of ratings?
5. What is the average discounted product price?
6. What is the average customer rating?
7. Is there a relationship between price and rating?
8. Is there a relationship between rating and rating count?
9. Which categories have better average customer ratings?
10. How do price, discounts, ratings, and reviews relate to each other?


📂 Project Structure

Amazon Sales Data Analytics/
│
├── Amazon Sales Data Analytics.ipynb
├── amazon_cleaned.csv
├── README.md
│
└── images/
    ├── 1_Distribution_of_Amazon_Product_Ratings.png
    ├── 2_Products_by_Category.png
    ├── 3_Average_Discount_by_Category.png
    ├── 4_Price_vs_Rating.png
    ├── 5_Rating_vs_Reviews.png
    ├── 6_Top_Reviewed_Products.png
    ├── 7_Top_Rated_Products.png
    ├── 8_Number_of_Products_by_Category.png
    ├── 9_Average_Discounted_Price_by_Category.png
    └── 10_Average_Product_Rating_by_Category.png
    └── 11_Correlation_Heatmap.png
    └── 12_Top 15_Highly_Rated_Amazon_Products.png


⭐ Project Highlights

Data Analysis: Python, Pandas, NumPy
Visualization: Matplotlib, Seaborn
Notebook: Jupyter
Project Type: Data Analytics & Business Intelligence

👨‍💻 Author:

N. Rishi Kumar
B.Tech – Artificial Intelligence & Machine Learning

Conclusion:
This project demonstrates data cleaning, exploratory data analysis, and visualization skills using Python to generate meaningful insights from Amazon Sales Data.

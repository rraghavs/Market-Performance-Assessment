# 📊 Market Analysis Dashboard Project
### 📝 Project Description
This project involves creating an interactive and insightful Market Analysis Dashboard using Power BI. The dashboard is powered by a detailed sales dataset (Dataset.csv) and provides an overview of sales performance, customer insights, product trends, and regional analysis.

### 📁 Project Files
Dataset:

File: Dataset.csv
Purpose: Contains raw sales data for analysis and visualization.
Power BI Dashboard:

File: Market_analysis_dashboard.pbix
Purpose: Interactive Power BI dashboard that visualizes key metrics and trends derived from the dataset.
### 🗂️ Dataset Details
File Name: Dataset.csv
Number of Records: 5,901
Number of Columns: 23
Key Columns:
## 🚀 Features of the Power BI Dashboard
Sales Overview:
Total sales, total profit, and number of orders (KPIs).
Monthly and yearly sales trends (line chart).
Product Analysis:
Top 10 products by sales and profit (bar charts).
Category-wise and sub-category-wise performance analysis (stacked charts).
Regional Insights:
Sales and profit by region (map visualization).
Heatmaps for performance comparison across states and cities.
Customer Segmentation:
Segment-wise sales and profit distribution (pie and column charts).
Customer-specific insights and order history.
Returns Analysis:
Insights into returned products and their impact on overall profit.
## 🛠️ Tools and Technologies
Power BI Desktop:
Used for data visualization and dashboard creation.
Power Query:
Data cleaning and transformation.
Python/Excel (Optional):
Pre-processing or additional data analysis before importing into Power BI.
## 🗂️ Steps to Use the Project
#### 1️⃣ Dataset Preparation
Ensure Dataset.csv is available in the same directory as the .pbix file.
Clean and preprocess the dataset using Power Query.
#### 2️⃣ Open the Power BI File
Open the Market_analysis_dashboard.pbix file in Power BI Desktop.
#### 3️⃣ Customize and Explore
Explore the interactive visuals and customize filters for deeper insights:
Time-based slicers.
Region, product, and customer segmentation slicers.
## 📊 Insights You Can Derive
Sales Trends:
Identify seasonal sales patterns and peak performance periods.
Profitability:
Evaluate which products, regions, and customer segments generate the most profit.
Shipping Efficiency:
Assess delivery times and the impact of different shipping modes.
Customer Retention:
Identify high-value customers and their buying patterns.
## 📊 Insights You Can Derive
Sales Trends:
Identify seasonal sales patterns and peak performance periods.
Profitability:
Evaluate which products, regions, and customer segments generate the most profit.
Shipping Efficiency:
Assess delivery times and the impact of different shipping modes.
Customer Retention:
Identify high-value customers and their buying patterns.
## 🔧 Sample Visualization from the Dashboard
import matplotlib.pyplot as plt
import pandas as pd

# Load dataset
data = pd.read_csv('Dataset.csv')

# Top 5 products by sales
top_products = data.groupby('Product Name')['Sales'].sum().sort_values(ascending=False).head(5)

# Plot
top_products.plot(kind='bar', color='orange')
plt.title('Top 5 Products by Sales')
plt.xlabel('Product Name')
plt.ylabel('Total Sales')
plt.show()
## 🖼️ Dashboard Preview


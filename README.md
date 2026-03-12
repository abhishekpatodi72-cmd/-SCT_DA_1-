# -SCT_DA_1-

```python
import pandas as pd

# Load the files to inspect content for a better description
data_file = "superstore_excel_dashboard_task1 (1).xlsx - Data.csv"
dashboard_file = "superstore_excel_dashboard_task1 (1).xlsx - Dashboard.csv"
sales_trend_file = "superstore_excel_dashboard_task1 (1).xlsx - Sales Trend.csv"

df_data = pd.read_csv(data_file)
df_dashboard = pd.read_csv(dashboard_file, skiprows=2) # Adjusting based on snippet showing headers later
df_trend = pd.read_csv(sales_trend_file)

print("Data Columns:", df_data.columns.tolist())
print("\nDashboard Head:\n", df_dashboard.head(10))
print("\nSales Trend Head:\n", df_trend.head())



```

```text
Data Columns: ['Row ID', 'Order ID', 'Order Date', 'Ship Date', 'Ship Mode', 'Customer ID', 'Customer Name', 'Segment', 'Country', 'City', 'State', 'Postal Code', 'Region', 'Product ID', 'Category', 'Sub-Category', 'Product Name', 'Sales', 'YearMonth']

Dashboard Head:
        Total Sales 2261536.7827  Unnamed: 2 Unnamed: 3   Unnamed: 4
0     Total Orders         4922         NaN        NaN          NaN
1              NaN          NaN         NaN        NaN          NaN
2              NaN          NaN         NaN        NaN          NaN
3         Category        Sales         NaN     Region        Sales
4        Furniture  728658.5757         NaN    Central  492646.9132
5  Office Supplies   705422.334         NaN       East   669518.726
6       Technology   827455.873         NaN      South   389151.459
7              NaN          NaN         NaN       West  710219.6845

Sales Trend Head:
      Month      Sales
0  2015-01  14205.707
1  2015-02   4519.892
2  2015-03  55205.797
3  2015-04  27906.855
4  2015-05  23644.303


```

# Superstore Sales Performance Dashboard

This project is a comprehensive **Superstore Sales Dashboard** built using Microsoft Excel. It provides a data-driven overview of a retail store's performance across various regions, categories, and time periods, enabling stakeholders to make informed business decisions.

## 📌 Project Overview

The primary goal of this dashboard is to analyze sales data to identify trends, top-performing categories, and regional strengths. The analysis focuses on key business metrics such as total revenue, order volume, and category-wise performance.

### Key Metrics Tracked:

* **Total Sales:** $2,261,536.78
* **Total Orders:** 4,922
* **Regional Sales Distribution:** Breakdown across Central, East, South, and West regions.
* **Category Analysis:** Performance comparison between Furniture, Office Supplies, and Technology.
* **Sales Trends:** Monthly sales performance tracking over multiple years (2015–2018).

## 📊 Dashboard Features

* **Dynamic KPIs:** Real-time summary of total sales and order counts.
* **Regional Analysis:** Insights into which regions contribute most to the revenue.
* **Product Category Insights:** Comparison of sales volume and value across major product categories.
* **Time-Series Trend:** A monthly sales trend chart to identify seasonal patterns and growth trajectories.

## 🛠️ Tools Used

* **Microsoft Excel:** - Data cleaning and preprocessing (handling missing values, formatting dates).
* Pivot Tables for data aggregation.
* Data Visualization (Line charts, Bar charts, and KPI cards).
* Formulas (SUM, COUNT, etc.) for metric calculation.



## 📂 Dataset Description

The analysis is based on the **Superstore Dataset**, which includes:

* **Order Details:** Order ID, Order Date, Ship Date, Ship Mode.
* **Customer Information:** Customer Name, Segment, City, State, Region.
* **Product Details:** Category, Sub-Category, Product Name.
* **Sales Data:** Sales figures per transaction.


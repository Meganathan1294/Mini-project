# Mapping Snitch Fashion Sales: End-to-End Data Transformation & Visualization

## 📌 Project Overview
This project involves transforming raw, uncleaned retail data into a structured format to analyze product profitability, regional growth, and the impact of discounts on the company's bottom line. The analysis is based on a dataset of 2,500 rows with significant missing values across multiple columns.

## 🛠️ Tech Stack
*   **Data Cleaning & Transformation:** Microsoft Excel (Advanced Formulas, Index/Match)
*   **Business Intelligence:** Power BI (DAX, Interactive Visualization)

## 🧹 Data Lifecycle & Cleaning Highlights
To ensure the integrity of the analysis, a rigorous cleaning process was followed:
*   **Missing Unit Prices:** Imputed missing values by calculating the **AVERAGEIF** unit price for the same Product Name.
*   **Discount & Units Sold:** Missing discounts were filled using the **MEDIAN** of the column, while missing unit counts were defaulted to a median of 2.
*   **Categorical Standardization:** Corrected inconsistent city names (e.g., standardizing "hyd" and "hyderbad" to "Hyderabad").
*   **Derived Columns:** 
    *   **Sales After Discount:** Calculated as `Units sold * Unit price * (1 - discount %)`.
    *   **Profit Status:** Categorized as "Profit" or "Loss" based on a threshold of Rs. 500.
*   **Date Handling:** Missing order dates were filled using the **MODE** of the available dates.

## 📊 Business Intelligence Dashboards
The project features a comprehensive Power BI suite consisting of three specialized reports:

### 1. Executive Sales & Performance
*   **KPI Gauge:** Shows a total revenue of **5.49M** against target goals.
*   **Top Categories:** Identifies **Dresses and Accessories** as the leading revenue drivers.
*   **Segment Analysis:** Highlights **B2B** as a larger contributor to total revenue than B2C.

### 2. Product & Inventory Insights
*   **Regional Trends:** Visualizes that Mumbai excels in Dresses while Hyderabad performs strongly in Jackets.
*   **Pricing Analysis:** Tracks a downward trend in average unit price from 2023 to 2025, indicating volume-driven growth.
*   **Inventory Movement:** Identifies **Classic Tees and Puffer Coats** as the highest-volume items, each exceeding 200 units sold.

### 3. Customer & Segment Analysis
*   **Market Growth:** Displays a massive surge in total revenue and B2B volume moving into 2025.
*   **Promotional Impact:** Shows a linear increase in discount volume, suggesting that growth is being driven by aggressive promotional pricing.

## 📂 Project Assets
*   `Mini Project.xlsx`: The final cleaned and transformed dataset.
*   `Snitch_Fashion_Sales_Uncleaned.xlsx`: The original raw data used for the cleaning workflow.
*   `mini project dashboard.pbix`: The complete Power BI project file.

## 👤 Author Information
*   **Name:** R. Meganathan
*   **Batch:** DA-ANB11
*   **Mentor:** Kumaran
*   **Submission Date:** January 8, 2026

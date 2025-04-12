# Sales & Marketing Performance Dashboard

[![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=for-the-badge&logo=powerbi)](https://powerbi.microsoft.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

## Project Overview

This repository contains a comprehensive Sales & Marketing Performance Dashboard developed using Microsoft Power BI. The dashboard provides a holistic view of key performance indicators (KPIs) across various dimensions, enabling data-driven decision-making for sales strategies, marketing campaign effectiveness, and overall business growth. It integrates data across multiple years (2022, 2023, 2024), offering trend analysis and year-over-year (YoY) comparisons.

The primary goal of this dashboard is to empower stakeholders with actionable insights by visualizing complex data related to revenue, costs, profitability, customer engagement, lead sources, sales channels, marketing campaigns, regional performance, and product-level details.

## Key Features

*   **Multi-Year Analysis:** Interactive slicer to filter data by year (2022, 2023, 2024), allowing for temporal analysis and performance tracking over time.
*   **KPI Monitoring:** Prominent display of critical metrics like Total Revenue, Cost, Profit, Average Conversion Rate, and Views, including Year-over-Year (vs PY) percentage changes.
*   **Trend Analysis:** Visualization of monthly revenue trends, comparing the selected year against the previous year (Revenue PM).
*   **Segmentation:** Detailed breakdown of revenue by:
    *   Lead Source (Email, Referral, Social Media, Cold Calling, Website)
    *   Sales Channel (In-Store vs. Online)
    *   Marketing Campaign Effectiveness
    *   Geographical Region (Europe, Asia, North America, South America)
    *   Country-level performance (including Sessions and Revenue)
*   **Product-Level Insights:** A dedicated "Product Details" view offering granular information on individual products, including ratings, stock levels, pricing, views, revenue, cost, and profit, along with trend sparklines.
*   **Interactive Visualizations:** Leverages various Power BI visuals like KPI cards, line charts, bar charts, donut charts, tables with sparklines, and maps for intuitive data exploration.
*   **Data Comparison:** Built-in YoY comparison calculations provide immediate context on performance relative to the previous period.

## Dashboard Sections

The dashboard is organized into two main views:

### 1. Overview Tab

This tab provides a high-level executive summary of the overall Sales and Marketing performance.

*   **Top KPIs:** Displays core financial and engagement metrics with YoY comparisons.
*   **Revenue by Month:** Tracks monthly revenue fluctuations and compares them with the previous year's performance.
*   **Revenue by Lead Source:** Identifies the most effective channels driving revenue.
*   **Revenue by Sales Channel:** Shows the contribution of In-Store vs. Online channels to total revenue.
*   **Revenue by Marketing Campaign:** Assesses the performance and ROI of different marketing initiatives.
*   **Revenue by Region:** Highlights the geographical distribution of revenue.
*   **Revenue & Session by Country:** Provides a ranked view of country-level performance based on sessions and revenue, complemented by a world map visualization.
  
![Dashboard Overview](https://github.com/vincenzomaltese/Sales-Marketing-Performance-Dashboard/blob/main/images/Overview.jpg)
### 2. Product Details Tab

This tab allows for a deep dive into the performance of individual products.

*   **Product Listing:** A detailed table showing key product attributes and performance metrics.
*   **Metrics:** Includes Product ID, Name (with image), Rating, Scoring, Stock levels, Number of Invoices, Price, Views, Revenue, Cost, and Profit per product.
*   **Trend Sparklines:** Embedded line charts visualizing the monthly trend for Revenue, Cost, and Profit for each product within the selected year.
*   **Search Functionality:** Enables users to quickly find specific products.

![Product Details View](https://github.com/vincenzomaltese/Sales-Marketing-Performance-Dashboard/blob/main/images/product_details.jpg)

## Technical Details

*   **Tool:** Microsoft Power BI Desktop
*   **Data Sources:** (Assumed - Specify if known) Likely sourced from relational databases (Sales DB, CRM), flat files (CSVs, Excel), web analytics platforms, and marketing automation tools.
*   **Data Modeling:** A relational data model potentially following a star schema, connecting fact tables (e.g., Sales Transactions, Website Sessions) with dimension tables (e.g., Date, Product, Customer, Region, Campaign, Lead Source).
*   **Key DAX Measures:** Calculations for Total Revenue, Cost, Profit, Avg Conversion Rate, Views, YoY Growth Rates (vs PY), Previous Month Revenue (Revenue PM), and percentage contributions for various segments.

## How to Use This Repository

This repository provides multiple ways to explore the Sales & Marketing dashboard and its underlying data:

1.  **View Static Report (PDF):**
    *   **Best for:** Quickly viewing the dashboard's key visuals and insights without installing Power BI.
    *   **Requires:** A PDF reader.
    *   **Steps:**
        1.  Download the `Sales&Marketing.pdf` file from this repository. 
        2.  Open the file using any PDF viewer.
    *   **Note:** This is a static export and is not interactive.

2.  **Explore Interactive Report (PBIX):**
    *   **Best for:** Full interactive experience, drilling down into data, exploring the data model, and viewing DAX measures.
    *   **Requires:** Microsoft Power BI Desktop (available for free [here](https://powerbi.microsoft.com/en-us/desktop/)).
    *   **Steps:**
        1.  Ensure you have Power BI Desktop installed.
        2.  Download the `Sales&Marketing.pbix` file from this repository.
        3.  Open the `.pbix` file using Power BI Desktop.
        4.  Interact with the report:
            *   Use the **Year slicer** at the top to filter data (2022, 2023, 2024).
            *   Navigate between the **"Overview"** and **"Product Details"** tabs.
            *   Click on elements within charts (e.g., a region, a campaign) to **cross-filter** other visuals.
            *   Hover over visuals for **tooltips** with more details.
            *   Use the **search bar** in the "Product Details" tab.

3.  **Access Raw Data (CSV):**
    *   **Best for:** Examining the source data used for the dashboard or performing independent analysis.
    *   **Requires:** Any tool capable of reading CSV files (e.g., Excel, Google Sheets, Python with Pandas, R).
    *   **Steps:**
        1.  Download the `sales_data.csv` file from this repository.
        2.  Open or import the file using your preferred tool.

## Potential Enhancements

*   Incorporate customer segmentation analysis (e.g., RFM).
*   Add predictive forecasting for key metrics.
*   Integrate sentiment analysis based on product ratings or reviews.
*   Include A/B testing results for marketing campaigns.
*   Develop more granular cost allocation models.


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details (assuming you choose MIT).

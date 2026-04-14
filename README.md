# 🛒 End-to-End E-Commerce Sales Analysis

A comprehensive Excel-based data analytics project that explores transactional data from an e-commerce platform to uncover insights on sales performance, logistics efficiency, customer behavior, and business profitability.

---

## 📁 Project Structure

```
e_commerce_dataset.xlsx
├── Cleaned Data          # Preprocessed and transformed dataset
├── Data Understanding    # Initial exploration and data profiling
├── Descriptive Statistics# Summary statistics for key metrics
├── Pivot Table Analysis  # Multi-dimensional breakdowns
├── What-If Analysis      # Scenario modeling for cost variables
├── Scenario Summary      # Summarized scenario comparison results
├── Data Visualization    # Charts and visual analysis
├── Forecast              # Shipping cost forecasting by delivery days
├── Dashboard             # Interactive KPI dashboard
└── Insights              # Key business takeaways
```

---

## 📊 Dataset Overview

| Attribute         | Details                                      |
|-------------------|----------------------------------------------|
| **File**          | `e_commerce_dataset.xlsx`                    |
| **Records**       | ~4,300 transactions                          |
| **Time Period**   | 2019 onwards                                 |
| **Product Categories** | Laptop, Mobile, Tablet, TV, PC, Gaming Console |
| **Geography**     | Multiple Indian cities and states            |

### Key Columns

| Column | Description |
|---|---|
| `order_id` | Unique order identifier |
| `Product_category_cleaned` | Standardized product category |
| `origin_city` / `destination_city` | Shipment route details |
| `destination_state` | Delivery state |
| `logistics_provider_name` | Carrier/logistics partner |
| `final_delivery_status` | Delivered / Returned |
| `Payment Mode` | Credit Card, Debit Card, etc. |
| `Sources` | Order source — App or Website |
| `dispatch_date` / `actual_delivery_date` / `promised_delivery_date` | Delivery timeline |
| `Delivery Days` | Calculated transit duration |
| `transit_storage_cost` | Cost incurred during transit |
| `shipping_cost` | Final shipping cost |
| `Session_length` | Customer session duration |

---

## 🔧 Methodology

### 1. Data Understanding & Exploration
- Examined dataset structure, data types, and distributions
- Identified missing values and anomalies

### 2. Data Cleaning & Preparation
- **Missing Values** — Handled using mean/zero replacement based on business context
- **Duplicates** — Removed using unique order identifiers
- **Column Standardization** — Renamed columns for consistency (spaces → underscores)
- **Data Type Correction** — Dates parsed to proper formats; numeric fields cast correctly
- **Derived Columns Created:**
  - `Order_Year`, `Order_Month`, `Order_Day`
  - `Total_Sales`, `Discounted_Price`, `Cost_Price`
  - `Profit`, `Profit_Percentage`
  - `Sales_Category` (Low / Medium / High, threshold-based)
- **Outlier Handling** — Detected and treated using boxplots and statistical boundaries

### 3. KPI & Formula-Based Analysis
Key business KPIs computed:
- Total Sales & Total Profit
- Average Order Value (AOV)
- Total Orders & Total Customers
- Average Discount & Average Profit Percentage
- Total Product Categories

### 4. Descriptive Statistics
Summary statistics (mean, median, std dev, min, max) calculated for all key numerical metrics.

### 5. Pivot Table Analysis
Multi-dimensional analysis across product categories, cities, logistics providers, payment modes, and delivery performance.

### 6. What-If & Scenario Analysis
- Modeled the effect of varying transit cost discount rates on overall logistics spend
- Compared Current vs. Optimized cost scenarios using Excel's Scenario Manager

### 7. Forecasting
- Forecasted `shipping_cost` as a function of `Delivery Days`
- Includes lower and upper confidence bounds for predictions

### 8. Data Visualization & Dashboard
Interactive dashboard visualizing:
- Sales and profit trends over time
- Category-wise and product-wise performance
- Discount vs. profit relationship
- Customer purchase behavior by source and payment mode
- KPI summary cards for executive overview

---

## 💡 Key Insights

- Product categories such as **Laptops** and **Mobiles** dominate order volumes
- Delivery performance (on-time vs. returned) varies significantly across logistics providers and routes
- **App-based** orders show distinct session behavior vs. website orders
- Shipping costs and transit storage costs can be optimized based on scenario modelling results
- Forecast analysis reveals a relationship between delivery duration and shipping cost

---

## 🛠 Tools Used

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Core platform for all analysis, visualization, and dashboarding |
| Excel Pivot Tables | Multi-dimensional data aggregation |
| Excel Formulas (DAYS, IF, etc.) | KPI calculation and derived columns |
| Excel Scenario Manager | What-if and scenario analysis |
| Excel Forecast Sheet | Time-series forecasting |
| Excel Charts & Slicers | Interactive dashboards |

---

## 🚀 How to Use

1. **Clone or download** this repository
2. Open `e_commerce_dataset.xlsx` in **Microsoft Excel** (2016 or later recommended for full feature support)
3. Navigate through the sheets in order — start with **Cleaned Data**, then explore **Pivot Table Analysis**, **Dashboard**, and **Insights**
4. Use slicers and filters in the **Dashboard** sheet to interact with the data
5. Refer to **What-If Analysis** and **Scenario Summary** sheets to explore cost optimization scenarios

---

## 👤 Author

**Sarthak Somani**
*Data Analytics Project — January 2026*

---

## 📄 License

This project is for educational and portfolio purposes. The dataset is used solely for analytical demonstration.

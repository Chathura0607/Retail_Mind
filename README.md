# Strategic Growth Analysis for Unique Gifts Ltd.

## 📘 Project Overview

This project was conducted as a capstone assignment for the **ITS 2122: Python for Data Science & AI** module. Our team acted as data science consultants for **Unique Gifts Ltd.**, a UK-based online retailer. The primary goal was to transform two years of raw transactional data into actionable business intelligence to guide strategic decision-making in marketing, inventory, and customer relationship management.

## 🎯 Business Objectives

The analysis was designed to answer key strategic questions for the client:

1.  **Sales Performance & Seasonality:** Identify sales trends and seasonal patterns to optimize inventory and marketing.
2.  **Product Portfolio Optimization:** Distinguish between high-volume ("Bread & Butter") and high-value ("Cash Cow") products to refine sales strategies.
3.  **Geographic Footprint:** Analyze revenue distribution to identify growth opportunities in domestic (UK) and international markets.
4.  **Customer Segmentation:** Move beyond a one-size-fits-all approach by segmenting customers based on purchasing behavior using the RFM model.
5.  **Wholesaler vs. Retail Analysis:** Investigate and validate the existence of a wholesale customer segment to develop tailored B2B strategies.

## ⚙️ Technical Stack

*   **Language:** Python 3
*   **Libraries:**
    *   `pandas` & `numpy` for data manipulation and analysis
    *   `matplotlib` & `seaborn` for data visualization
    *   `requests` for API integration
*   **Environment:** Jupyter Notebook
*   **Key Techniques:** Data Cleaning, Exploratory Data Analysis (EDA), Time-Series Analysis, RFM Customer Segmentation, API Integration.

## 📊 Dataset

The analysis is based on the **"Online Retail II"** dataset from the UCI Machine Learning Repository, containing over 1 million transactions from Dec 2009 - Dec 2011.

**Data Dictionary:**
| Column | Type | Description |
| :--- | :--- | :--- |
| `Invoice` | object | Unique 6-digit transaction number. Prefix 'C' indicates a cancellation. |
| `StockCode` | object | Unique 5-digit code identifying each product. |
| `Description` | object | Name/description of the product. |
| `Quantity` | int64 | Number of units per transaction. Negative values indicate cancellations. |
| `InvoiceDate` | object | Date and time the transaction was generated. |
| `Price` | float64 | Unit price of the product in GBP (£). |
| `Customer ID` | float64 | Unique 5-digit identifier for each customer. |
| `Country` | object | The country where the customer resides. |

## 🔧 Methodology & Project Phases

Our analysis followed a structured, five-phase approach:

1.  **Data Sanitation & Preprocessing:** Cleaned the raw data by handling missing values, removing cancelled orders and non-product transactions, and performing feature engineering (e.g., creating `TotalPrice` and datetime features).
2.  **Exploratory Data Analysis (EDA):** Analyzed sales trends, seasonality, geographic revenue distribution, and product performance.
3.  **Advanced Analytics - RFM Segmentation:** Implemented the Recency, Frequency, Monetary model to segment the customer base into actionable groups (e.g., Champions, Loyal Customers, At-Risk).
4.  **Strategic Recommendations:** Analyzed the customer base to confirm the "Wholesaler Hypothesis" and formulated data-driven strategies.
5.  **Data Enrichment via API:** Integrated a currency exchange API to convert transaction values from GBP to USD and EUR for enhanced financial reporting.

## 📈 Key Insights & Recommendations

### **1. Exceptional Growth with High Seasonality**
*   **Finding:** A **127% increase** in monthly revenue from 2010 to 2011, with **34.6% of all revenue** generated in Q4 (holiday season).
*   **Recommendation:** Launch targeted Q4 marketing campaigns by September. Develop a "New Year, New You" promotion for January to combat the post-holiday sales dip.

### **2. Product Strategy Requires Rebalancing**
*   **Finding:** A clear divergence between top products by quantity sold (e.g., 'WORLD WAR 2 GLIDERS') and by revenue generated (e.g., 'PAPER BAG RETROSPOT').
*   **Recommendation:** Use popular, low-cost items as lead magnets to cross-sell customers into higher-margin "Cash Cow" products. Feature high-value products more prominently.

### **3. Customer Base Duality: Retail vs. Wholesale**
*   **Finding:** RFM analysis revealed that **13.4% of customers ("Champions") drive 36.2% of revenue**. A bimodal spending distribution confirmed a distinct segment of high-value wholesale clients.
*   **Recommendation:** Immediately segment B2B and B2C customers. Develop a dedicated wholesale channel with account management, volume pricing, and exclusive product lines.

## 👥 Team

This project was completed by the Data Science Consultancy Team as part of the Graduate Diploma in Software Engineering at the Institute of Software Engineering (IJSE).

## 📄 Final Deliverables

1.  **Strategic Insights Report (`Strategic_Insights_Report-final.pdf`):** A polished business report detailing findings, visualizations, and strategic recommendations for the executive board.
2.  **Technical Appendix (`Technical_Appendix.ipynb`):** A well-documented Jupyter Notebook containing all code, from data cleaning to advanced analysis, ensuring full reproducibility.

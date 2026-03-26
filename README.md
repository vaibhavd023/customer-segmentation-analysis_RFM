# customer-segmentation-analysis_RFM
Customer segmentation analysis using RFM with Python.

# Customer Segmentation Analysis - RFM Model

## Project Overview
This project performs **RFM (Recency, Frequency, Monetary)** analysis on the Online Retail II dataset to segment customers and provide actionable business strategies. The analysis helps identify high-value customers, at-risk customers, and lost opportunities to optimize marketing efforts and increase revenue.

---

## Dataset

This project uses the **Online Retail II** dataset from the UCI Machine Learning Repository.

**Description**:  
This Online Retail II data set contains all the transactions occurring for a UK-based and registered, non-store online retail between **01/12/2009** and **09/12/2011**. The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.

- **Number of entries**: 1,067,371  
- **Number of columns**: 8  
- **File size**: ~43.5 MB (Excel format)

### Columns Description

| Column       | Description |
|--------------|-----------|
| **Invoice**      | Invoice number. A 6-digit integral number uniquely assigned to each transaction. If this code starts with 'C', it indicates a cancellation. |
| **StockCode**    | Product (item) code. A 5-digit integral number uniquely assigned to each distinct product. |
| **Description**  | Product (item) name. |
| **Quantity**     | The quantities of each product (item) per transaction. |
| **InvoiceDate**  | Invoice date and time. |
| **Price**        | Unit price in sterling (£). |
| **CustomerID**   | Customer number. A 5-digit integral number uniquely assigned to each customer. |
| **Country**      | Country name where the customer resides. |

### Download Links

- Official Source: [UCI Machine Learning Repository - Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii)
- Alternative (CSV format on Kaggle): [Online Retail II on Kaggle](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci)

> **Note**: The full dataset is **not included** in this repository due to its large size (>25 MB). Please download it using the links above and place it in the `data/` folder before running the notebook.

---

## Key Findings & Strategic Recommendations

### RFM Segment Overview

| RFM Segment              | Customers | Revenue      | Recommended Strategy                          |
|--------------------------|-----------|--------------|-----------------------------------------------|
| **Champions**            | 1,079     | £5,587,668   | VIP treatment, loyalty rewards, exclusive offers |
| **Best Customers**       | 320       | £724,522     | Premium support, early access to new products |
| **Can't Lose Them**      | 327       | £679,578     | High-value focus, personalized service        |
| **Lost Customers**       | 1,253     | £394,579     | Upsell opportunities, cross-selling           |
| **Loyal Customers**      | 287       | £260,644     | Win-back campaigns, special incentives        |
| **Lost - Big Spenders**  | 129       | £243,343     | Immediate re-engagement, special offers       |
| **Good Customers**       | 189       | £172,574     | Aggressive win-back campaign                  |
| **Hibernating**          | 349       | £160,620     | Low priority, automated campaigns only        |
| **Low-Value Customers**  | 274       | £66,907      | Budget-friendly reactivation offers           |
| **At Risk - Big Spenders**| 33       | £55,571      | Convert to higher-value segment               |
| **Potential**            | 74        | £48,790      | Cross-sell and upsell strategies              |

### Conclusion & Strategic Action Plan

The business is **heavily dependent** on a small number of top-tier customers (**Champions** and **Best Customers**), while struggling to convert and grow the much larger base of mid and lower-tier segments. This over-reliance, combined with weak conversion pipelines from other RFM tiers, is driving high overall churn.

The core issue is not just retention — it's **ineffective conversion** from lower segments into higher-value ones.

#### Four Key Strategic Initiatives

1. **Protect the Core**  
   Deliver VIP treatment, loyalty rewards, and exclusive offers to **Champions** to maintain their high engagement and lifetime value.

2. **Aggressive Win-Back**  
   Launch targeted win-back campaigns with special incentives for **Lost Big Spenders** and **Lost Customers**.

3. **Strengthen the Conversion Pipeline**  
   Focus on moving **Good Customers** and **Potential** customers into higher RFM segments through cross-selling, upselling, and personalized nurturing.

4. **Proactive Churn Management**  
   Implement a churn prediction system to identify **At-Risk** customers early and intervene before they move to "Lost" segments.

---

**Business Impact**: Implementing these initiatives can significantly reduce dependency on top customers, improve retention rates, and unlock revenue growth from the larger customer base.

---

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/customer-segmentation-rfm.git
   cd customer-segmentation-rfm

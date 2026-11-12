# 📊 Retail Diagnostic & Profitability Root-Cause Analysis

## 📌 Project Overview
This project moves beyond basic Exploratory Data Analysis (EDA) to conduct a deep operational diagnostic on the **Sample Superstore** dataset. The primary objective is to isolate the root causes of financial leakage, identify loss-making product sub-categories, pinpoint geographical fault lines, and establish precise discount thresholds where profitability flips from positive to negative.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Libraries:** `pandas`, `numpy`, `seaborn`, `matplotlib`
* **Workflow:** Data cleaning, advanced aggregation (`groupby`, `agg`), multi-level filtering, and data visualization.

---

## 🔍 Key Findings & Insights

1. **High-Level Performance vs. Reality:**
   * While categories like *Technology* ($146.5k profit) and *Office Supplies* ($126.0k profit) drive strong overall returns, *Furniture* generates massive sales ($754.7k) but an disproportionately low profit ($19.7k).
2. **Loss-Driving Sub-Categories:**
   * **Tables** (-$17.7k) and **Bookcases** (-$3.6k) in Furniture, along with **Supplies** (-$1.2k) in Office Supplies, are the primary sources of financial leakage.
3. **Discount Tipping Points:**
   * Data reveals a critical threshold: **discounts exceeding 20% (0.20)** consistently flip transactions into severe net losses (e.g., Tables discounted at 40-50% cause an average loss exceeding $200 per order).
4. **Geographical & Product Localization:**
   * Losses are heavily concentrated in key metropolitan areas, specifically **New York City** and **Philadelphia**.
   * Specific SKUs (such as heavy conference tables like *Chromcraft Bull-Nose Wood Oval Conference Table*) generate outsized losses relative to units sold.

---

## 💡 Strategic Recommendations

* **Enforce Strict Discount Caps:** Implement automated approval workflows in the CRM/ERP system to block discounts above 15%–20% on vulnerable items like Tables and Bookcases.
* **Logistics Audit:** Conduct a targeted fulfillment and shipping cost audit in high-loss regions (NYC & Philadelphia) to identify regional expense inflation.
* **Portfolio Optimization:** Phase out or renegotiate vendor terms for extreme loss-making product variants.

---

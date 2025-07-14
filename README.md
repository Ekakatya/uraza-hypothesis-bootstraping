![Matrix](Title.png)
# 📊 Impact of Uraza-Bayram on FMCG Sales: A Bootstrapping Analysis

## 🧾 Project Overview
This project investigates whether the Islamic holiday **Uraza-Bayram (Eid al-Fitr)** significantly boosts **confectionery product sales** in **Muslim-majority Russian regions**, specifically **Tatarstan** and **Bashkortostan**, compared to other regions.

**Hypothesis:**  
Sales of confectionery items increase significantly during Uraza-Bayram in Muslim-majority regions due to cultural and religious purchasing behaviors.

---

## 🏢 Business Context

While Uraza-Bayram is not directly linked to confectionery consumption, it is often accompanied by:

- 🎁 Gift-giving traditions (sweets and treats)
- 🛍️ Region-specific purchasing behavior
- 📈 Localized marketing impact potential

Understanding this can help optimize **promo planning** and **regional marketing strategies**.

---

## 📅 Data Description

### Time Periods

| Period              | Weeks     | Purpose     |
|---------------------|-----------|-------------|
| Pre-holiday period  | Weeks 5–8 | Baseline    |
| Holiday period      | Weeks 9–12| Test period |

### Dataset Columns

| Column            | Description                          | Type     |
|-------------------|--------------------------------------|----------|
| `Product Code`     | Unique product identifier            | string   |
| `Technology`       | Product type or category             | string   |
| `YearWeek`         | Year and week in `YYYYWW` format     | integer  |
| `Turnover Qty`     | Sales volume (in tons)               | float    |
| `Outlet Region`    | Russian region where sale occurred   | string   |

---

## 🧪 Methodology

### 1. Data Preparation
- Cleaned missing/inconsistent values  
- Removed duplicate records  

### 2. Experimental Design
- **Test Group**: Republic of Tatarstan & Republic of Bashkortostan  
- **Control Group**: Other Russian regions  

### 3. Analysis Approach: Difference-in-Differences (DiD)

\[
Y = β₀ + β₁ \cdot \text{Post} + β₂ \cdot \text{Treatment} + β₃ \cdot (\text{Post} \times \text{Treatment}) + ε
\]

- `Post`: Indicator variable for holiday period (Weeks 9–12)  
- `Treatment`: Indicator variable for test region  
- `Post × Treatment`: Interaction effect capturing holiday uplift  

---

## ✅ Project Conclusion

- **Tatarstan** showed a **significant increase** in confectionery sales during Uraza-Bayram  
- **Bashkortostan** displayed **weaker or statistically insignificant** impact  
- **Business Recommendation**:
  - Focus holiday marketing campaigns in **Tatarstan**
  - Include **Bashkortostan** in secondary campaigns due to its large Muslim population  

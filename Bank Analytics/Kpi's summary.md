
# 💰 Bank Analytics Dashboard – KPI Summary

This project presents an **interactive financial analytics dashboard** built in **Microsoft Power BI** to analyze **loans, revenue, collections, and branch performance**.  
It delivers a **high-level KPI view** along with drill-down capabilities by branch, bank, product code, religion, and year.

---

## 🟥 KPI Design
- KPI cards for:
  - **Total Loans**
  - **Total Funded Amount**
  - **Total Collection**
  - **Total Revenue**
  - **Total Interest Earned**

---

## 📈 KPI Summary – Bank Analytics

The dashboard provides an **overview of loan distribution, collection efficiency, and revenue performance** across different branches, banks, and customer segments.

### 🔢 Core Metrics
- **Total Loans:** **65.54K**
- **Total Funded Amount:** **733M**
- **Total Collection:** **808.38M**
- **Total Revenue:** **2.42B**
- **Total Interest Earned:** **3.75M**

---

### 🧠 Key Insights
1. **Branch Loan Distribution**
   - *Mathura* leads with **2.1K loans**, followed closely by *Fatehgarh* and *Haridwar* (~2K each).
   - Smaller branches like *Khordha*, *Behro*, and *Samastipur* have fewer than **1.5K loans**.

2. **Loan Demographics**
   - The **26–35 age group** dominates loan disbursement (**261M funded**), followed by **36–45** (**243M**).
   - The **56–63 age group** has minimal loan volume (**19M**).

3. **Collections by Product Code**
   - **XLG** category generates the largest collections (**708.34M**).
   - **IML** and **XLS** products contribute less than **1M** each.

4. **Loan Trends Over Time**
   - Peak lending occurred in **2018** with **25.9K loans**.
   - A noticeable decline after **2019**, with only **2.4K loans** in 2020.

5. **Religious Segmentation**
   - **Hindu borrowers** dominate (≈ **49K loans**).
   - **Sikh** and **Muslim** communities account for **9K** and **7K** loans respectively.

> These insights enable the bank to optimize product offerings, strengthen underperforming branches, and target the right demographic segments.

---

## 📂 About the Dataset

### Data Fields
- **Loan Details:** LoanID, BranchName, LoanAmount, FundedAmount, Collection, Revenue, Interest
- **Customer Demographics:** AgeGroup, Religion
- **Product Details:** ProductCode, DisbursementDate
- **Bank Data:** BankName, TotalLoans, SumOfLoanAmount

### Modeling & Measures (DAX Highlights)
- `Total Revenue = SUM(Loans[Revenue])`
- `Total Collection = SUM(Loans[Collection])`
- `Loan Count = COUNT(Loans[LoanID])`
- `Funded Amount = SUM(Loans[FundedAmount])`
- `Interest Earned = SUM(Loans[Interest])`

---

## 🔗 Quick Navigation
- *[README.MD](https://github.com/mdsamreen414/Power-BI/blob/main/Bank%20Analytics/README.md)*
- *[Screenshots](https://github.com/mdsamreen414/Power-BI/tree/main/Bank%20Analytics/SS.md)*

---

## 🧕 **About Me**  
📍 Hyderabad, India  
I'm **Md Samreen**, a certified **Data Analyst** with expertise in [**Excel**](https://github.com/mdsamreen414/Excel), [**Power BI**](https://github.com/mdsamreen414/Power-BI), [**MYSQL**](https://github.com/mdsamreen414/MYSQL), and [**Tableau**](https://github.com/mdsamreen414/Tableau). I specialize in turning raw datasets into insightful and interactive dashboards that empower data-driven decisions.  

**Technical Skills**  
Proficient in advanced Excel functions, data cleaning and transformation, SQL queries, and KPI reporting. Skilled in designing dynamic visualizations using Power BI and Tableau, along with database management in MySQL.  

**Soft Skills**  
Strong in problem-solving, analytical thinking, and attention to detail. Adaptable, collaborative, and effective in communicating insights to both technical and non-technical audiences.  

**Portfolio**  
📌 Visit my portfolio: [**Portfolio Website**](https://your-portfolio-link.com)  



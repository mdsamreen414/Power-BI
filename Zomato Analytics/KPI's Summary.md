# 🍽️ Zomato Restaurant Analytics Dashboard

This project showcases a comprehensive restaurant analysis built in **Microsoft Power BI**. It highlights KPIs, cuisine performance, cost trends, service availability, and time-based patterns. The work involved data cleaning, DAX measures, model design, and interactive report building.

---

### 🟥 KPI Design
- KPI cards for:
  - **Count of Cuisines**
  - **Count of Countries**
  - **Total Restaurants**
  - **Average Rating**
  - **Total Cities**

### 🖼️ Dashboard Creation
- Interactive slicers: **Country**, **Restaurant Name**, **Year**, **Cuisine**
- Visuals used: KPI cards, clustered bars, combo (bar+line), gauge, map, and small-multiple trends

---

## 📈 KPI Summary – Zomato Analytics

The dashboard provides a high-level view of restaurant distribution, ratings, and costs across regions and cuisines, with drill-downs by year and restaurant.

### 🔢 Core Metrics
- **Count of Cuisines:** **1,826**
- **Count of Countries:** **15**
- **Total Restaurants:** **9,551**
- **Average Rating:** **2.89**
- **Total Cities:** **141**

### 🧠 Key Insights
1. **Cuisine Performance**
   - *North Indian* has the highest cumulative ratings (~2,009), followed by *North Indian, Chinese* (~1,352).
   - Fusion/dual cuisines are prominent in metropolitan markets.

2. **Top Restaurants by Rating**
   - *Talaga Sampireun* leads (sum rating ≈ **14.7**), with *Sushi Masa* next (≈ **4.9**).

3. **Cost Trends**
   - Highest **Avg Cost for Two** observed at *Satoo – Hotel Shangri-La* and *Skye* (≈ **0.80M** in local currency).
   - Yearly cost pattern (2010–2018) is broadly stable with minor fluctuations.

4. **Service Availability**
   - “Delivering Now” is very limited (≈ **0.36%**).
   - **Online Ordering** enabled for ≈ **25.66%** of restaurants.

5. **Yearly Distribution**
   - Restaurant counts are steady across 2010–2018, peaking near **2018**.

> These insights help benchmark cuisine popularity, pricing, and service maturity across cities and countries.

---

## 📂 About the Dataset

### Data Fields
- **Restaurant Details:** RestaurantName, City, CountryName
- **Cuisines:** Single and multi-cuisine labels (e.g., *North Indian, Chinese*)
- **Ratings:** Average_Rating, Sum_of_Rating
- **Cost:** Avg_Cost_For_Two (Local), **USD** conversion (calculated field)
- **Operations:** Delivering_Now, Has_Online_Delivery, Day_Opening (avg)
- **Time:** Year (2010–2018)

### Modeling & Measures (DAX Highlights)
- `Avg Rating = AVERAGE(Reviews[Rating])`
- `Total Restaurants = DISTINCTCOUNT(Restaurants[RestaurantID])`
- `Count of Cuisines = DISTINCTCOUNT(Restaurants[Cuisines])`
- `Avg Cost (USD) = SUMX(Values(Restaurants[RestaurantID]), Restaurants[Avg_Cost_For_Two] * [FX Rate])`
- `Sum of Ratings = SUM(Reviews[Rating])`

### Usage
- **Filters:** Country, Restaurant, Year, Cuisine
- **Typical Analyses:** Top cuisines by rating, premium restaurants by cost, city-wise distribution, adoption of delivery/online ordering, and year-over-year trends.

---

## 🔗 Quick Navigation
- 🖼️ *[Dashboard Screenshot](https://github.com/mdsamreen414/Power-BI/tree/main/Zomato%20Analytics/Screenshots.md)*
- 📂 *[README.MD](https://github.com/mdsamreen414/Power-BI/blob/main/Zomato%20Analytics/README.md)*

---
🧕**About Me**  
📍 Hyderabad, India  
I'm **Md Samreen**, a certified **Data Analyst** with expertise in [**Excel**](https://github.com/mdsamreen414/Excel), [**Power BI**](https://github.com/mdsamreen414/Power-BI), [**MYSQL**](https://github.com/mdsamreen414/MYSQL), and [**Tableau**](https://github.com/mdsamreen414/Tableau). I specialize in turning raw datasets into insightful and interactive dashboards that empower data-driven decisions.  

**Technical Skills**  
Proficient in advanced Excel functions, data cleaning and transformation, SQL queries, and KPI reporting. Skilled in designing dynamic visualizations using Power BI and Tableau, along with database management in MySQL.  

**Soft Skills**  
Strong in problem-solving, analytical thinking, and attention to detail. Adaptable, collaborative, and effective in communicating insights to both technical and non-technical audiences.  

**Portfolio**  
📌 Visit my portfolio:[**Portfolio Website**](https://your-portfolio-link.com)  

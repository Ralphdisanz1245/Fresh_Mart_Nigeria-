# Fresh_Mart_Nigeria
# 🛒 FreshMart Nigeria PLC: Cost & Profitability Analysis

A Power BI analytics project that examines **where FreshMart's money goes (costs)** and **where its profit comes from** across stores, products, regions and customer segments, from **January 2024 to December 2025**.

The repository contains an interactive two-page Power BI dashboard and a plain-language management report with findings and recommendations.

---

## 🖼️ Dashboard Screenshots

### Cost Dashboard
![Cost Dashboard](Screenshot%202026-11-09%20121850.png)

### Profitability Dashboard
![Profitability Dashboard](Screenshot%202026-11-09%20121959.png)


## 📁 Repository Contents

| File | Description |
| --- | --- |
| `Task7_assignment.pbix` | Power BI report with the **Cost Analysis** and **Profitability Analysis** dashboards |
| `FreshMart_Management_Report.docx` | Management report summarising the findings, key insights, recommendations and next steps |
| `README.md` | Project overview (this file) |

---

## 📊 Dataset at a Glance

| Item | Value |
| --- | --- |
| Period | Jan 2024 – Dec 2025 |
| Sales transactions | 5,000 |
| Stores | 4 (Abuja, Kano, Lagos, Rivers) |
| Products | 20 across 3 categories (Electronics, Groceries, Beauty) |
| Customers | 200 |
| Customer regions | South West, North West, North Central, South South |

> The data does not state a currency, so amounts are shown in the model's own units (M = million, K = thousand).

---

## 🧩 Data Model

The Power BI model follows a star schema:

- **Fact_Sales**: transaction-level sales (with date hierarchy)
- **Dim_Stores**: store
- **Dim_Products**: product and category
- **Dim_Customers**: gender, state, region, age segment and membership tier

### DAX measures used

`Total Sales` · `Total Cost` · `Total Profit` · `Profit Margin` · `Average Order Value` · `Average Cost` · `Cost Per Customer` · `Cost To Revenue Ratio`

---

## 🖥️ Dashboards

### 1. Cost Dashboard Analysis
- KPI cards: Total Cost, Average Cost, Cost Per Customer, Cost-to-Revenue Ratio
- Charts: Cost by Store, Cost by Category, Cost by Region, Cost by Product, Cost by Year and Month
- Slicers: Category, Gender, State, Age Segment, Membership

### 2. Profitability Dashboard Analysis
- KPI cards: Total Sales, Total Cost, Total Profit, Profit Margin, Average Order Value
- Charts: Profit by Store, Profit by Product, Profit by State, Profit by Gender, Profit by Year and Month
- Slicers: Age Segment, Region, Membership, Category

> **Note:** The saved Profitability dashboard has a filter that hides 2025, so it currently shows 2024 only. Remove the filter to see both years.

---

## 🔑 Key Findings

| Measure | 2024 | 2025 | Change |
| --- | --- | --- | --- |
| Sales (revenue) | 322.7M | 338.0M | +4.7% |
| Cost of goods | 261.1M | 273.7M | +4.8% |
| Profit | 61.7M | 64.3M | +4.3% |
| Profit margin | 19.1% | 19.0% | Flat |
| Number of sales | 2,471 | 2,529 | +2.3% |

**Two-year totals:** Sales 660.7M · Cost 534.8M · Profit 126.0M (about 19% margin).

### Highlights

1. **Growth is steady but modest.** Sales, cost and profit all grew about 4–5%, so the 19% margin has not improved.
2. **Stores perform almost the same.** Costs and profit differ by only about 4% between the best and worst store (Kano leads).
3. **Electronics is half the business.** It accounts for 52% of cost and 52% of profit, so results and risk are concentrated.
4. **A few products drive cost.** The top 4 products make up 37% of cost and the top 8 make up 61%.
5. **South West and North West dominate.** Together they account for 56% of cost and 56% of profit.
6. **Growth is uneven.** North West grew +17%, while North Central (−0.9%), South South (−1.4%) and Abuja (−2.9%) declined.
7. **Discounts are the biggest avoidable loss.** Every product is priced 30% above cost (a 23.1% margin), but discounting brings the margin down to 19%.

### The discount effect

| Discount | Share of sales | Margin | Profit | Units per sale |
| --- | --- | --- | --- | --- |
| None | 35% | 23.1% | 54.3M | 4.43 |
| 5% off | 32% | 19.0% | 41.7M | 4.49 |
| 10% off | 33% | 14.5% | 30.0M | 4.44 |

Discounts cost roughly **34.5M** over two years, about a quarter of the profit earned, and customers who get a discount buy no more than those who do not.

---

## ✅ Recommendations

1. **Tighten the discount policy (top priority).** Cap discounts at 5%, or limit them to bulk buys, loyalty members or slow stock. Each 1 point of margin recovered is worth about 3.3M profit per year.
2. **Negotiate with suppliers** on Rice 1, Lotion 5, Laptop 3 and Laptop 5. A 2% saving is worth about 2M per year.
3. **Replicate what works** in North West and Groceries, and investigate Abuja, North Central and South South.
4. **Protect Older Adults** (the profit base) and **target Youth and Silver-to-Gold upgrades**, since these customers earn the most per person.
5. **Set a cost target** of 79–80% of sales and track it monthly.

### Suggested timeline

| When | Action |
| --- | --- |
| Next 30 days | Agree a new discount rule; start supplier talks on the top four products |
| Next 60 days | Review the decline in Abuja, North Central and South South; pilot the new discount rule in one store |
| Next 90 days | Roll out the discount rule everywhere; launch Youth and Gold campaigns; report first monthly cost-to-sales results |

---

## 🚀 How to Use

1. Clone or download this repository:
   ```bash
   git clone https://github.com/Ralphdisanz1245/Fresh_Mart_Nigeria-.git
   ```
2. Open `Task7_assignment.pbix` in **Power BI Desktop** (Windows).
3. Use the slicers to filter by category, gender, state, region, age segment and membership.
4. Read `FreshMart_Management_Report.docx` for the full written analysis.

---

## 📝 Notes on the Data

- **Region** means the customer's region, not the store's.
- Results are very even (for example, one fixed markup on every item), so small differences between stores or categories should not be over-read. The discount and regional growth patterns are the clearest signals.

---

## 🛠️ Tools

- Microsoft Power BI Desktop (DAX, data modelling, visualisation)
- Microsoft Word (management reporting)

---

## 👤 Author

**Ralph** · [GitHub: Ralphdisanz1245](https://github.com/Ralphdisanz1245)

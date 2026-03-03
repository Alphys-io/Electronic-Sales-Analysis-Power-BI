# 📊 Electronic Sales & Profit Analysis – Power BI Dashboard

> A business intelligence dashboard built in Power BI to analyze sales performance, profitability, and trends across product categories, months, and quarters.

---

## 🗂️ Dashboard Overview 
  <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/bee60354-b06b-4d61-8d4c-dde5e035b3b5" />
<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/e047ed23-7e17-4849-9ca9-b62dbb35c22e" />
<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/ff898b9f-0534-4f0e-bff7-9a8b42e76260" />

 
| Page | Description |
|------|-------------|
| **Sales Analysis** | KPI cards, Total Sales by Product Category (donut chart), and a detailed product-level sales table |
| **Profit Analysis** | Profit by Product Category (bar chart), Profit by Month (horizontal bar), and Profit by Quarter (horizontal bar) |
| **Promotion Analysis** | Total Sales & Profit by Promotion type (combo chart), and a ranked product-level promotion table |

---

## 📌 Key Business Insights

### 💰 Overall Performance
- **Total Sales:** 56.25M
- **Profit:** 54.39M
- **Profit Margin:** 96.68%
- **Sales Last Month:** 56.09M

> The business maintains a near-perfect profit margin, indicating very low cost of goods relative to revenue.

---

### 🏆 Top Product Categories by Sales
| Category | Sales |
|----------|-------|
| Computers | 21.63M |
| Cameras & Camcorders | 17.33M |
| TV and Video | 9.26M |
| Cell Phones | 5.92M |
| Music, Movies & Audio Books | 1.07M |

> **Computers** alone account for ~38% of total sales, making it the most critical category to monitor and invest in.

---

### 📅 Seasonal Trends
- **Best months:** October & November (5.3M profit each) — driven by holiday demand
- **Best quarter:** Q4, followed by Q2
- **Weakest months:** January & December (4.1M each)

> Inventory, marketing campaigns, and staffing should be scaled up going into Q4 to capitalize on peak demand.

---

### 🎯 Promotion Performance
| Promotion Type | Total Sales |
|---------------|-------------|
| No Discount | 18.3M |
| Adventist Promotion | 8.6M |
| Winners Promotion | 6.7M |
| Deeper Promotion | 6.4M |
| Xmas Holiday Promotion | 3.7M |

> **No Discount** accounts for the largest share of revenue (~41%), proving that premium products sell well at full price. The Xmas Holiday Promotion underperformed compared to all other campaigns and should be reviewed for ROI.

**Total across all promotions:** Sales = 56,254,053.53 | Profit = 54,387,676.54

---

### 🛍️ Top Products by Sales
| Product | Sub Category / Promotion | Total Sales | Profit |
|---------|--------------------------|-------------|--------|
| Kekule Projector 1080p X980 White | No Discount | 183,600 | 181,670 |
| Proseware Projector 1080p LCD86 Black | No Discount | 160,650 | 158,042 |
| Proseware Projector 1080p LCD86 White | No Discount | 160,650 | 158,817 |
| Fabrikam Trendsetter 2/3" 3mm X300 White | No Discount | 139,860 | 136,903 |
| Kekule Projector 1080p X980 Black | Deeper Promotion | 123,930 | 119,684 |

---

### Findings
**Overall Business Performance**
The business is performing strongly with total sales of 56.25 million and a profit of 
54.39 million, giving an impressive profit margin of nearly 97%. Cumulative sales came 
in at 16 million, which is very close to the overall total, suggesting consistent and stable 
revenue.

**What's Selling the Most?**
Looking at the donut chart on the Sales Analysis page, Computers dominate product 
sales at 21.63M, followed by Cameras and Camcorders at 17.33M, then TV and Video at 
9.26M. Cell phones and Music/Movies/Audio Books contribute much smaller shares. 
This tells us the business is heavily dependent on computer and camera products —
which is both an opportunity and a risk.

**Top Performing Products**
The table shows that Projectors & Screens consistently appear as top revenue 
generators. The single best-selling product was the Proseware Projector 1080p LCD86 
White at 110,160 in sales, mostly in Q4 2011. Camcorders like the Fabrikam 
Independent Filmmaker also performed well, reaching over 101,000 in a single period.

**Profit Breakdown (Profit Analysis Page)**
Computers generate the highest profit at 20.9M, almost double that of Cameras and 
Camcorders at 16.8M. TV and Video contributes 8.9M, while Cell Phones and Audio 
bring in much smaller margins around 1M each. This confirms that the company's 
profitability is heavily anchored in the computer category.

**When Is the Business Most Profitable?**
Looking at profit by month, October and November are the strongest months, each at 
5.3M, likely driven by holiday season demand. April and May follow at 4.8M each. 
January and December are the weakest months at 4.1M each. By quarter, Q4 is the 
clear winner, followed closely by Q2, then Q3, with Q1 being the slowest — reinforcing 
the seasonal pattern.

**Promotion Analysis**
**How Promotions Affect Sales**
This third page reveals something very important: the majority of the business's revenue 
actually comes from products sold at No Discount (18.3M), which is by far the largest 
bar on the chart. This means customers are willing to pay full price — a very healthy sign 
for the brand's perceived value.
After that, the Adventist Promotion generated 8.6M, Winners Promotion 6.7M, Deeper 
Promotion 6.4M, and the Xmas Holiday Promotion the least at 3.7M. Interestingly, the 
Christmas promotion underperformed compared to other promotional campaigns, 
which may warrant a review of that strategy.

**Top Products and Their Promotions**
The table confirms that the best-selling products — particularly Kekule and Proseware 
Projectors — largely sold under No Discount, reinforcing that premium products don't 
need heavy discounting to move. The top single product, the Kekule Projector 1080p 
X980 White, generated 183,600 in sales with a profit of 181,670 — an almost perfect 
margin on that item alone.

**Key Takeaway**
Discounts are not the primary sales driver here. The business should be cautious about 
over-relying on promotions since the no-discount segment dominates. The Xmas 
Holiday Promotion in particular should be evaluated for ROI — it generated the least 
revenue of all promotional types. The business is healthy and highly profitable. Focus 
should remain on computers and cameras as they drive most revenue and profit. Q4 is 
the golden quarter — inventory, marketing, and staffing should be prioritized heading 
into October/November.
****

## 🧮 DAX Measures

All key metrics in this report are powered by the following DAX calculations:

```dax
-- 1. Total Sales
Total Sales = SUM(Sales[Sales])

-- 2. Total Cost
Total Cost = SUM(Sales[Total Cost])

-- 3. Profit
Profit = [Total Sales] - [Total Cost]

-- 4. Profit Margin
Profit Margin = DIVIDE([Profit], [Total Sales])

-- 5. Sales Year-to-Date
Sales YTD = TOTALYTD([Total Sales], 'Date'[Date])

-- 6. Sales Same Period Last Year
Same Period LY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))

-- 7. Year-over-Year Sales Change
Sales YOY = [Total Sales] - [Same Period LY]

-- 8. Year-over-Year Sales Change (%)
Sales YOY % = DIVIDE([Sales YOY], [Same Period LY])

-- 9. Sales Last Month
Sales Last Month = CALCULATE([Total Sales], PARALLELPERIOD('Date'[Date], -1, MONTH))
```

---

## 🔍 Measure Explanations

| Measure | Purpose | Business Use |
|---------|---------|--------------|
| `Total Sales` | Sums all revenue | Baseline KPI for all comparisons |
| `Total Cost` | Sums all costs | Cost monitoring |
| `Profit` | Revenue minus cost | Core profitability metric |
| `Profit Margin` | Profit as % of sales | Efficiency indicator |
| `Sales YTD` | Cumulative sales from start of year | Track annual progress |
| `Same Period LY` | Sales in same time window last year | Year-over-year baseline |
| `Sales YOY` | Difference vs. last year | Growth/decline tracking |
| `Sales YOY %` | % change vs. last year | Normalized growth metric |
| `Sales Last Month` | Sales in the prior month | Month-on-month comparison |

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Data Model:** Sales fact table linked to a Date dimension table

---
## 👤 Analyst

**Gbenovie Obhoo**
📧 Gbenovieobhoo@gmail.com

---




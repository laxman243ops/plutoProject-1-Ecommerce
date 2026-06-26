# 📦 Project 01 — E-Commerce Sales Analysis
**Pluto Academy Data Analytics Internship**

---

## 👤 Intern Details

| Field | Details |
|---|---|
| **Name** | Butcha Laxmana Rao |
| **Program** | Pluto Academy — Data Analytics Internship |
| **Project** | Project 01 — E-Commerce Sales Analysis |
| **Dataset** | Olist Brazilian E-Commerce (Kaggle) |
| **Tools** | Python · Pandas · Matplotlib · Seaborn |

---

## 📊 Dataset

**Source:** [Olist Brazilian E-Commerce — Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Files used:
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_products_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_customers_dataset.csv`
- `product_category_name_translation.csv`

---

## 🧹 Data Cleaning Summary

| Step | Action | Result |
|---|---|---|
| Date columns | Converted 5 columns to datetime | Fixed for trend analysis |
| Order filter | Kept only `delivered` status orders | Removed cancelled/pending |
| Null values | Filled unknown categories with `'Unknown'` | No data loss |
| Table merge | Merged 6 CSVs into one master dataframe | Ready for analysis |
| Duplicates | Removed all duplicate rows | Clean dataset |

---

## 📈 KPI Summary

| KPI | Value |
|---|---|
| 💰 Total Revenue | **R$ 1,829,209.53** |
| 📦 Total Orders | **13,339** |
| 🏆 Top Category | **beleza_saude** (R$ 1,47,980.12) |
| 📅 Peak Month | **April 2018** |
| 🏙️ Best State | **SP — São Paulo** (R$ 19,302.56) |
| ⭐ 5-Star Reviews | **56.4%** |
| 🚨 1-Star Reviews | **13.8%** |

---

## 🔍 Sales Analysis — 5 Questions Answered

**Q1. Which product category has the highest revenue?**
`beleza_saude` (Beauty & Health) — R$ 1,47,980.12, leading all categories by 11%+.
Top 5 categories:
- beleza_saude — R$ 1,47,980.12
- relogios_presentes — R$ 1,32,362.31
- cama_mesa_banho — R$ 1,13,063.84
- esporte_lazer — R$ 1,12,500.21
- informatica_acessorios — R$ 1,10,155.85

**Q2. Which month had peak sales?**
**April 2018** — Revenue ~R$ 17,000. Q2 (Apr–Jun) consistently outperforms all other quarters across both 2017 and 2018.

**Q3. Which region performs best?**
**SP (São Paulo)** — R$ 19,302.56 — nearly 3× more than #2 RJ (R$ 7,080.74). Top 4 states:
- SP: R$ 19,302.56
- RJ: R$ 7,080.74
- SC: R$ 6,531.87
- MG: R$ 4,408.29

**Q4. What is the average order value trend?**
AOV declined from R$ 253.30 (Oct 2016) to R$ 89.41 (Apr 2017) — a 65% drop — then stabilised. This reflects market maturation and price competition as the platform scaled.

**Q5. What is the customer review score distribution?**
- ⭐⭐⭐⭐⭐ 5 stars: 56.4% (1,236 reviews)
- ⭐⭐⭐⭐ 4 stars: 17.7% (388 reviews)
- ⭐ 1 star: 13.8% (302 reviews)
- ⭐⭐⭐ 3 stars: 8.3% (181 reviews)
- ⭐⭐ 2 stars: 3.9% (86 reviews)

---

## 📉 Visualisations

| # | Chart Type | What It Shows |
|---|---|---|
| Chart 1 | Horizontal Bar | Top 10 Categories by Total Revenue |
| Chart 2 | Line + Bar (dual axis) | Monthly Revenue Trend + Order Volume |
| Chart 3 | Horizontal Bar | Top 10 States by Revenue (Regional) |
| Chart 4 | Histogram | Distribution of Order Values |
| Chart 5 | Pie Chart | Customer Review Score Breakdown |
| Chart 6 | Heatmap | Revenue per Category per Month |
| Dashboard | KPI Cards | 6 Key Business Metrics |

All charts include titles, axis labels, and legends.

---

## 💡 Business Insights Report

**Insight 1 — Beauty & Health is the Undisputed Revenue Leader (Chart 1)**
`beleza_saude` generated R$ 1,47,980.12 — 11% more than #2. The heatmap (Chart 6) confirms this category has consistent monthly sales, not just seasonal spikes. It is the single most reliable revenue driver on the platform.
**Recommendation:** Increase inventory depth and allocate 20-25% more marketing budget to beauty products year-round. Introduce a loyalty rewards program for repeat buyers in this category to reduce churn.

**Insight 2 — Revenue Grew 17× in 2 Years but Q2 Spikes Need to Be Planned For (Chart 2)**
Total monthly revenue grew from R$ 1,000 (Oct 2016) to R$ 17,000 (Apr 2018) — a 17× increase. April 2018 was the single strongest month. The zigzag pattern suggests bi-weekly buying cycles.
**Recommendation:** Launch targeted discount campaigns in February and March to pre-load Q2 demand. Ensure logistics and stock are ramped up before April to avoid supply shortfalls at peak.

**Insight 3 — São Paulo Concentration is a Business Risk (Chart 3)**
SP alone generated R$ 19,302 — nearly 3× more than RJ (R$ 7,080) and almost the combined revenue of states ranked 5th–10th. This overdependence is a single-point-of-failure risk.
**Recommendation:** Allocate dedicated campaign budgets for CE, PB, SE, PR, RS, and BA — states with clear growth potential but low current penetration. Target 10% regional diversification in 12 months.

**Insight 4 — 1-Star Reviews Are the Second Most Common Rating (Chart 5)**
Despite 56.4% five-star ratings, 1-star (13.8%) is the second most frequent single rating — more than 3-star and 2-star combined. This polarisation signals product/delivery issues in specific categories.
**Recommendation:** Cross-reference 1-star reviews with categories and delivery time data. Identify which categories generate the most complaints and address root causes — whether product quality, seller standards, or last-mile delivery speed.

**Insight 5 — Most Orders Are Under R$ 300 and AOV is Declining (Chart 4)**
The order value histogram shows an extreme right-skew — the vast majority of orders are below R$ 300. Combined with AOV dropping from R$ 253 (Oct 2016) to R$ 89 (Apr 2017), this shows customers are trending toward smaller, lower-value purchases.
**Recommendation:** Introduce bundle offers and a minimum-spend incentive (e.g. "Spend R$ 300 and get free shipping") to reverse AOV decline. Create curated product combos in the top 3 categories to encourage higher basket sizes.

---

## 🔍 Most Surprising Finding

The most unexpected result was that `fashion_roupa_masculina` (men's clothing) and `papelaria` (stationery) show extreme isolated revenue spikes in the heatmap — dark blue in just one or two months — then essentially disappear. These appear to be viral or event-driven demand moments rather than organic growth. The broader surprise is that despite these dramatic spikes, neither category appears in the top 10 by total annual revenue. Steady, consistent performers like `beleza_saude` generate far more total value than one-time viral moments.

---

## 🚀 How to Run

```bash
pip install pandas matplotlib seaborn numpy
python project01_ecommerce.py
```

Place all Olist CSV files in the same directory before running.

---

## 📁 Output Files Generated

```
project01_outputs/
├── chart1_revenue_by_category.png
├── chart2_monthly_trend.png
├── chart3_regional_sales.png
├── chart4_order_value_histogram.png
├── chart5_review_scores_pie.png
├── chart6_category_month_heatmap.png
└── dashboard_kpi.png
```
<img width="1417" height="748" alt="image" src="https://github.com/user-attachments/assets/f8cddc28-0caa-4f51-8279-e2e583357d61" />


---

*Pluto Academy Data Analytics Internship 2026 · plutoacademy.in*

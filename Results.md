E-Commerce Sales Analytics Dashboard
Analysis Report  |  Python, SQL, Tableau  |  Butcha Laxmana Rao
1. Overview
This project analyzes e-commerce sales data to understand which products, regions and time periods drive revenue, and how customers rate their orders. Data was cleaned and transformed with a Python and SQL pipeline, validated with SQL queries, and visualized in an interactive dashboard.
Dataset: [dataset name, e.g. Brazilian e-commerce (Olist)]
Data size: [number of records after cleaning]     Currency: [confirm: $ or R$]
2. Headline Metrics
Total Revenue
1,829,209.53	Total Orders
13,339	Top Category
beleza_saude	Peak Sales Month
2018-04

3. Key Findings
Top 5 product categories by revenue
Rank	Category	Revenue
1	beleza_saude (health & beauty)	147,980.12
2	relogios_presentes (watches & gifts)	132,362.31
3	cama_mesa_banho (bed, bath & table)	113,063.84
4	esporte_lazer (sports & leisure)	112,500.21
5	informatica_acessorios (computer accessories)	110,155.85

Top 5 regions (customer state)
Rank	State	Sales
1	SP	19,302.56
2	RJ	7,080.74
3	SC	6,531.87
4	MG	4,408.29
5	CE	1,825.79

Average order value and review distribution
Month	Avg. order value
2016-10	253.30
2017-01	148.32
2017-02	110.26
2017-03	104.86
2017-04	89.41

Review score	Count	Share
5 stars	1,236	56.4%
4 stars	388	17.7%
3 stars	181	8.3%
2 stars	86	3.9%
1 star	302	13.8%

4. Insights
•	Revenue is spread across categories: health & beauty leads, with the top five categories contributing about 616K, roughly one third of total revenue.
•	Sales grew over time: monthly sales rose from late 2016 and reached their peak in April 2018, with seasonal ups and downs along the way.
•	Strong regional concentration: São Paulo (SP) leads by a wide margin, about 2.7 times the next state (RJ), so other regions are a growth opportunity.
•	Average order value fell in early 2017: from about 253 in October 2016 to about 89 in April 2017. The October 2016 figure is based on very few orders, so the early drop should be read with care.
•	Most orders are small: the order value distribution is heavily right-skewed, with most orders low in value and a few very large ones.
•	Customer satisfaction is high: about 74% of reviews are 4 or 5 stars, while 17.7% are 1 or 2 stars, which points to delivery or product issues worth investigating.
5. Dashboard
 
Figure 1: Dashboard with revenue by category, monthly trend, regional sales, order value distribution, review scores and category vs month heatmap.
<img width="1000" height="523" alt="image" src="https://github.com/user-attachments/assets/4dd5023f-b79d-497a-8bd7-0f28e38395cd" />

6. Recommendations
•	Prioritize inventory and marketing for the top categories, especially health & beauty and watches & gifts.
•	Run targeted campaigns in states outside SP to reduce dependence on a single region.
•	Analyze the 1-2 star reviews to find the main causes of dissatisfaction, such as delivery delays or product quality.
•	Prepare for peak months by planning stock and promotions ahead of the spring season.

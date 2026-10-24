# Store Profitability, Revenue & Customer Loyalty Analysis | Power BI

## 📊 Project Overview

This project explores store-level profitability, revenue performance, regional differences, store-format performance, and customer loyalty using **Microsoft Power BI**.

The objective was to transform retail business data into interactive dashboards that help stakeholders understand financial performance, identify potential profitability risks, compare store formats, and evaluate the contribution of customer loyalty to revenue.

The project consists of two analytical dashboards:

1. **Profitability & Store Performance Dashboard** — examines gross profit, loyalty adoption, daily performance, monthly net profit trends, revenue composition, and product-category gross margins.
2. **Sales & Revenue Performance Dashboard** — examines revenue and profit KPIs, regional profitability, rent versus revenue, loyalty revenue contribution, and loyalty redemption costs.

## 🎯 Business Problem

Retail businesses operate across different regions and store formats, each with different revenue opportunities, operating costs, and profitability outcomes.

Total revenue alone does not provide a complete picture of business performance. A store may generate substantial revenue while also incurring high operating costs. Similarly, strong loyalty participation does not automatically translate into greater profitability if loyalty programme costs are too high.

This project investigates:

- How revenue, rent, and profitability relate to one another.
- Which regions and store formats demonstrate stronger financial performance.
- How profitability changes over time.
- Which product categories generate stronger gross margins.
- How loyalty participation and member revenue contribute to overall performance.
- Whether loyalty redemption costs require further investigation.
- How weekday and weekend performance differs across store formats.

## 🎯 Project Objectives

1. Evaluate revenue, gross profit, net profit, and net profit margin.
2. Monitor monthly profitability trends and compare performance between years.
3. Compare store performance across regions and store formats.
4. Investigate the relationship between rent and revenue at store level.
5. Analyse weekday versus weekend revenue patterns.
6. Compare gross margins across product categories.
7. Evaluate loyalty adoption and loyalty member revenue contribution.
8. Examine loyalty redemption costs across regions.
9. Identify potential performance gaps and opportunities for improvement.
10. Present findings through interactive Power BI dashboards.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard development and visual analytics |
| Power Query | Data preparation and transformation |
| DAX | KPI calculations and analytical measures |
| Data Modelling | Organising fact and dimension tables |
| GitHub | Project documentation and portfolio presentation |

## 📁 Dataset Overview

The analysis uses retail store profitability, revenue, and loyalty-related data.

Key fields used or identified in the project include:

| Field | Analytical Purpose |
|---|---|
| `store_name` | Identifies individual stores |
| `store_format` | Compares High-Street and Transport-Hub stores |
| `region` | Enables regional comparisons |
| `rent_gbp` | Represents store rental costs |
| `total_monthly_revenue_gbp` | Supports monthly revenue analysis |
| `profitability_status` | Classifies store profitability |
| `loyalty_member_revenue_pct` | Measures recorded loyalty member revenue contribution |
| `loyalty_redemption_cost_gbp` | Supports loyalty redemption cost analysis |
| `gross_margin_pct` | Enables product-category margin comparisons |
| `month_name` and `Year` | Support monthly and yearly analysis |
| `Day Type` | Separates weekday and weekend performance |

*Document only the fields present in the actual dataset. Explain any renamed or calculated columns.*

## 🔄 Project Workflow

### Step 1: Understand the Business Requirements

I identified the business questions the dashboards needed to answer, focusing on financial performance, store operations, regional comparisons, and customer loyalty.

This established a clear connection between the dataset, analytical questions, and final dashboard design.

### Step 2: Data Preparation and Transformation

I prepared the data using Power Query and the Power BI data model.

The preparation process focused on:

- Reviewing column names and data types.
- Checking numerical and categorical fields.
- Preparing time-related fields for monthly and yearly analysis.
- Organising revenue, profitability, store, and loyalty attributes.
- Creating a Day Type classification for weekdays and weekends.
- Preparing revenue categories for category-level comparisons.
- Reviewing missing values, duplicates, and inconsistencies where applicable.

### Step 3: Data Modelling

The project uses store-level financial data alongside time-related and daily sales information.

The model supports analysis by month, year, store, region, store format, and product category.

Relationships between fact and dimension tables must be configured correctly to ensure that report filters affect the intended measures.

### Step 4: KPI Development

The dashboards include the following performance indicators:

- Total Revenue
- Gross Profit
- Net Profit
- Net Profit Margin
- Loyalty Revenue Contribution
- Loyalty Adoption Rate
- Average Daily Gross Profit
- Average Daily Footfall
- Average Transaction Value
- Revenue per Square Foot

Each KPI should have a documented formula, unit, and aggregation method.

### Step 5: Dashboard Design

The report was organised into two dashboards to separate complementary analytical themes.

The first dashboard focuses on store profitability and operational performance. The second focuses on revenue, profit, regional comparisons, rent, and loyalty-related analysis.

Both dashboards provide filters for year, region, quarter, and store.

The purple colour palette and consistent KPI cards create a unified visual identity across the report.

---

# 📈 Dashboard 1: Profitability & Store Performance

## Dashboard Overview

This dashboard focuses on the financial and operational performance of retail stores.

It combines KPI cards with monthly trend analysis, revenue composition, day-type comparisons, and product-category gross margin analysis.

## Key Performance Indicators

### 1. Gross Profit

Measures the gross profit generated under the project's defined calculation.

**Business value:** Helps stakeholders understand the amount remaining after the costs included in the gross profit calculation.

### 2. Loyalty Adoption Rate

Tracks the project's loyalty adoption metric.

**Business value:** Provides an indication of customer participation in the loyalty programme.

The formula and denominator should be documented to establish whether this measures customer adoption, transaction participation, or another metric.

### 3. Average Daily Gross Profit

Summarises gross profit on an average daily basis.

**Business value:** Helps stakeholders assess daily profitability rather than relying only on total-period results.

### 4. Average Daily Footfall

Represents the recorded average daily footfall measure.

**Business value:** Supports analysis of customer traffic and its potential relationship with financial performance.

### 5. Average Transaction Value

Measures average transaction value according to the project's calculation.

**Business value:** Helps stakeholders investigate whether revenue growth may be associated with higher spending per transaction.

## Visual Analysis

### A. Monthly Net Profit Trend by Year

**Visual:** Line chart comparing monthly net profit across two years.

**Business question:** How does net profit change throughout the year, and how does monthly performance compare between years?

**Analytical value:**

- Highlights monthly increases and decreases in net profit.
- Identifies comparatively strong or weak months.
- Supports year-over-year comparisons.
- Helps investigate seasonality and unusual changes.

**Business application:** Management can investigate the factors behind weaker months and determine whether stronger months follow a repeatable pattern.

### B. Retail Beans Revenue Contribution by Month and Year

**Visual:** Stacked column chart comparing the displayed Retail Beans Revenue percentage across months and years.

**Business question:** How does the recorded Retail Beans revenue contribution vary across the reporting period?

**Analytical value:**

- Provides a monthly view of the category measure.
- Allows comparison between reporting years.
- Supports investigation of changes in product-category contribution.

**Business application:** Product managers can investigate category performance and determine whether further merchandising or sales analysis is needed.

### C. Total Revenue by Revenue Category

**Visual:** Doughnut chart showing Espresso, Filter, Food, and Retail Beans revenue categories.

**Business question:** How is total revenue distributed across the selected revenue categories?

**Analytical value:**

- Provides a category-level view of revenue composition.
- Supports product mix analysis.
- Helps identify categories contributing to overall sales.

**Business application:** Management can use category contribution to guide further investigation into product demand, pricing, and merchandising.

**Validation note:** Confirm that each doughnut segment uses the correct category-specific revenue measure. If every category displays the same value, investigate the data structure and aggregation before interpreting the chart.

### D. Total Revenue by Day Type and Store Format

**Visual:** Clustered column chart comparing weekday and weekend revenue for High-Street and Transport-Hub stores.

**Business question:** How does revenue differ between weekdays and weekends across store formats?

**Analytical value:**

- Compares weekday and weekend performance.
- Highlights differences between store formats.
- Helps investigate whether particular formats perform better on specific days.

**Business application:** Findings may inform staffing, stock planning, promotional timing, and opening-hour decisions.

For a fair comparison, distinguish total revenue from average daily revenue. If the objective is to understand typical daily performance, compare average revenue per weekday with average revenue per weekend day.

### E. Average Gross Margin Percentage by Product Category

**Visual:** Horizontal bar chart comparing gross margin percentage across product categories.

**Business question:** Which product categories have the highest recorded gross margins?

**Analytical value:**

- Makes category margin differences easy to compare.
- Highlights categories requiring further investigation.
- Complements revenue analysis with a profitability-related measure.

**Business application:** Management can investigate pricing, supplier costs, discounts, and product mix.

A high gross margin percentage does not necessarily mean a category generates the highest total gross profit. Both margin percentage and revenue contribution should be considered.

---

# 💰 Dashboard 2: Sales & Revenue Performance

## Dashboard Overview

The second dashboard provides a broader view of sales, financial performance, regional differences, store-level rent and revenue, and loyalty-related metrics.

Its purpose is to help stakeholders assess financial outcomes and identify areas where store performance, cost structure, or customer loyalty may require closer investigation.

## Key Performance Indicators

### 1. Total Revenue

Summarises revenue for the selected reporting period.

**Business value:** Establishes the overall sales performance baseline.

### 2. Net Profit

Measures net profit according to the project's defined financial calculation.

**Business value:** Helps assess the financial outcome after the costs included in the calculation.

### 3. Net Profit Margin

Measures net profit relative to revenue.

**Business value:** Helps stakeholders understand how much net profit is generated per unit of revenue.

The percentage presentation should be consistent throughout the report.

### 4. Loyalty Revenue Percentage

Displays the recorded loyalty revenue contribution measure.

**Business value:** Helps evaluate the role of loyalty-related revenue within overall sales performance.

Verify whether the calculation represents a ratio, percentage, or average of store-level percentages.

### 5. Revenue per Square Foot

Measures revenue relative to the recorded store area.

**Business value:** Supports comparisons of sales productivity across stores with different physical sizes.

Verify the units and store-area denominator before using this measure for store rankings.

## Visual Analysis

### A. Average Net Profit Margin by Region and Store Format

**Visual:** Column chart comparing average net profit margin across regions and store formats.

**Business question:** How does net profit margin differ across regions and store formats?

**Analytical value:**

- Provides a regional comparison of the displayed profitability measure.
- Helps investigate differences between High-Street and Transport-Hub stores.
- Supports the identification of locations or formats requiring additional financial analysis.

**Business application:** Management can investigate whether differences are associated with rent, sales volume, operating costs, store size, or other factors.

**Validation note:** Confirm the intended aggregation. An unweighted average of store-level margins can differ from overall net profit divided by overall revenue.

### B. Loyalty Redemption Costs by Region

**Visual:** Column chart displaying loyalty redemption costs across regions.

**Business question:** Which regions incur the highest loyalty redemption costs?

**Analytical value:**

- Supports comparisons of recorded redemption costs.
- Helps identify regional differences for further investigation.
- Provides context for evaluating loyalty programme costs.

**Business application:** Stakeholders can investigate redemption activity, programme participation, and the financial return associated with loyalty-related spending.

**Validation note:** The displayed regional values appear identical in the screenshot. Verify that the regional filter affects the measure and that the underlying data supports the comparison.

### C. Total Rent and Total Revenue by Store

**Visual:** Scatter chart comparing rent and revenue at store level.

**Business question:** How does rent relate to revenue across individual stores?

**Analytical value:**

- Explores the relationship between store rent and revenue.
- Highlights stores with comparatively high rent and low revenue.
- Helps identify stores that may require a more detailed cost and profitability review.

**Business application:** Management can investigate lease costs, sales productivity, location, format, and operating performance.

A scatter chart can reveal an association, but it does not establish that rent causes a particular revenue outcome.

### D. Average Loyalty Member Revenue Percentage by Store Format

**Visual:** Column chart comparing the displayed loyalty member revenue percentage between High-Street and Transport-Hub stores.

**Business question:** Which store format has the higher recorded loyalty member revenue contribution?

**Analytical value:**

- Compares the displayed loyalty metric between store formats.
- Supports investigation of differences in loyalty-related revenue.
- Allows comparisons with other financial and operational measures.

**Business application:** The business can investigate whether loyalty performance differs by format and whether observed differences correspond with transaction behaviour, customer mix, or programme engagement.

**Validation note:** If the field represents store-level percentages, confirm whether an average is appropriate. A transaction-weighted or revenue-weighted calculation may answer a different business question.

### E. Store-Level Financial Performance Table

**Visual:** Table displaying region, store name, store format, profitability status, total revenue, and net profit-related fields.

**Business question:** How do individual stores compare in terms of financial performance and profitability status?

**Analytical value:**

- Provides store-level detail behind summary charts.
- Supports investigation of individual stores within specific regions.
- Allows users to examine profitability classifications alongside financial measures.

**Business application:** Managers can investigate stores that may require operational review.

**Validation note:** The screenshot shows the same total revenue value repeated across multiple store rows. Check whether the measure responds to the individual store filter and whether store-level revenue is being displayed correctly.

---

# 🔍 Key Findings & Business Interpretation

The dashboards establish several useful analytical directions. These observations describe what the visuals are designed to investigate; they should not be treated as confirmed business findings until the underlying measures and data have been validated.

## 1. Monthly Profitability Patterns

The monthly net profit chart allows performance comparisons across months and years.

**Potential business action:** Investigate monthly fluctuations, including sales changes, operating costs, seasonality, and store-level performance.

## 2. Store Format Performance

Comparisons between High-Street and Transport-Hub stores support investigation of differences in revenue, margin, and loyalty-related measures.

**Potential business action:** Assess whether differences persist after accounting for revenue volume, operating costs, and the number of observations in each group.

## 3. Rent and Revenue Relationship

The store-level scatter chart provides a method for exploring the relationship between rental costs and revenue.

**Potential business action:** Prioritise stores for review based on rent relative to revenue and assess overall profitability before recommending lease or operational changes.

## 4. Product Category Margins

The gross margin chart provides a basis for comparing product-category margins.

**Potential business action:** Combine margin percentage with category revenue and gross profit to identify categories that are both commercially important and financially attractive.

## 5. Loyalty Programme Performance

The loyalty-related metrics provide a basis for evaluating member revenue contribution and redemption costs.

**Potential business action:** Compare loyalty-related revenue and redemption costs using consistent periods and appropriate denominators. Where possible, evaluate incremental revenue and programme operating costs before drawing conclusions about programme profitability.

## 6. Data Quality and Measure Validation

The dashboard review highlights the importance of validating how measures respond to regional, store, and category filters.

**Potential business action:** Test measures against the source data, investigate repeated values, and verify that each visual answers the intended business question.

---

# 💡 Business Recommendations

### 1. Review Stores with Potential Rent Pressure

Investigate stores where rental costs appear high relative to revenue and evaluate overall profitability before making lease decisions.

### 2. Monitor Monthly Profitability

Use monthly trends to investigate weaker reporting periods and determine whether corrective action or further analysis is required.

### 3. Evaluate Revenue and Margin Together

Avoid relying on revenue alone when evaluating category or store performance. Combine revenue, gross profit, gross margin, rent, and net profit where available.

### 4. Improve Loyalty Programme Measurement

Use clearly defined adoption and member revenue measures. Compare loyalty-related benefits with redemption costs and other programme expenses.

### 5. Investigate Store Format Differences

Compare High-Street and Transport-Hub stores using consistent metrics and suitable denominators. Consider differences in trading days, store size, customer traffic, and operating costs.

### 6. Strengthen Reporting Reliability

Validate calculations and filter behaviour before distributing dashboards to decision-makers.

---

# 🎨 Dashboard Design & Interactivity

The report uses a consistent visual layout to make financial and operational metrics easier to navigate.

### Design Features

- Purple-themed report header and consistent visual identity.
- KPI cards for high-level performance monitoring.
- Line charts for monthly trends.
- Column charts for category, regional, and store-format comparisons.
- A doughnut chart for revenue composition.
- A scatter chart for store-level rent and revenue analysis.
- A detailed table for investigating individual store performance.
- Interactive Year, Region, Quarter, and Store filters.
- A reset option for returning the report to its default filter state.

### Design Objective

The dashboards support both summary-level monitoring and detailed investigation without requiring users to manually inspect the underlying dataset for every question.

---

# 📌 Project Limitations & Validation Considerations

Before using the report for business decisions, verify the following:

1. **KPI definitions:** Confirm the formula, unit, and aggregation method for every displayed metric.
2. **Store-level revenue:** Verify that revenue measures respond correctly to store-level filters.
3. **Regional redemption costs:** Confirm that the regional chart displays the appropriate cost for each region.
4. **Revenue composition:** Verify that each revenue category uses the correct source field.
5. **Loyalty adoption:** Confirm the numerator and denominator used to calculate adoption.
6. **Margin aggregation:** Distinguish between average store-level margin and overall weighted net profit margin.
7. **Daily performance:** Use comparable daily averages when comparing weekdays with weekends.
8. **Date relationships:** Verify that year, quarter, and month filters operate correctly across relevant tables.
9. **Financial definitions:** Ensure gross profit, net profit, rent, and loyalty costs are defined consistently with the source data.

These checks help ensure that the report provides accurate, interpretable, and decision-ready information.

---

# 🚀 Skills Demonstrated

- Business problem definition and analytical question development.
- Data preparation and transformation using Power Query.
- KPI development and analytical calculations using DAX.
- Power BI data modelling and filter behaviour.
- Financial and operational performance analysis.
- Trend analysis and year-over-year comparison.
- Store, regional, and product-category analysis.
- Loyalty-related metric analysis.
- Interactive dashboard design and data storytelling.
- Business interpretation and recommendation development.
- Project documentation and portfolio presentation using GitHub.

---

# 📂 Repository Structure

```text
powerbi-store-profitability-loyalty-analysis/
│
├── README.md
│
├── dashboards/
│   ├── profitability-store-performance.png
│   └── sales-revenue-performance.png
│
├── powerbi/
│   └── store-profitability-loyalty-analysis.pbix
│
├── data/
│   └── README.md
│
└── documentation/
    ├── business-questions.md
    ├── kpi-definitions.md
    └── findings-and-recommendations.md
```

*This is a suggested folder structure. Include only files that actually exist in your repository. If the dataset cannot be shared, document its structure and omit the original data files.*

## 📸 Dashboard Preview

### Dashboard 1 — Profitability & Store Performance
<img width="1344" height="753" alt="Screenshot 2026-10-11 154300" src="https://github.com/user-attachments/assets/67096b50-7943-4cd1-a05c-7428bf48c85a" />




This dashboard provides a view of gross profit, loyalty adoption, daily performance, monthly net profit trends, revenue composition, weekday versus weekend revenue, and product-category gross margins.

### Dashboard 2 — Sales & Revenue Performance
<img width="1342" height="763" alt="Screenshot 2026-10-11 154352" src="https://github.com/user-attachments/assets/6b20f470-f223-448e-a0d7-83943c260754" />


This dashboard provides a view of total revenue, net profit, net profit margin, loyalty revenue contribution, revenue per square foot, regional comparisons, rent versus revenue, and store-level financial performance.

---

# 🏁 Conclusion

This project demonstrates how Power BI can transform retail financial and operational data into interactive dashboards that support business analysis.

By bringing together profitability, revenue, store format, regional performance, product-category margins, and loyalty-related measures, the report creates a structured starting point for investigating business performance and identifying opportunities for improvement.

**A useful dashboard must combine clear visual communication with reliable calculations and sound business interpretation.**

The next step is to validate the underlying measures, document the KPI definitions, and confirm that each visual responds correctly to the report filters.

---

## 👤 Konkwo Victor

**Data Analytics & Business Intelligence Portfolio Project**

**Tools:** Microsoft Power BI | Power Query | DAX | GitHub

*This project is presented for analytical learning and portfolio demonstration. Business recommendations should be confirmed against validated source data before implementation.*

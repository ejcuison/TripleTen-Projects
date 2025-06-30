# SuperStore Returns Analysis (Tableau Storytelling Project)

** Link to Tableau: https://public.tableau.com/app/profile/erwin.cuison/viz/Sprint5Project-Tableau/AnalysisonSuperstoreReturns?publish=yes

** Link to Presentation Recording: https://www.loom.com/share/26fbdd8c02c94ebdb9b9a0e9da266f0d?sid=d68dfec2-8b21-4a16-9430-b03087cf4b0a

## Overview

This project is a data storytelling presentation built in Tableau, focused on analyzing product returns using the SuperStore dataset. The goal is to uncover key patterns in return rates across different dimensions and provide actionable recommendations for reducing returns.

## Data Source

**File**: \`Superstore.xls\`  
**Tables**: \`Orders\`, \`People\`, \`Returns\`

## Tools Used

\- Tableau Desktop

## Key Steps

1\. **Data Preparation**  
   \- Left joined \`Returns\` table onto \`Orders\`.  
   \- Created a calculated field: \`Returned\` (1 for "Yes", 0 for null).  
   \- Derived return rate as the average of the \`Returned\` field.

2\. **Visualizations**  
   \- Scatterplot: Correlation between total sales and total returns (by product subcategory).  
   \- Bar Chart: Return rate by product category.  
   \- Customer Filter: Removed customers with only one order.  
   \- Map: Geographic distribution of return rates (by state).  
   \- Time Analysis: Return rate by time (month, week).  
   \- Composite Chart: Return rates across multiple factors (date, geography, category).

3\. **Dashboard Design**  
   \- Documented design requirements.  
   \- Created low-fidelity mockups and dashboard templates.  
   \- Finalized dashboard with images, titles, and markers.

4\. **Storytelling**  
   \- Drafted a story arc with Tableau Story Points.  
   \- Included summary, dashboard overview, root cause analysis using filters, and proposed actions.  
   \- Delivered a 3–5 minute presentation.

## Insights & Recommendations

\- **Return Rate Drivers**: Product subcategory, shipping mode, state, and month.  
\- **Problem Subcategories**: Machines, Fasteners, Chairs, Appliances, Tables.  
\- **Actionable Steps**:  
  \- Investigate or stop selling top 3–5 returned subcategories.  
  \- Reduce marketing focus in Utah, Oregon, and California.  
  \- Eliminate same-day shipping to reduce return likelihood.  
  \- Monitor and limit risk during high-return months (August–December, excluding November).

## Conclusion

This Tableau project presents a clear, data-driven narrative to understand and mitigate product returns. It provides both strategic and tactical recommendations backed by visual analysis.

\---


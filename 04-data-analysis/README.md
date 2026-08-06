# Data Analysis

Excel analysis: data cleaning, formulas, and pivot tables.
# Data Analysis

Excel-based analysis applying data cleaning, formulas, and pivot table techniques.

---

## 1. Data Cleaning

Raw operational data required cleaning before analysis. Issues identified and resolved:

| Issue | Impact on Analysis | Resolution |
|---|---|---|
| Duplicate records | Inflated transaction counts | Remove Duplicates |
| Inconsistent text casing | Same category counted separately | PROPER / UPPER standardization |
| Leading and trailing spaces | Lookup and matching failures | TRIM |
| Blank cells in key fields | Skewed averages and totals | Filter, review, and populate or exclude |
| Numbers stored as text | Formulas returning zero or errors | Convert to number format |

---

## 2. Formulas Applied

| Function | Business Question Answered |
|---|---|
| SUM | What is total revenue for the period? |
| AVERAGE | What is the average transaction value? |
| COUNTIF | How many orders came from each branch? |
| IF | Which orders exceed the approval threshold? |
| VLOOKUP | What is the product category for each item code? |

---

## 3. Pivot Table Analysis

Pivot tables were used to summarize transaction data across multiple dimensions.

**Analyses produced**

- Revenue by branch — identifying top and underperforming locations
- Transaction volume by month — surfacing seasonal demand patterns
- Percentage contribution per product category — via "Show Values As → % of Grand Total"
- PivotChart visualizations for stakeholder reporting

---

## 4. Analytical Takeaway

The value of the analysis lies not in the calculations themselves but in the decisions they support: which products to prioritize for restocking, which branches require operational review, and where demand patterns justify adjusting inventory levels.

---

**Tool used:** WPS Office Spreadsheets


# Part 1: Business Data Cleaning, Validation & Excel Reporting

## Business Problem Summary

This project focuses on cleaning, validating, and preparing a retail order dataset for business analysis. The raw dataset contained inconsistent text formatting, missing values, duplicate records, discount validation issues, date inconsistencies, and calculation mismatches. The objective was to create a clean, analysis-ready dataset and generate business reports for management decision-making.

---

## Dataset Used

Dataset: Retail Orders Dataset (Instructor Provided)

Files:
- raw_orders.xlsx (Original dataset)
- cleaned_orders.xlsx (Cleaned dataset)

---

## Tools Used

- Microsoft Excel
- Excel Formulas
- Pivot Tables
- Conditional Formatting
- Sorting & Filtering
- Data Validation

---

## Cleaning Steps Performed

### Text Cleaning
- Removed extra spaces.
- Standardized customer names.
- Standardized Region, State, City, Category and Sub-Category.
- Standardized Ship Mode.
- Standardized Payment Status and Order Status.

### Date Validation
- Checked missing Order Dates.
- Checked missing Ship Dates.
- Identified records where Ship Date was earlier than Order Date.

### Missing Values
- Missing Region replaced with "Unknown".
- Missing Ship Mode replaced with "Unknown".
- Missing Discount replaced with 0 according to business rules.

### Duplicate Validation
- Checked exact duplicate rows.
- Checked duplicate Order IDs.
- Flagged conflicting records for review.

### Business Rule Validation
- Negative discounts identified.
- Discounts above the allowed range checked.
- Cancelled and failed payment records identified.
- Returned/Refunded orders summarized separately.

### Calculated Columns Created
- cleaned_discount
- calculated_sales
- calculated_profit
- profit_margin
- shipping_delay_days
- order_month
- order_year
- data_quality_flag

---

## Data Quality Report

The report includes:

- Missing Value Summary
- Duplicate Summary
- Invalid Discount Summary
- Date Issue Summary
- Order Status Issue Summary
- Sales & Profit Calculation Mismatch Summary
- Final Summary

---

## Pivot Reports Created

The following Pivot Tables were developed:

1. Sales & Profit by Region
2. Sales & Profit by Category & Sub-Category
3. Order Count by Ship Mode
4. Average Profit Margin by Customer Segment
5. Returned/Cancelled/Failed Orders by Region
6. Monthly Sales Trend

---

## Key Business Insights

- Sales performance varies across different regions.
- Some categories generate higher profit than others.
- Standard Class is the most frequently used shipping method.
- Negative discount records require business review.
- Missing values were successfully handled according to business rules.
- Returned and cancelled orders reduce overall business performance.

---

## Business Rules Applied

- Missing Region → Unknown
- Missing Ship Mode → Unknown
- Missing Discount → 0
- Negative Discount → Flagged
- Ship Date before Order Date → Flagged
- Cancelled Orders excluded from completed sales analysis.
- Failed Payments excluded from completed sales analysis.
- Returned/Refunded Orders summarized separately.

---

## Assumptions

- Missing discount values were treated as zero where other sales information was available.
- Original source data was preserved without modification.
- Conflicting duplicate records were retained and flagged for review instead of deletion.

---

## Known Limitations

- The source dataset contained multiple date formats that required validation during cleaning.
- Some business validations depend on the quality of the source data provided.

---

## Repository Structure

```
data/
    raw_orders.xlsx
    cleaned_orders.xlsx

outputs/
    data_quality_report.xlsx
    pivot_summary.xlsx
    cleaning_log.md

screenshots/
    raw_data_preview.png
    cleaned_data_preview.png
    pivot_summary_1.png
    pivot_summary_2.png

README.md
```

---

## Screenshots Included

- Raw Dataset Preview
- Cleaned Dataset Preview
- Sales & Profit by Region Pivot Table
- Sales & Profit by Category Pivot Table

---

## Project Outcome

The retail order dataset was successfully cleaned, validated, standardized, and transformed into an analysis-ready dataset. Business rules were applied, calculated fields were created, data quality reports were generated, and management-ready Pivot Table summaries were prepared for business decision-making.

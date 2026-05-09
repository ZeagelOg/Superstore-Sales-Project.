# Superstore Sales — Excel Solution Walkthrough

> Corporate Segment Analysis | Canada's Largest Retail Chain | 8 Regions | 3,076 Orders

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Summary](#dataset-summary)
- [Files](#files)
- [Activity 1 — Excel Formatting & Reporting](#activity-1--excel-formatting--reporting)
- [Activity 2 — Pivot Table Profitability Analysis](#activity-2--pivot-table-profitability-analysis)
- [Conclusions & Recommendations](#conclusions--recommendations)
- [Tools Used](#tools-used)
- [Presentation Slides](#Presentation-Slides)

---

## Project Overview

This project analyzes Superstore Sales data across various regions in Canada, focusing exclusively on the **Corporate customer segment**. The work is divided into two activities:

- **Activity 1** — Clean, format, and build a structured report from raw sales data
- **Activity 2** — Use Pivot Tables to identify the top-3 most profitable and most loss-making product sub-categories by region

---

## Dataset Summary

| Attribute | Detail |
|-----------|--------|
| Retailer | Superstore Sales — Canada |
| Segment Focus | Corporate only |
| Total Orders | 3,076 |
| Regions Covered | 8 |
| Provinces Covered | 13 |
| Product Sub-categories | 17 |
| Total Sales | $5.5 Million |
| Total Profit | $599,000 |

---

## Files

| File | Description |
|------|-------------|
| `superstore_sales (1).csv` | Raw dataset |
| `superstore_sales_solution.xlsx` | Excel solution workbook (fully formatted) |
| `Superstore_Solution_Walkthrough.pptx` | Presentation deck (10 slides) |
| `README.md` | This file |

---

## Activity 1 — Excel Formatting & Reporting

### Section 1 & 2 — Initial Formatting & Segment Filtering

| Task | Description |
|------|-------------|
| Column Widths | All columns widened for readability; no truncated text |
| Header Formatting | Header row filled with colour; borders applied to all header cells |
| Segment Sheets | 4 new worksheets created: Corporate, Consumer, Home Office, Small Business |
| Data Split | Each segment's orders copied into its own dedicated sheet |
| Focus Sheet | All subsequent work performed on the Corporate worksheet only |

---

### Section 3 — Data Cleaning & Formatting

| Task | Description |
|------|-------------|
| Frozen Header | Top row frozen so headers stay visible while scrolling |
| Hidden Columns | Non-essential columns removed (e.g. Customer Segment — all rows are Corporate) |
| Sales & Profit | Rounded to 1 decimal place; formatted as US dollars ($) |
| Date Format | Order Date and Ship Date reformatted to readable format e.g. `15-Jan-2012` |
| Product Base Margin | Retained for profitability calculations |
| Order Quantity | Kept as integer — no rounding applied |

---

### Section 4 — Sorting & Conditional Formatting

**3-Level Sort Applied:**

1. Alphabetically by Region
2. Within Region: by Province (A to Z)
3. Within Province: by Sales (High to Low)

**Conditional Formatting Rule 1 — Top 10% Sales:**

- Top 10% orders by Sales within each Region/Province group
- Highlighted with light green fill and dark green border

**Conditional Formatting Rule 2 — Profit Heat Scale:**

| Colour | Meaning |
|--------|---------|
| Red | Heavy Loss |
| Yellow | Break Even |
| Green | High Profit |

---

### Section 5 — Report Finalization

| Task | Description |
|------|-------------|
| Double Bottom Borders | Applied to the last row of each Region group to visually separate regions |
| Page Layout | Column widths and print area adjusted; landscape orientation selected |
| Password Protection | Worksheet protected with a password to prevent accidental edits |

---

## Activity 2 — Pivot Table Profitability Analysis

### Top 3 Profitable Sub-Categories by Region

| Region | #1 Sub-Category | Profit ($) | #2 Sub-Category | #3 Sub-Category |
|--------|----------------|------------|----------------|----------------|
| Atlantic | Office Machines | $24,336 | Binders & Binder Acc. | Telephones & Comm. |
| Northwest Territories | Telephones & Comm. | $11,577 | Chairs & Chairmats | Copiers and Fax |
| Nunavut | Telephones & Comm. | $1,242 | Computer Peripherals | Envelopes |
| Ontario | Binders & Binder Acc. | $30,614 | Office Machines | Telephones & Comm. |
| Prarie | Office Machines | $91,914 | Telephones & Comm. | Computer Peripherals |
| Quebec | Office Machines | $14,107 | Chairs & Chairmats | Binders & Binder Acc. |
| West | Binders & Binder Acc. | $43,849 | Telephones & Comm. | Office Machines |
| Yukon | Telephones & Comm. | $11,421 | Appliances | Binders & Binder Acc. |

---

### Most Loss-Making Sub-Categories

| Sub-Category | Total Loss | Worst Regions |
|--------------|------------|---------------|
| Tables | -$35,431 | Ontario (-$16,169), Quebec (-$6,563), Atlantic (-$4,577) |
| Bookcases | -$9,306 | Quebec (-$11,367), NW Territories (-$3,270), Ontario (-$2,933) |
| Scissors, Rulers & Trim. | -$3,331 | Nunavut (-$1,760), Prarie (-$482), Quebec (-$359) |
| Storage & Organization | -$2,087 | Atlantic (-$7,288), Yukon (-$3,291), Quebec (-$2,369) |
| Rubber Bands | -$354 | West (-$119), Prarie (-$94), Quebec (-$84) |

---

## Conclusions & Recommendations

### Grow These

| Sub-Category | Total Profit | Notes |
|--------------|-------------|-------|
| Office Machines | ~$180,000 | Ranked #1 in Prarie and Atlantic |
| Binders & Accessories | ~$126,000 | Dominant in West and Ontario |
| Telephones & Comm. | ~$121,000 | Top performer in 4 of 8 regions |
| Appliances | ~$50,000 | Strong growth potential |

### Review / Discontinue

| Sub-Category | Total Loss | Action |
|--------------|------------|--------|
| Tables | -$35,431 | Loss in 6 of 8 regions — Ontario is worst; consider regional discontinuation |
| Bookcases | -$9,306 | Mainly a Quebec drag — review pricing strategy |
| Scissors / Rulers | -$3,331 | Loss concentrated in Nunavut and Prarie |
| Storage & Organization | -$2,087 | Profitable only in West and Prarie |

> **Note:** Tables and Chairs are complementary products. A regional discontinuation strategy is recommended over blanket removal to avoid impacting Chair sales.

---

## Tools Used

- Microsoft Excel — formatting, pivot tables, conditional formatting, password protection

## Presentation Slides
Slide 1
<img width="1296" height="733" alt="image" src="https://github.com/user-attachments/assets/d0ea0148-7af7-4793-82b2-ac9778df28b2" />

Slide 2
<img width="1292" height="737" alt="image" src="https://github.com/user-attachments/assets/a31ed392-e155-44fc-8f24-976b503f9266" />

Slide 3
<img width="1300" height="743" alt="image" src="https://github.com/user-attachments/assets/eac57eea-b42f-4fc7-aeb3-63203a9215d2" />

Slide 4
<img width="1304" height="735" alt="image" src="https://github.com/user-attachments/assets/9c224ba6-2e15-4c7b-8eda-1fb5181ca1c4" />

Slide 5
<img width="1300" height="742" alt="image" src="https://github.com/user-attachments/assets/b25feca9-a3da-41ca-b81c-7a41a22445c7" />

Slide 6
<img width="1282" height="729" alt="image" src="https://github.com/user-attachments/assets/bcad1718-13db-4542-bab5-87fc38c9bc13" />

Slide 7
<img width="1283" height="727" alt="image" src="https://github.com/user-attachments/assets/b7a9f87d-f8bf-4ec0-b719-f4297d576ba7" />

Slide 8
<img width="1289" height="734" alt="image" src="https://github.com/user-attachments/assets/d08fe637-3702-4a0f-99b3-333cdf3da1b0" />

Slide 9
<img width="1279" height="731" alt="image" src="https://github.com/user-attachments/assets/03502586-5a57-47f5-85dd-98463858d504" />

Slide 10
<img width="1291" height="737" alt="image" src="https://github.com/user-attachments/assets/b642ee01-8038-493d-98b2-4a2a5efb73f4" />



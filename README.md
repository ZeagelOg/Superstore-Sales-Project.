# 🛒 Superstore Sales — Excel Analysis Project

> A data analysis project on Canada's largest retail chain, performed entirely in Microsoft Excel.  
> Covers data cleaning, structured reporting, conditional formatting, and Pivot Table-based profit/loss insights for the **Corporate customer segment**.

---

## 📁 Project Structure

```
Superstore-Sales-Project/
├── superstore_sales (1).csv              # Raw dataset (original source data)
├── superstore_sales_solution.xlsx        # Excel workbook with full solution
├── Superstore_Solution_Walkthrough.pptx  # Presentation deck (10 slides)
└── README.md
```

---

## 🎯 Objectives

The project is split into two activities:

| Activity | Goal |
|----------|------|
| **Activity 1** | Clean, format, and build a structured sales report for the Corporate segment |
| **Activity 2** | Use Pivot Tables to identify the most profitable and most loss-making product sub-categories by region |

---

## 📊 Dataset Overview

- **Source:** Superstore Sales (Canada)
- **Segment:** Corporate (filtered from all 4 segments)
- **Orders:** 3,076
- **Regions:** 8 (Atlantic, Northwest Territories, Nunavut, Ontario, Prarie, Quebec, West, Yukon)
- **Provinces:** 13
- **Product Sub-Categories:** 17
- **Total Sales:** ~$5.5M
- **Total Profit:** ~$599K

---

## 🔧 Activity 1 — Data Cleaning & Report Building

### Section 1 & 2 · Basic Formatting & Filtering
- Widened all columns for readability
- Applied colour fill and borders to the header row
- Created **4 separate worksheets** — one per customer segment (Corporate, Consumer, Home Office, Small Business)
- Copied raw data of each segment into its respective sheet

### Section 3 · Report Making I
- Froze the header row for easy scrolling
- Deleted/hidden non-essential columns (e.g. Customer Segment — all rows are Corporate)
- Rounded **Sales** and **Profit** to 1 decimal place
- Formatted Sales and Profit as **US Dollar ($)**
- Reformatted Order Date and Ship Date to a readable format (e.g. `15-Jan 2012`)

### Section 4 · Report Making II

**Sorting:**
1. Alphabetically by **Region**
2. Within Region → alphabetically by **Province**
3. Within Province → **Sales descending**

**Conditional Formatting I — Top 10% Orders:**
- Within each Region → Province group, top 10% orders by Sales are highlighted in **light green fill** with a **dark green border**

**Conditional Formatting II — Profit Heat Scale:**
- Profits coloured on a **green scale** (darker = higher profit)
- Losses coloured on a **red scale** (darker = greater loss)

### Section 5 · Region Demarcation
- Applied **double bottom borders** to the last row of every Region group
- Adjusted page layout (landscape, fit-to-page) to minimise printed pages
- Added **password protection** to the worksheet

---

## 📈 Activity 2 — Pivot Table Analysis

### High-Profit Categories

Top 3 most profitable sub-categories per region (from Pivot Table):

| Region | #1 | #2 | #3 |
|--------|----|----|-----|
| Atlantic | Office Machines ($24K) | Binders & Acc. | Telephones & Comm. |
| Northwest Territories | Telephones & Comm. ($11.6K) | Chairs & Chairmats | Copiers and Fax |
| Nunavut | Telephones & Comm. ($1.2K) | Computer Peripherals | Envelopes |
| Ontario | Binders & Acc. ($30.6K) | Office Machines | Telephones & Comm. |
| Prarie | Office Machines ($91.9K) | Telephones & Comm. | Computer Peripherals |
| Quebec | Office Machines ($14.1K) | Chairs & Chairmats | Binders & Acc. |
| West | Binders & Acc. ($43.8K) | Telephones & Comm. | Office Machines |
| Yukon | Telephones & Comm. ($11.4K) | Appliances | Binders & Acc. |

**Key insight:** Office Machines and Telephones & Communication appear in the top 3 across almost every region.

---

### Loss-Making Categories

Most loss-making sub-categories across all regions:

| Sub-Category | Total Loss | Worst Regions |
|---|---|---|
| **Tables** | -$35,431 | Ontario (-$16K), Quebec (-$6.6K), Atlantic (-$4.6K) |
| **Bookcases** | -$9,306 | Quebec (-$11.4K), NW Territories (-$3.3K), Ontario (-$2.9K) |
| **Scissors, Rulers & Trimmers** | -$3,331 | Nunavut (-$1.8K), Prarie (-$482), Quebec (-$359) |
| **Storage & Organization** | -$2,087 | Atlantic (-$7.3K), Yukon (-$3.3K), Quebec (-$2.4K) |
| **Rubber Bands** | -$354 | West (-$119), Prarie (-$94), Quebec (-$84) |

> **💡 Note on Tables & Bookcases:** These are complementary furniture products — customers often buy them together. A regional discontinuation strategy is recommended over a blanket removal, since Bookcases are profitable in West and Prarie.

---

## ✅ Recommendations

### Grow 🟢
- **Office Machines** — $180K total profit, #1 in Prarie & Atlantic
- **Binders & Accessories** — $126K profit, dominant in West & Ontario
- **Telephones & Communication** — $121K profit, top performer in 4 regions
- **Appliances** — $50K profit, strong potential across regions

### Review / Discontinue 🔴
- **Tables** — Loss in 6 of 8 regions; consider regional pricing strategy
- **Bookcases** — Quebec is the primary drag; review supplier margins
- **Scissors, Rulers & Trimmers** — Niche product with thin margins
- **Storage & Organization** — Only profitable in West and Prarie

---

## 🛠 Tools Used

- **Microsoft Excel** — Data cleaning, formatting, conditional formatting, Pivot Tables

---

## 📜 License

This project is for educational purposes as part of a data analytics assignment.

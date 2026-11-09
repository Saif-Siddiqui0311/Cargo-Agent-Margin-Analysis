# 📦 Cargo Agent Margin Analysis

**Excel | Power Pivot | DAX | Dashboard design**

> I analysed 5 months of air cargo sales and airline costs to find out where an agent earns its margin, and why that margin almost doubled.

<img width="1904" height="962" alt="image" src="https://github.com/user-attachments/assets/6cbcdd94-71fe-49b7-a3c0-49949103ecef" />

*One month slicer controls every card, chart, and pivot on the page.*

---

## 🎯 Headline Results

| | |
|---|---|
| 💰 **Gross margin** | PKR 70.1M on PKR 303.4M sales (23.1%) |
| 📈 **Margin growth** | 15.3% in April → 29.0% in August |
| 🎯 **Scheduled target** | 115% attained over 5 months |
| ⚠️ **Loss batches** | 72 in total (PKR 0.37M), 56 of them in April |

---

## ❓ Questions I Answered

1. How did sales, margin, and yield change month by month?
2. Did scheduled flights meet their targets?
3. Which routes, clients, and commodities matter most?
4. How well are flights used?
5. Where does the business lose money?

---

## 🛠️ Tools

- **Excel Tables** with structured references
- **Power Pivot and DAX** measures (Yield per kg, Margin %, Distinct Count)
- **PivotTables, PivotCharts, and a Slicer** controlling 12 pivots at once
- **SUMIFS, COUNTIFS, SUMIF, GETPIVOTDATA**, sparklines, conditional formatting

---

## 🔍 The Analysis

### 1. Monthly P&L (*NET Revenue sheet*)
Sales and margin per month from one batch-level table.
- **July was the turning point:** sales +65% vs June (weight +34%, yield +24%).
- **July and August produced 66%** of the total margin.

### 2. Target vs Actual (*Dashboard, MGR Target*)
```excel
Attainment = Scheduled revenue / Target
```
- April to June: 94% to 99% of target.
- July and August: **150% and 131%.** Targets did not keep up with the business.

### 3. Sectors (*Sector sheet*)
I split each monthly revenue change into a **weight effect** and a **yield effect**, so it shows *why* revenue moved.
- **KHI–LHE** is 32% of revenue and 41% of margin.
- Return legs sell much cheaper: **ISB–KHI PKR 45/kg vs KHI–ISB PKR 86/kg.**

### 4. Clients (*Client sheet*)
- Cash Sales (walk-in) is **53% of revenue**.
- But credit clients drove the growth: **cash share fell from 81% to 29%.**

### 5. Flights (*Flight sheet*)
- Top 5 flights earn **42% of revenue**.
- Flights carried **75% of their pricing estimate** overall. FL-034 carried 3×, while FL-009 used only 17%.

### 6. Commodities (*Commodity sheet*)
- Courier Mail is **34% of revenue**.
- **High yield ≠ high margin:** Valuable Goods earns PKR 141/kg but only a 14.7% margin. Auto Parts earns 42%.

### 7. Loss Batches (*NET Revenue sheet*)
- 56 of the 72 loss batches happened in **April**. After that, only 3 to 5 per month.

---

## 💡 What I Learned

- 🧱 **Data modelling:** merging sales and cost into one batch table removed label mismatches.
- 🧮 **DAX measures:** define once, reuse in every pivot.
- 🎛️ **Dashboard control:** one slicer, one consistent view.
- 📊 **Variance analysis:** explaining *why* numbers moved, not only *how much*.

---

## ✅ Conclusions (C-suite Summary)

1. **Pricing drove the margin growth.** Yield rose 27% while airline cost per kg rose only 6%.
2. **Two corridors carry the business:** Karachi–Lahore and Karachi–Islamabad produce 82% of revenue.
3. **Return legs are underpriced** and need a plan.
4. **Targets and capacity estimates are out of date** and should be reset.
5. **Loss control works:** loss batches fell from 56 to about 4 per month.

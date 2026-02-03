# SCOR-Based Supply Chain Analytics (AuraGlow Beauty | Simulated)

A portfolio-style supply chain analytics project using the **SCOR model (Plan, Source, Make, Deliver, Return)** to clean, analyze, visualize, and interpret supply chain performance for a D2C beauty brand (**simulated**) with **600 records**.

## 🎯 Objective
Collect/simulate supply chain data, perform **data cleaning + analysis + visualization**, and generate actionable insights mapped to **SCOR**.

## 🧰 Tech Stack
- **Excel**: data cleaning + sanity checks  
- **Tableau**: interactive dashboards + storytelling  
- **Python (Jupyter)**: exploratory analysis + validation checks  

## 📦 Dataset (Simulated)
The dataset contains 600 rows covering:
- SKU, product type, price, availability, units sold, revenue
- stock levels, lead times, order quantities
- shipping time/cost, routes, transport mode, carrier
- supplier, manufacturing costs/lead time, inspection results, defect rates

> Note: This is a simulated dataset created for academic analysis.

---

## 🧭 SCOR Framework: What I Analyzed

### 1) PLAN — Demand & Inventory
- Identified inventory gaps and stock-out risk zones
- Cross-checked whether stock issues are driven by demand vs lead-time variability

### 2) SOURCE — Supplier Performance
- Benchmarked suppliers on defect risk vs cost impact  
- Flagged the "double-liability" supplier (high cost + high defects)
- Recommendation: shift volume to a safer cost-effective alternative supplier

### 3) MAKE — Manufacturing Quality & Cost
- Compared manufacturing costs across product categories
- Identified where higher costs also correlate with quality leakage

### 4) DELIVER — Logistics & Regional Performance
- Compared regional performance for sales, profit, and defect outcomes  
- Identified a “Perfect Order” benchmark region

### 5) RETURN — Reverse Logistics
- Quantified where returns/quality failures create the most operational cost
- Framed next steps to isolate root cause (manufacturing vs transit damage)

---

## 🔍 Key Insights (Highlights)
- **Supplier strategy**: prioritize quality to protect brand equity; transition away from the high-cost/high-defect supplier.
- **Inventory risk**: a high-demand region faces stock-out risk driven by lead-time variability (not just demand).
- **Category focus**: one category tends to show higher manufacturing costs *and* higher defect rates → needs tighter QC.
- **Regional benchmark**: one city consistently performs best on profit + quality → use it as the operational standard.
- **Returns**: reverse logistics costs spike where defects are highest → focus root-cause isolation.

---

## 📊 Dashboards & Visual Outputs
**Tableau dashboards** are included in `/dashboards/tableau/`.

Add screenshots here so GitHub instantly shows the work:

| Dashboard | Preview |
|---|---|
| Location Insights | ![Location](assets/dashboard_location.png) |
| Procurement Analysis | ![Procurement](assets/dashboard_procurement.png) |
| Shipping Routes | ![Routes](assets/dashboard_routes.png) |

> Tip: Export each Tableau dashboard as PNG and save in `/assets/`.

---

## ▶️ How to Run (Python)
1. Install dependencies:
   ```bash
   pip install -r requirements.txt

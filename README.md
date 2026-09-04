# Luxottica-Inventory-Dashboard
# 🕶️ EssilorLuxottica Data Pipeline & Executive Inventory Dashboard

## 📌 Project Overview & Core Business Problem
An active wholesale distribution center for **EssilorLuxottica** luxury eyewear brands (**Ray-Ban** and **Oakley**) was experiencing workflow delays due to a flat, unformatted database layout. 

### Key Operational Challenges:
1. **Procurement Delays:** The buying team had no visual indicator to separate stock anomalies requiring immediate purchasing ("Reorder") from stable listings ("OK").
2. **Static Pricing Models:** The lack of programmatic margins forced manual adjustments on luxury assets, leading to pricing errors and missing profit targets.
3. **Data Contamination:** Raw system extractions combined deep SKU metadata (Brand, Model, Color, and Eye Size) into single text blocks wrapped in excessive whitespace, breaking search strings.

**The Solution:** Engineered a clean horizontal data architecture, applied advanced psychological tiered retail models, deployed mixed-reference exceptions highlighting, and packaged the engine into a dynamic, filterable executive reporting canvas.

---

## 🧹 Phase 1: Advanced Data Triage & String Transformation
Legacy system strings required deep formatting stabilization before running nested search protocols:
* **Whitespace Pruning:** Deployed `=TRIM()` optimization chains across raw values to safely isolate invisible keystroke spacing corruptions that cause lookup array crashes (`#N/A`).
* **Multi-Step Delimiter Parsing:** Executed structural parsing layers using **Text to Columns** data parameters. Segregated complex multi-element SKU strings (e.g., `RAYBAN-RB2140-TOR-50`) using uniform boundaries (`-`) into clean categorical attributes: **Brand, Model Name, Color,** and **Eye Size**.

---

## 💡 Phase 2: Tiered Mathematical Modeling & Psychological Pricing
To satisfy strict brand guidelines, I constructed an automated cost-plus pricing layer to scale retail values with localized market segments:
* **Conditional Tiered Markup Rules:** Programmed a dynamic validation engine utilizing integrated `=IF()` logical formulas to partition margin rules between standard lines and ultra-premium products.
* **Whole-Dollar Charm Price Formatting:** Nested the pricing tier arrays inside an `=MROUND()` wrapper. Configured the rounding array to automatically snap variable decimal calculations to uniform corporate price ceilings finishing tightly on an executive flat currency flag (`$9.00`).
```excel
=MROUND(IF(G2<90, G2*2.2, G2*2.6), 10) - 1
```
*This infrastructure automatically targets a baseline portfolio markup matrix between 54.46% and 61.92%, stabilizing margins safely at a **57.70% overall average profit floor**.*

---
<img width="1180" height="724" alt="image" src="https://github.com/user-attachments/assets/7916ceec-25c6-4df0-b7a1-273f27c65442" />

## 🎨 Phase 3: Interactive UI Dashboard & Automation Alerts
To maximize administrative processing and executive tracking velocities, the clean table was integrated into a live visualization suite:

* **Mixed-Reference Condition Triggers:** Developed formula-driven conditional rules across the complete `A2:M125` array. By hard-locking structural lookup target references (`=$H2="Reorder"`), the spreadsheet automatically flashes **entire horizontal database rows in light red** the instant a SKU breaches its minimum safety volume.
* **Synchronized Reporting Grids:** Grouped complex line items into nested Pivot Table groupings tracking overall Wholesale Assets Capital vs. Retail Revenue Realization potentials.
* **Front-End Dashboard Suit:** Implemented a cloud-synchronized **Status Slicer** coupled with an animated **2D Clustered Column Pivot Chart** mapped with absolute currency bounds ($Y-Axis$).

---
<img width="926" height="592" alt="image" src="https://github.com/user-attachments/assets/ba17fe95-d5da-472d-bda8-63512f961640" />

## 🌟 Business Outcomes & Key Analytical Insights
* **Targeted Capital Allocations:** The finalized application allows executives to filter out stable lines instantly. By selecting the **"Reorder"** filter tab, the dashboard isolates that the facility holds a bottleneck of **$48,593.10 in unreleased wholesale capital**, which will generate **$120,901.00 in future retail revenue value**.
* **Operational Strategy Mapping:** The synchronized Pivot Chart quickly establishes that **Ray-Ban** accounts for the largest chunk of outstanding low-stock backlogs, directing procurement teams to execute Ray-Ban replenishment cycles prior to processing secondary labels.

---

## 📂 Repository Contents
* `EssilorLuxottica_Inventory_Dashboard.xlsx` - Main interactive dashboard application.
* `Project_Documentation.md` - Comprehensive deployment steps and analytical summaries.

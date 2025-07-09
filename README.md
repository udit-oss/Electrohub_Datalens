Electrohub_DataLens_Project/
├── 1.Business_Problem/
│ └── Business_Problem.docx ← problem statement & key questions
│
├── 2.Data/
│ ├── 1.Raw_Data/ ← original Excel data
│ │ └── Store_Data.xlsx ← 4 sheets: Dim Customers, Dim Product, Dim Promotion, Sheet3 (Fact Table)
│ │
│ └── 2.Cleaned_Data/ ← exported Excel after Power Query
│ └── Dim_Customers.xlsx
| └── Dim_Products.xlsx
| └── Dim_Promotions.xlsx
| └── Fact_Table.xlsx
│
├── 3.Data_Dictionary/
│ └── Data_Dictionary.xlsx ← definitions for every field & calculation
│
├── 4.Transformations/
│ └── Methodology.docx ← step‑by‑step Power Query ETL narrative
│
├── 5.Power_BI_Report/
│ └── Electrohub_DataLens.pbix ← main Power BI report file
│
├── 6.Summary/
│ └── Electrohub_DataLens_Summary.pptx ← executive slide deck with screenshots & insights

## 🚀 Getting Started

1. **Open the Power BI Report**  
   - Launch Power BI Desktop and open `5.Power_BI_Report/Electrohub_DataLens.pbix`.

2. **Refresh Data**  
   - Place the latest `Store_Data.xlsx` in `2.Data/Raw_Data/`.  
   - In Power BI: **Home → Refresh**.  
   - (Optional) Export cleaned tables to `2.Data/Cleaned_Dara/` via **Data view → Copy Table → Paste into CSV**.

3. **Review ETL Steps**  
   - Open `4.Transformations/Methodology.docx` to see each Power Query step: renames, merges, calculated columns, data‑type settings.

4. **Field Definitions**  
   - See `3.Data_Dictionary/Data_Dictionary.xlsx` for full list of raw and derived fields, their sources, and formulas.

5. **Explore Dashboards**  
   - Use the **“Overview”** page for topline KPIs & filter controls.  
   - Navigate to **Product Rankings**, **Period Comparison**, **Promo & Regional Insights**, and **Detail** pages for deeper analysis.

6. **Presentation**  
   - The slide deck in `6.Summary/Electrohub_DataLens_Summary.pptx` summarizes key findings, visuals, and recommendations.

---

## 🛠️ Technical Details

- **Tooling:** Power BI Desktop (Power Query, DAX)  
- **Data Model:** Star schema with one active Date table and two disconnected slicer tables for period comparisons  
- **Key DAX Measures:**  
  - Net Sales, Total Sales, Discount Value, Profit, Average Order Value, Profit Margin %  
  - Period Comparison measures (`Sales P1`, `Sales P2`, `Profit P1`, `Profit P2`, `Qty P1`, `Qty P2`)

---

Thank you for reviewing the Electrohub DataLens project! Feel free to reach out with any questions or feedback.

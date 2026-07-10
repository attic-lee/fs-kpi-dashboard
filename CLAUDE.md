# CLAUDE.md — Project A: Financial Services KPI Dashboard

## Task
Set up GitHub repo and push all files for Project A.

## Who I Am
**Name:** Attic C. Lee
**GitHub:** attic-lee

## Repo Details
- **Name:** `fs-kpi-dashboard`
- **Visibility:** Public
- **Local path:** `C:\Users\Attic\code\fs-kpi-dashboard\`

## Folder Structure to Create
```
fs-kpi-dashboard/
├── data/
│   ├── am_fund_performance.csv
│   ├── rb_product_revenue.csv
│   ├── ins_claims_premiums.csv
│   └── macro_benchmarks.csv
├── outputs/
│   ├── dashboard_am.png           ← screenshot from Power BI Page 1
│   ├── dashboard_rb.png           ← screenshot from Power BI Page 2
│   ├── dashboard_ins.png          ← screenshot from Power BI Page 3
│   └── dashboard_summary.png     ← screenshot from Power BI Page 4
├── FS_KPI_Dashboard.pbix
├── FS_KPI_Financial_Model.xlsx
├── README.md
├── CLAUDE.md
└── .gitignore
```

## README.md to Create
```markdown
# Financial Services KPI Dashboard

A cross-sector analytics dashboard covering three FS sectors built in Power BI.

## Sectors Covered
- **Asset Management** — 6 funds, AUM tracking, active return vs benchmark
- **Retail Banking** — 8 products, revenue, NPS, cost-income ratio
- **Insurance** — 6 lines of business, combined ratio, GWP, underwriting profit

## Key Metrics
| Sector | Headline KPI | Value |
|--------|-------------|-------|
| Asset Management | Avg AUM | £736mm across 6 funds |
| Asset Management | Avg Active Return | -5.82 bps (2022 bear market drag) |
| Asset Management | Fee Income | £93.43k |
| Retail Banking | Total Revenue | £1.75M |
| Retail Banking | Avg NPS Score | 31.50 |
| Retail Banking | Avg CIR | 0.62 (within benchmark) |
| Insurance | Total GWP | £1.18M |
| Insurance | Avg Combined Ratio | 0.91 (profitable) |
| Insurance | Avg Loss Ratio | 0.64 |

## Dashboard Pages
1. **Asset Management** — AUM trend by fund (Jan 2022–Dec 2024), active return vs benchmark, year slicer
2. **Retail Banking** — Revenue by product, NPS by product
3. **Insurance** — Combined ratio by line (with 1.0 reference line), GWP by line
4. **Group Summary** — Executive overview across all three sectors with key insights

## Screenshots
![Asset Management](outputs/dashboard_am.png)
![Retail Banking](outputs/dashboard_rb.png)
![Insurance](outputs/dashboard_ins.png)
![Group Summary](outputs/dashboard_summary.png)

## Tech Stack
- **Power BI Desktop** — 4-page dashboard
- **DAX** — KPI measures
- **Excel** — 6-sheet financial model (industry colour coding)
- **Python** — data generation (pandas, numpy)

## Excel Financial Model
`FS_KPI_Financial_Model.xlsx` — 6 sheets with industry-standard colour coding:
- 🔵 Blue text = hardcoded inputs
- ⚫ Black text = formulas
- 🟢 Green text = cross-sheet links
- 🟡 Yellow background = key assumptions

## Data
756 rows across 4 CSV files — synthetic data using real FS industry
terminology, metrics, and realistic value ranges (Jan 2022–Dec 2024).

## Key Insights
- **Asset Management:** Global Bond Income and Infrastructure Debt generate
  positive alpha — UK Equity Growth underperforms benchmark
- **Retail Banking:** Mortgages drives highest revenue; Trade Finance has
  lowest NPS score — opportunity for service improvement
- **Insurance:** All 6 lines profitable (combined ratio < 1.0);
  Liability and Commercial Property most efficient lines

---
*Attic C. Lee — CV Portfolio Project A*
```

## .gitignore to Create
```
__pycache__/
*.pyc
.env
.DS_Store
*.log
~$*.xlsx
~$*.pbix
```

## Git Commands to Run
```bash
cd C:\Users\Attic\code\fs-kpi-dashboard
git init
git add .
git commit -m "Initial commit — FS KPI dashboard (Power BI) and financial model (Excel)"
git remote add origin https://github.com/attic-lee/fs-kpi-dashboard.git
git branch -M main
git push -u origin main
```

## Files I Will Copy Manually
Before pushing, I will copy these files into the correct folders:
- `FS_KPI_Dashboard.pbix` → root folder
- `FS_KPI_Financial_Model.xlsx` → root folder
- `am_fund_performance.csv` → `data/`
- `rb_product_revenue.csv` → `data/`
- `ins_claims_premiums.csv` → `data/`
- `macro_benchmarks.csv` → `data/`
- Power BI screenshots → `outputs/`

## Instructions for Claude Code
1. Create the folder structure at `C:\Users\Attic\code\fs-kpi-dashboard\`
2. Create `README.md` with the content above
3. Create `.gitignore` with the content above
4. Create `CLAUDE.md` (this file) in the root
5. Tell me when the structure is ready so I can copy the files in
6. Once I confirm files are copied, run the git commands to push to GitHub
7. Note: browser login prompt will appear for GitHub authentication — I will handle that

## CV Bullet (ready to paste after push)
> Built a 4-page cross-sector financial services KPI dashboard (Power BI, DAX)
> covering asset management (AUM £736mm, 6 funds), retail banking (£1.75M revenue,
> 8 products), and insurance (combined ratio 0.91, 6 lines). Delivered alongside an
> industry-standard Excel financial model with blue/black/green colour coding and
> 47 live formulas across 6 sheets.

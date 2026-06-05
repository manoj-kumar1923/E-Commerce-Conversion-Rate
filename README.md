# 🛒 E-Commerce Conversion Rate Tracker

A professional Excel-based project for tracking, analyzing, and optimizing e-commerce conversion rates across the full purchase funnel — from traffic acquisition through to completed orders.

---

## 📁 Repository Structure

```
ecommerce-conversion-rate/
├── ECommerce_Conversion_Rate.xlsx   # Main Excel workbook (5 sheets)
├── create_excel.py                  # Python script to regenerate the workbook
├── README.md                        # Project documentation
├── .gitignore                       # Git ignore rules
└── sample_data/
    ├── raw_data.csv                 # Monthly funnel metrics (CSV)
    └── channel_data.csv             # Channel breakdown (CSV)
```

---

## 📊 Workbook Overview — 5 Sheets

| Sheet | Description |
|-------|-------------|
| **Raw Data** | 12-month monthly funnel data: Visitors → Sessions → Cart → Checkout → Orders, with formula-driven CVR columns |
| **Dashboard** | KPI cards + 3 charts (CVR trend, Revenue bars, Funnel stage comparison) |
| **Funnel Analysis** | Stage-by-stage drop-off analysis with benchmark comparisons and auto status flags |
| **Channel Breakdown** | CVR, AOV, and revenue share by 7 acquisition channels |
| **Insights & Actions** | 7 data-driven optimization recommendations with actionable next steps |

---

## 📐 Metrics Tracked

### Funnel Stages
```
Total Visitors → Sessions → Add-to-Cart → Checkout Initiated → Orders Placed
```

### Key Metrics
| Metric | Formula |
|--------|---------|
| **Overall CVR** | Orders / Total Visitors |
| **Session → Cart Rate** | Add-to-Cart / Sessions |
| **Cart → Checkout Rate** | Checkouts / Add-to-Cart |
| **Average Order Value (AOV)** | Revenue / Orders |
| **Drop-Off %** | (Stage N − Stage N+1) / Stage N |

---

## 📈 Charts Included

- **Line Chart** — Monthly overall CVR % trend (Jan–Dec)
- **Bar Chart** — Monthly revenue ($)
- **Multi-line Chart** — All three funnel stage rates side-by-side

---

## 🚀 Getting Started

### Prerequisites
- Microsoft Excel 2016+ **or** LibreOffice Calc 7+
- Python 3.8+ with `openpyxl` (only if regenerating the workbook)

### 1. Clone the Repository
```bash
git clone https://github.com/manoj-kumar1923/E-Commerce-Conversion-Rate/blob/main/Screenshot_2026-06-05_165912%5B1%5D.png
cd ecommerce-conversion-rate
```

### 2. Open the Workbook
Open `ECommerce_Conversion_Rate.xlsx` in Excel and navigate to the **Dashboard** sheet for a visual overview.

### 3. Enter Your Own Data
1. Go to the **Raw Data** sheet.
2. Replace the values in columns B–G (rows 5–16) with your actual monthly metrics.
3. All CVR formulas, charts, and dashboard KPIs will update automatically.

### 4. Regenerate the Workbook (Optional)
```bash
pip install openpyxl
python create_excel.py
```

---

## 🎨 Design Conventions

| Color | Usage |
|-------|-------|
| 🔵 Dark Navy `#0D2137` | Primary headers, labels |
| 🔵 Blue `#1565C0` | Sub-headers, secondary data |
| 🟢 Teal `#00796B` | Session→Cart rate |
| 🟠 Orange `#E65100` | Overall CVR %, highlights |
| 🟣 Purple `#6A1B9A` | Cart→Checkout rate |
| 🟡 Amber `#F57F17` | Totals row |
| 🟢 Gold `#FFC107` | Annual summary |

---

## 🏷️ Industry Benchmarks Used

| Stage | Benchmark |
|-------|-----------|
| Session → Add-to-Cart | 25% |
| Add-to-Cart → Checkout | 13% |
| Overall CVR (Visitors → Orders) | 5.5% |

*Source: Baymard Institute / Google Ads industry averages*

---

## 🛠️ Customization Tips

- **Add more channels**: Extend the Channel Breakdown sheet with rows for TikTok Ads, Affiliate, etc.
- **Weekly granularity**: Duplicate the Raw Data sheet and adjust column headers to weeks.
- **A/B test tracking**: Add a new sheet with test name, variant, CVR per variant, and statistical significance.
- **Goal targets**: Add a "Target CVR" column to Raw Data and a variance column `=Actual - Target`.

---

## 📄 License

MIT License — free to use, fork, and adapt.

## 🤝 Contributing

Issues and pull requests are welcome. Please open an issue first for major changes.

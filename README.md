# Market Basket Analysis – BIL 476 Final Project

## Project Overview
Comprehensive Market Basket Analysis on the UCI "Online Retail" dataset using Apriori and FP-Growth algorithms with advanced null-invariant metric evaluation.

## Requirements
- Python 3.10+
- pandas, numpy, matplotlib, seaborn, mlxtend, openpyxl

### Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn mlxtend openpyxl
```

## Dataset
Download the **Online Retail** dataset from the [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/online+retail) and place `Online Retail.xlsx` in the project root.

## Usage
```bash
python veriyükleme.py
```

This will execute the full pipeline:
1. **Data Loading & Preprocessing** – Removes missing values, cancellations, zero-quantity entries
2. **EDA** – Generates Top 10 products, country distribution, and monthly trend charts
3. **Algorithm Comparison** – Runs Apriori and FP-Growth, benchmarks execution time
4. **Rule Analysis** – Generates association rules with Support, Confidence, Lift, Kulczynski, and Cosine metrics
5. **Misleading Rule Detection** – Identifies rules with high confidence but negative correlation (Lift ≤ 1.0)
6. **Sensitivity Analysis** – Tests min_support thresholds: 0.03, 0.05, 0.07, 0.10
7. **Multi-Country Comparison** – Compares rule quality across France, Germany, and Spain

## Output Files
| File | Description |
|------|-------------|
| `grafik_top10_urun.png` | Top 10 most sold products |
| `grafik_ulke_dagilimi.png` | Transaction distribution by country |
| `grafik_aylik_trend.png` | Monthly transaction trend |
| `grafik_apriori_vs_fpgrowth.png` | Algorithm execution time comparison |
| `grafik_association_scatter.png` | Support vs Confidence scatter (colored by Lift) |
| `grafik_sensitivity_analysis.png` | Sensitivity analysis across min_support values |
| `grafik_multi_country.png` | Multi-country rule comparison |

## Report
The IEEE-format report is available in `final_report.tex`. Compile in Overleaf or any LaTeX editor.

## Author
Fatma Zehra Nur Paksoy – TOBB ETU – 211401009

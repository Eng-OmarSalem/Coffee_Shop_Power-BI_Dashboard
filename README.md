[README.md](https://github.com/user-attachments/files/30863952/README.md)
<div align="center">

# ☕ Coffee Trend Spend Analysis Dashboard

**An interactive Power BI dashboard tracking $112K in coffee-shop spend across 3,547 transactions — peak hours, weekday vs. weekend habits, and per-drink trends, all cross-filterable by coffee type.**

[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=flat-square&logo=powerbi&logoColor=black)](#-interactive-dashboard)
[![Data](https://img.shields.io/badge/Transactions-3%2C547-6F4E37?style=flat-square)](#-dataset)
[![Period](https://img.shields.io/badge/Period-Mar%202024%20--%20Mar%202025-6F4E37?style=flat-square)](#-dataset)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](#-license)

</div>

---

## 📖 Overview

This project analyzes just over a year of point-of-sale data (March 2024 – March 2025) from a coffee shop, turning raw transaction logs into a single-page Power BI dashboard that answers the questions a shop owner actually cares about: *When are we busiest? Which drinks sell? Do weekends make up for slower weekdays?*

Every visual on the dashboard responds instantly to the coffee-type filter bar at the top — click "Cocoa" and the whole page, KPIs, charts, and all, recalculates to show that drink alone.

## ✨ Highlights

- ☕ **3,547 transactions, $112K in total spend**, spanning March 2024 to March 2025 (381 distinct days of sales).
- 🖱️ **One filter bar, eight drinks** — Americano, Americano with Milk, Cappuccino, Cocoa, Cortado, Espresso, Hot Chocolate, and Latte — every visual cross-filters live when you click one.
- ⏰ **Peak hour identified automatically**: 10 AM, generating ~$10.2K of the $112K total on its own.
- 📅 **Weekday vs. weekend breakdown**: weekdays drive 75% of spend ($84K) vs. 25% on weekends ($28K) — with average spend per weekday running higher than per weekend day.
- 🌗 **Time-of-day segmentation** (Morning / Afternoon / Night) via a donut chart, plus a 13-month spending trend line and a day-of-week bar chart.
- 💳 **100% card transactions** — every single one of the 3,547 sales in the dataset was paid by card, not cash.

## 📊 Interactive Dashboard

**Full view — all drinks**

<img src="Screenshot_2026-08-09_003300.png" alt="Coffee dashboard, unfiltered view" width="100%">

The default view: total spend, cups sold, and peak-hour KPIs up top, with the 13-month spending trend, day-of-week breakdown, and time-of-day donut chart filling out the page.

**Filtered view — Cocoa only**

<img src="Screenshot_2026-08-09_003340.png" alt="Coffee dashboard filtered to Cocoa" width="100%">

Clicking a single drink (here, "Cocoa") instantly recalculates every KPI and chart on the page — $8,521 in Cocoa sales, 239 cups, with its own peak hour (8 PM) and weekday/weekend split.

## 🗂️ Dataset

| | |
|---|---|
| **File** | `coffee_data.csv` |
| **Transactions** | 3,547 |
| **Period** | March 1, 2024 – March 23, 2025 (381 distinct days) |
| **Drinks** | 8 — Americano, Americano with Milk, Cappuccino, Cocoa, Cortado, Espresso, Hot Chocolate, Latte |
| **Payment method** | Card only (100% of transactions) |

Columns: `hour_of_day`, `cash_type`, `money(Rs)`, `coffee_name`, `Time_of_Day`, `Weekday`, `Month_name`, `Weekdaysort`, `Monthsort`, `Date`, `Time`. The `*sort` columns exist purely so the dashboard's day-of-week and month charts display in calendar order rather than alphabetically.

> **Note on currency:** the source column is named `money(Rs)`, but the dashboard's number formatting displays values with a `$` symbol. Figures in this README follow the dashboard's own display convention — treat the currency symbol as a formatting choice, not a confirmed currency conversion.

## 💡 Key Insights

- **Latte and Americano with Milk are the top earners** — $26.9K and $24.8K respectively — despite Americano with Milk having the highest transaction *count* (809 orders), meaning Latte earns more per cup on average.
- **Espresso is the long tail**: only 129 orders and $2.7K total, the smallest of all 8 drinks by a wide margin.
- **Weekday reliance is heavy**: 75% of all spend happens Monday–Friday, so weekend promotions could be a real lever for growth.
- **10 AM is the single best hour** to be fully staffed — it consistently outperforms every other hour of the day in the dataset.

## 🛠️ Tech Stack

`Power BI Desktop` · `Power Query` · `DAX`

## 📁 Project Structure

```
.
├── Coffee_Dashboard.pbix              # Power BI dashboard (Power Query + DAX + report page)
├── coffee_data.csv                    # source transaction data (3,547 rows)
├── Screenshot_2026-08-09_003300.png   # dashboard screenshot: full/unfiltered view
├── Screenshot_2026-08-09_003340.png   # dashboard screenshot: filtered to Cocoa
└── README.md
```

## 🚀 Getting Started

**Prerequisites:** [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).

1. Clone or download this repository.
2. Open `Coffee_Dashboard.pbix` in Power BI Desktop.
3. If prompted to locate the data source, point it at `coffee_data.csv` in this repo.
4. Click any drink in the filter bar at the top to explore — every KPI and chart updates instantly.

## 📜 License

Code and report design in this repository are available under the [MIT License](LICENSE). The dataset is provided as-is for portfolio/educational use.

## 📬 Contact

Questions or feedback? Open an issue, or reach out at **[salemomar676@gmail.com](mailto:salemomar676@gmail.com)** · [LinkedIn](https://www.linkedin.com/in/eng-omarsalem) · [Portfolio](https://gamma.app/docs/Copy-of-Brand-Partnership-Proposal-lrp9yrhau9gdpj1)

</div>

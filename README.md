# Household Electricity Consumption Analysis

**Python Programming: Individual Case Study (Internal Assessment)**
Manjari Majumdar · RA2411005010075 · B.Tech EEE, SRM Institute of Science and Technology, Chennai

## Problem
A monthly electricity bill shows one number, the total. It doesn't show which appliances use the most energy, which days are unusually heavy, or how slab tariffs push the bill up. This project uses beginner-level Python to analyse 30 days of appliance-wise consumption for a household and turn the readings into useful information.

## Files
| File | Description |
|---|---|
| `RA2411005010075_ManjariMajumdar_CaseStudy.ipynb` | Executed notebook: code, outputs, plots, observations |
| `RA2411005010075_ManjariMajumdar_CaseStudy.pdf` | Case study report |
| `RA2411005010075_ManjariMajumdar_Dataset.csv` | Simulated dataset (30 days × 6 appliances, kWh) |
| `figures/` | Plots exported from the notebook |

## Python concepts used
Variables, lists, tuples (tariff slabs), sets (weekend days), dictionaries (daily records), `for` loops, `if-elif-else`, and six user-defined functions:
`load_data()`, `appliance_totals()`, `daily_totals()`, `find_high_usage_days()`, `weekday_vs_weekend()`, `calculate_bill()`.

## Key results
- The **AC** uses **44.3%** of the month's 377.66 kWh. Lights and fans come second at 20.3%.
- **Weekend** use is **37.7% higher** than weekday use (15.75 vs 11.44 kWh/day).
- **9 of 30 days** exceeded the 14 kWh/day threshold. 8 of them were weekends.
- The estimated bill is **₹1,070** under an illustrative slab tariff. Cutting AC use by 20% saves about **₹157/month**.

![Daily consumption](figures/fig1_daily_trend.png)
![Appliance-wise consumption](figures/fig2_appliance_bar.png)

## How to run
```bash
pip install -r requirements.txt
jupyter notebook RA2411005010075_ManjariMajumdar_CaseStudy.ipynb
```
Keep the CSV in the same folder as the notebook.

## Notes
The dataset is simulated; no external data was used. The tariff values are illustrative, modelled on the slab structure of Tamil Nadu domestic tariffs.

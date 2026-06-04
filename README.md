# Tire Shop Customer Experience KPI Dashboard

A Tableau dashboard tracking customer-facing KPIs for a retail tire shop, built to mirror the performance monitoring I performed as Assistant Manager at Discount Tire. The dashboard focuses on the **Quality** and **Delivery** pillars of the SQDC scorecard framework.

---

## Background

In my role as Assistant Manager, I regularly analyzed store KPI scorecards to identify performance gaps and drive improvements across the team. This project recreates that workflow in Tableau using a structured dataset — turning operational experience into a data portfolio piece.

---

## Dashboard Overview

The dashboard consists of three interconnected views, all filterable by service type:

| Sheet | What it shows |
|---|---|
| On-Time Completion Rate by Week | Weekly trend of on-time service completions across January 2024 |
| Avg Turnaround Time by Technician | Bar chart comparing each technician's average job duration against a 60-minute target |
| Quality by Service Type | Combo chart of average CSAT score (bars) and comeback rate % (line) per service type |

---

## KPIs Tracked

**Delivery**
- On-time completion rate (target: 100%)
- Average turnaround time in minutes (target: ≤60 min)

**Quality**
- Customer satisfaction score / CSAT (target: ≥4.0 out of 5)
- Comeback rate — vehicles returned for the same issue (target: 0%)
- Service accuracy rate — jobs completed correctly on first attempt

---

## Tools Used

- Tableau Desktop
- Microsoft Excel / CSV
- GitHub

---

## Dataset

`tire_shop_kpi_data.csv` contains 110 synthetic service records across January 2024 simulating a single retail tire shop location. Fields include:

- `date` — service date
- `technician_name` — assigned technician
- `service_type` — Tire Mount & Balance, Tire Rotation, or Flat Repair
- `vehicle_type` — Sedan, SUV, or Truck
- `turnaround_minutes` — actual job duration
- `on_time` — 1 if completed on time, 0 if late
- `csat_score` — customer satisfaction rating (1–5)
- `comeback` — 1 if vehicle returned for same issue
- `service_accurate` — 1 if job completed correctly on first attempt

---

## Key Insights

- **Flat Repair** had the highest CSAT (4.8 avg) and lowest comeback rate (0%), likely due to shorter job duration and clear customer expectations
- **Tire Mount & Balance** had the highest comeback rate (12%), suggesting a quality control opportunity worth investigating
- Two technicians averaged above the 60-minute target threshold on Mount & Balance jobs, indicating a coaching or process gap
- On-time rate dipped mid-month, correlating with higher Truck volume days — a staffing or scheduling signal

---

## How to View

1. Download `tire_shop_kpi_data.csv` and `tire-shop-kpi-dashboard.twbx` from this repo
2. Open the `.twbx` file in Tableau Desktop or Tableau Public (free)
3. Use the **Service Type** filter to drill into individual service categories

---

## About

Built by John Ekane — Charlotte, NC
[LinkedIn](https://linkedin.com/in/john-ekane) | jekane925@gmail.com

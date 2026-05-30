# ⛽ Fuel Savings Project

**Analysis of inbound vehicle fuel levels and cost-saving recommendations for fleet fuel purchasing.**

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Background](#background)
- [Dataset](#dataset)
- [Analysis](#analysis)
- [Key Findings](#key-findings)
- [Repository Structure](#repository-structure)
- [Tools Used](#tools-used)
- [Author](#author)

---

## Project Overview

This project analyzes the fuel levels of 100 inbound vehicles to identify patterns that can inform smarter fuel purchasing decisions. Rather than filling every vehicle to a fixed level regardless of current fuel status, a data-driven approach can eliminate unnecessary purchases and reduce overall fuel spend.

**Business Question:** How much fuel is actually needed for inbound vehicles, and what purchasing strategy minimizes cost while ensuring operational readiness?

---

## Background

Fuel management is a significant operational cost in fleet-heavy environments. A common inefficiency is purchasing a fixed volume of fuel per vehicle regardless of how much fuel the vehicle arrives with. By recording actual fuel levels at intake alongside tank capacity and vehicle make/model, it becomes possible to:

- Calculate the precise volume of fuel needed per vehicle
- Identify vehicles that arrive sufficiently fueled and require no top-off
- Estimate total fuel cost more accurately
- Recommend a purchasing threshold that balances readiness with cost efficiency

---

## Dataset

**File:** `Fuel_Data.xlsx`

The dataset was manually recorded across 100 inbound vehicles and includes the following fields:

| Field | Description |
|---|---|
| Vehicle Make/Model | Make and model of the inbound vehicle |
| Fuel Tank Capacity (gal) | Total fuel tank capacity for the vehicle |
| Fuel Level at Intake | Recorded fuel level of the vehicle upon arrival |
| Fuel Needed | Calculated volume of fuel required to reach target level |

**Collection method:** Direct observation and recording at vehicle intake  
**Sample size:** 100 vehicles  
**Format:** Microsoft Excel (.xlsx)

---

## Analysis

The analysis is visualized in `Dashboard 1.pdf`, which includes:

- **Histogram** of fuel levels at intake across all 100 vehicles, showing the distribution of how full vehicles arrive
- **Summary statistics** on fuel levels, tank capacities, and estimated fuel needed
- **Cost-saving recommendation** based on setting a fuel purchase threshold — vehicles arriving above a defined fuel level would not require a top-off, reducing unnecessary purchases

The histogram reveals the spread of arrival fuel levels and identifies the proportion of vehicles that arrive with sufficient fuel, allowing for a targeted purchasing policy rather than a blanket fill approach.

---

## Key Findings

- A meaningful portion of inbound vehicles arrive with fuel levels high enough to not require immediate refueling
- Setting a minimum fuel threshold for purchase eligibility (rather than filling all vehicles) can reduce fuel costs without impacting operational readiness
- Vehicle tank capacity varies by make/model, meaning a percentage-based threshold is more equitable than a fixed-gallon rule

> 📄 See `Dashboard 1.pdf` for the full histogram visualization and detailed cost-saving analysis.

---

## Repository Structure

```
Fuel-Savings-Project/
│
├── Fuel_Data.xlsx       # Raw data: 100 vehicles, fuel levels, tank capacities
├── Dashboard 1.pdf      # Histogram visualization and cost-saving analysis
└── README.md            # Project documentation
```

---

## Tools Used

- **Microsoft Excel** — Data collection, organization, and calculation
- **Tableau** — Dashboard and histogram visualization (exported as PDF)

---

## Author

**Matthew** — [@Bizarroxela](https://github.com/Bizarroxela)

*Part of an applied data science portfolio covering analytics, visualization, and machine learning projects.*

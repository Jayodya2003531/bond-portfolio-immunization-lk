# bond-portfolio-immunization-lk
Liability-Driven Investment using Redington Immunization — Sri Lankan Treasury Securities (FM 3015, University of Colombo)
# Liability-Adjusted Bond Portfolio Construction
### Sri Lankan Government Securities Market — A Quantitative Approach

**Course:** FM 3015 Financial Mathematics | Department of Mathematics  
**Institution:** University of Colombo | Semester I, 2026  
**Type:** Case Study 1 — First quantitative finance project

---

## Overview

This case study constructs a bond portfolio that immunizes a set of future 
insurance liabilities against interest rate risk, using real Sri Lankan 
Treasury securities data from the Ministry of Finance Primary Dealer report.

The portfolio is built using **Redington Immunization** — a classical 
liability-driven investment (LDI) framework requiring three conditions:

1. PV(assets) = PV(liabilities) — full funding
2. Duration(assets) = Duration(liabilities) — rate sensitivity matched  
3. Convexity(assets) ≥ Convexity(liabilities) — convexity cushion

**Key result:** An immunized portfolio of LKR [PV_L]M was constructed with 
Macaulay duration of [D_L] years. The surplus remained non-negative across 
all ±100 bps rate shock scenarios, confirming immunization effectiveness.

---

## Methods Used

- Macaulay Duration and Convexity calculation
- Redington immunization conditions
- Quadratic programming via Excel Solver (GRG Nonlinear)
- Sensitivity analysis (±50 bps, ±100 bps parallel yield curve shocks)
- Linear interpolation of the Sri Lankan yield curve

---

## Data Source

Sri Lankan Government Securities — Ministry of Finance Primary Dealer  
Report dated: [21/04/2026]  
Bond universe: Treasury bills (3M, 6M, 1Y) and Treasury bonds (2Y–30Y)

---

## Repository Contents

| File | Description |
|---|---|
| `CS1_[IndexNo].pdf` | Full case study report (6 pages) |
| `CS1_[IndexNo].xlsx` | Excel model — yield curve, liabilities, bond calculations, Solver |
| `yield_curve.png` | Sri Lankan government yield curve |
| `cashflow_chart.png` | Portfolio cash flows vs liability stream |
| `sensitivity_chart.png` | Surplus across ±100 bps rate scenarios |

---

## Key Results

| Metric | Value |
|---|---|
| Total PV of liabilities | $[324,426,956.01] |
| Liability Macaulay duration | [5.8828] years |
| Portfolio duration (matched) | [5.8828] years |
| Portfolio convexity | [26.3327] years² |
| Surplus at +100 bps shock | $ [324245622.78] |
| Surplus at −100 bps shock | $ [324608422.06] |

---

## Tools

Microsoft Excel (Solver Add-in) · Python (openpyxl) · Sri Lanka MoF PD Reports

---

## Skills Demonstrated

`Fixed Income` `Duration Matching` `Convexity` `Quadratic Optimization`  
`Liability-Driven Investment` `Interest Rate Risk` `Sri Lankan Capital Markets`
`Excel Solver` `Financial Modelling`

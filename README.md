# 🐟 Cointegration Analysis of Price and Quantity of Fish Export from India

> **Dissertation Project** | Kerala University of Fisheries and Ocean Studies (KUFOS), Panangad, Kochi  
> **Author:** Maneesha M (SME-2021-23-06)  
> **Guide:** Dr. Joshy C. G, Senior Scientist, ICAR – Central Institute of Fisheries Technology (CIFT), Cochin  

---

## 📌 Overview

India is one of the **top 5 fish exporting countries** in the world, with fish and fish products accounting for ~17% of agricultural exports. This study examines the **long-run equilibrium relationship** between the price and quantity of fish exported from India (1995–2023) using cointegration analysis, and forecasts export price up to **2033** using the Vector Error Correction Model (VECM).

The fish export categories analyzed include:
- Frozen Fish
- Live Fish
- Frozen Shrimp
- Frozen Squid
- Dried Fish
- Frozen Cuttlefish
- Chilled Fish
- Other Fish
- Total Fish (Aggregate)

---

## 🎯 Objectives

1. **Assess stationarity** of fish export price using the Augmented Dickey-Fuller (ADF) test
2. **Examine the long-run relationship** between fish export price and quantity using Cointegration methods
3. **Forecast fish export price** up to 2033 using the Vector Error Correction Model (VECM)

---

## 🗂️ Repository Structure

```
Cointegration-Analysis-on-Fish-Export-from-India/
│
├── 1 st Objectieve .ipynb        # ADF test for stationarity of price & quantity
├── 2 nd objectieve .ipynb        # Cointegration analysis (Engle-Granger & Johansen)
├── 3 rd obj correct.ipynb        # VECM forecasting
│
├── Frozen Fish.ipynb             # Item-wise analysis: Frozen Fish
├── frozen fish crt.ipynb         # Corrected analysis: Frozen Fish
├── Live fish.ipynb               # Item-wise analysis: Live Fish
├── Frozen Shrimp.ipynb           # Item-wise analysis: Frozen Shrimp
├── fr_squid.ipynb                # Item-wise analysis: Frozen Squid
├── Dreid fish.ipynb              # Item-wise analysis: Dried Fish
├── Fr cuttle fish.ipynb          # Item-wise analysis: Frozen Cuttlefish
├── Chilled Item.ipynb            # Item-wise analysis: Chilled Fish
├── other fish.ipynb              # Item-wise analysis: Other Fish
│
└── README.md
```

---

## 🛠️ Methodology

### 1. Unit Root Test — Augmented Dickey-Fuller (ADF)
All price and quantity series were found to be **non-stationary** at levels. After first-order differencing, all series became stationary (I(1)), confirming the prerequisite for cointegration analysis.

### 2. Cointegration Analysis
Two methods were used:

- **Engle-Granger Two-Step Procedure** — OLS regression of price on quantity, followed by ADF test on residuals to confirm cointegration.
- **Johansen Trace Test** — Used to determine the number of cointegrating vectors.

| Fish Category     | Cointegrating Vectors | Long-Run Relationship |
|-------------------|-----------------------|----------------------|
| Frozen Fish       | 1                     | ✅ Yes               |
| Live Fish         | 1                     | ✅ Yes               |
| Frozen Shrimp     | 1                     | ✅ Yes               |
| Dried Fish        | 1                     | ✅ Yes               |
| Other Fish        | 1                     | ✅ Yes               |
| Frozen Squid      | 0                     | ❌ No                |
| Frozen Cuttlefish | 0                     | ❌ No                |
| Chilled Fish      | 0                     | ❌ No                |
| Total Fish        | 0                     | ❌ No                |

### 3. Forecasting — Vector Error Correction Model (VECM)
VECM was applied to forecast price and quantity for all fish categories up to **2033**. Forecasted values exhibit an **upward trend**, consistent with increasing global demand and expanding export infrastructure.

#### Sample Forecasted Price Values (Rs. Crores)

| Year | Frozen Fish | Live Fish | Frozen Shrimp | Frozen Squid | Total Fish |
|------|------------|-----------|---------------|--------------|------------|
| 2024 | 5943.34    | 413.47    | 49458.96      | 3935.10      | 68331.01   |
| 2026 | 6452.69    | 424.82    | 58784.64      | 4147.96      | 80810.46   |
| 2028 | 6915.60    | 430.29    | 70147.48      | 4188.15      | 94916.64   |
| 2030 | 7375.38    | 432.14    | 83431.11      | 4195.74      | 111080.51  |
| 2033 | 8061.71    | 432.73    | 107719.60     | 4197.37      | 139818.54  |

---

## 📦 Requirements

```bash
pip install pandas numpy statsmodels matplotlib scipy
```

**Languages & Tools Used:**
- Python 3.x
- R (supplementary analysis)
- Jupyter Notebook
- Libraries: `statsmodels`, `pandas`, `numpy`, `matplotlib`

---

## 📊 Data Source

- **MPEDA** – Marine Products Export Development Authority: [https://mpeda.gov.in](https://mpeda.gov.in)
- **Ministry of Commerce and Industry**: [https://commerce.gov.in/trade-statistics/](https://commerce.gov.in/trade-statistics/)

**Data Coverage:** 1995–2023 | Item-wise annual export Price (Rs. Crores) and Quantity (MT)

---

## 📈 Key Findings

- All price and quantity series are **integrated of order one — I(1)**.
- **Frozen shrimp, live fish, other fish, frozen fish, and dried fish** show a stable long-run equilibrium between price and quantity.
- **Frozen squid, frozen cuttlefish, chilled fish, and total fish** do not exhibit a long-run cointegration relationship — their price and quantity fluctuations are relatively independent.
- All observed price-quantity relationships are **linear**.
- VECM forecasts indicate a **positive growth trend** in both price and quantity through 2033, driven by rising global demand and improvements in export infrastructure.

---

## 📄 Citation

If you use this work, please cite:

```
Maneesha M & Joshy C. G. (2023). A Study on Cointegration Analysis of Price and 
Quantity of Fish Export from India. Kerala University of Fisheries and Ocean Studies 
(KUFOS), Panangad, Kochi / ICAR-CIFT, Cochin.
```

---

## 📬 Contact

**Maneesha M**  
M.Sc. Statistics (Fisheries), KUFOS  
GitHub: [@maneesha1618](https://github.com/maneesha1618)

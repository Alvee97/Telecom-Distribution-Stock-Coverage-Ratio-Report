# 📊 Telecom Distribution Stock Coverage & Performance Reports

This repository contains **three Excel workbooks** used for telecom distribution reporting and performance tracking.  
Together, they provide **end-to-end visibility** into:  
- 📦 Stock Coverage Ratio (SCR) at **Distribution House (DH)** level  
- 👨‍💼 Sales execution by **Distribution Sales Representatives (DSRs)**  
- ✅ Service quality at **Point of Sale (POS)**  

---

## 📂 Files in this Repository

### 1. `DH SCR Update till 30 Jun’24 (Final).xlsb`
**Purpose:** Tracks **Stock Coverage Ratio (SCR)** for Robi & Airtel across all Distribution Houses (DHs).  

**Key Features:**
- DH-wise and DSR-wise stock coverage (days vs targets).  
- Pivot-based summaries of DH achievement.  
- Conditional formatting to flag DHs under 1.5 days of coverage.  

**Sheets Included:**
- `Summary` → Month-end SCR snapshot.  
- `Details` → Master dataset (brand, cluster, region, distributor, SCR targets).  
- `DH Wise Ach` → DH achievement vs target.  
- `DH Robi` / `DH AT` → Brand-specific DH breakdowns.  
- `DSR Robi` / `DSR AT` → Brand-specific DSR breakdowns.  

**Functions Used:** `SUMIFS()`, `INDEX-MATCH()`, `IFERROR()`, Pivot Tables, Conditional Formatting.  

---

### 2. `DSR Loc Mat Trnx SIM POS & SIM Delivery Update till 25th June’24.xlsb`
**Purpose:** Tracks **DSR (Distribution Sales Representatives)** performance on **SIM POS transactions, location match, and SIM delivery achievements**.  

**Key Features:**
- Incentive slab calculations (≥5, ≥3, ≥2 SIM deliveries).  
- Region-level leaderboards of winners.  
- RAW transaction data for transparency.  
- Automated SIM POS achievement % and incentive logic.  

**Sheets Included:**
- `Region` → Regional performance & winners.  
- `DSR` → DSR-level SIM POS & delivery achievement.  
- `RAW` → Base transaction dataset.  

**Functions Used:** `SUMIFS()`, `INDEX-MATCH()`, `IF()`, Pivot Tables, Conditional Formatting.  

---

### 3. `Quality EL POS Serve Update Till 24th June’24.xlsb`
**Purpose:** Tracks **POS service quality** across regions, DHs, and DSRs. Focus is on **4-Time Location Match (LM) Retailers** and execution quality.  

**Key Features:**
- Multi-level breakdown (Region → Area Manager → DH → DSR).  
- Quality score = % of POS outlets served according to standards.  
- Ensures POS servicing quality, not just transaction volume.  

**Sheets Included:**
- `Region` → Region-level quality POS tracking.  
- `AM` → Area Manager-level quality scores.  
- `OWN FF` → Own field force performance.  
- `DH` → Distributor-level POS service quality.  
- `DSR` → DSR-level service update.  
- `Mapping` → Supporting data mapping.  

**Functions Used:** `SUMIFS()`, `INDEX-MATCH()`, Ratios (`=Quality / Total`), Conditional Formatting.  

---

## ⚙️ Combined Reporting Flow

1. **DH SCR Report** → *Supply side visibility*  
   Tracks stock coverage days at DH & DSR level.  

2. **DSR SIM POS & Delivery Report** → *Execution & incentive visibility*  
   Tracks DSR SIM POS transactions, deliveries, and incentive slabs.  

3. **Quality EL POS Report** → *Service quality visibility*  
   Tracks how well POS outlets are being served (location match & quality scores).  

---

## 📌 Business Impact

✔️ **SCR Report** → Ensures distributors hold sufficient stock.  
✔️ **DSR SIM POS Report** → Aligns field sales reps with targets & incentives.  
✔️ **Quality EL POS Report** → Ensures service quality at POS outlets.  

Together, these three tools form a **comprehensive reporting system** for telecom distribution, linking:  
- **Supply → Execution → Service Quality.**  

---

## 🔑 Tools & Formulas Highlighted
- `SUMIFS()` → aggregate sales/deliveries.  
- `INDEX-MATCH()` / `VLOOKUP()` → map distributors, AMs, and DSRs.  
- `IFERROR()` → handle missing data.  
- `IF()` → incentive slab logic.  
- Pivot Tables → regional/DH/DSR summaries.  
- Conditional Formatting → instant performance highlights.

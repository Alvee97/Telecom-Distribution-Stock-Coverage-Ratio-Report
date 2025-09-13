# 📊 Distribution House Stock Coverage Ratio Report

This Excel workbook tracks **Stock Coverage Ratio (SCR)** for **Robi & Airtel Distribution Houses (DHs)** across regions.  
It consolidates sales, inventory, and achievement data at both **Distribution House (DH)** and **Distribution Sales Representative (DSR)** levels.

---

## 🔹 Sheets Overview

### 1. **Summary**
- **Purpose:** Provides a snapshot of distributor SCR status as of month-end.  
- **Functions/Tools Used:**
  - Linked formulas from `Details` and `DH Wise Ach` sheets.
  - Conditional formatting to flag DHs below/above target SCR (1.5 days).  
- **Details:**  
  - Shows **Robi Brand** and **Airtel Brand** side by side.  
  - Used for quick leadership review of coverage position.  

---

### 2. **Details**
- **Purpose:** Master table containing **distributor-level data**.  
- **Columns include:** Brand, Cluster, Region, Area, Distributor Name, Distributor Code, MSISDN, DH Type, SCR Targets, Actual SCR Days.  
- **Functions/Tools Used:**  
  - `SUMIFS()` to calculate sales/stock by distributor.  
  - `VLOOKUP()` / `INDEX-MATCH()` for distributor metadata.  
  - `IFERROR()` to handle missing distributor codes.  
- **Details:**  
  - Serves as the **data backbone** for all other sheets.  

---

### 3. **DH Wise Ach**
- **Purpose:** Distribution House–wise achievement vs SCR targets.  
- **Functions/Tools Used:**  
  - `Pivot Table` summarizing SCR achievement.  
  - Ratios (`=Actual/Target`) to track performance.  
- **Details:**  
  - Shows per-DH stock coverage in both value and days.  
  - Highlighted metrics indicate **under-coverage (<1.5 days)**.  

---

### 4. **DH Robi**
- **Purpose:** Robi brand-specific DH level data.  
- **Data Includes:** User name, mobile number, geography, parent hub, daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - Date-wise sales tracking (`SUMIFS()` with date criteria).  
  - Consolidation with regional hubs.  
- **Details:**  
  - Daily stock movement for Robi DHs → aggregated for SCR calculation.  

---

### 5. **DSR Robi**
- **Purpose:** Robi brand-specific **Distribution Sales Representative (DSR)** level tracking.  
- **Data Includes:** DSR name, parent distributor, owner hub, and daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - `SUMIFS()` for daily transactions.  
  - `INDEX-MATCH()` to link DSR with Distributor & Hub.  
- **Details:**  
  - Helps identify **DSR-level performance gaps**.  

---

### 6. **DH AT**
- **Purpose:** Airtel brand-specific DH level tracking.  
- **Data Includes:** Distributor names, owners, geography, and daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - Similar logic to **DH Robi** sheet.  
- **Details:**  
  - Used for Airtel’s distribution planning.  

---

### 7. **DSR AT**
- **Purpose:** Airtel brand-specific DSR level tracking.  
- **Functions/Tools Used:**  
  - Same structure as **DSR Robi**.  
- **Details:**  
  - Evaluates daily performance of each DSR under Airtel distributors.  

---

## ⚙️ Key Excel Functions Used
- `SUMIFS()` → aggregating sales/stock by distributor/date.  
- `VLOOKUP()` / `INDEX-MATCH()` → mapping distributor & DSR metadata.  
- `IFERROR()` → handling missing/mismatched data.  
- `Pivot Tables` → DH-wise & cluster-level aggregation.  
- `Conditional Formatting` → flagging low SCR.  

---

📌 **Note:**  
This file is the **master monthly reporting tool** for tracking stock coverage across Robi & Airtel Distribution Houses and their DSRs, ensuring visibility on coverage gaps.


This Excel workbook tracks **Stock Coverage Ratio (SCR)** for **Robi & Airtel Distribution Houses (DHs)** across regions.  
It consolidates sales, inventory, and achievement data at both **Distribution House (DH)** and **Distribution Sales Representative (DSR)** levels.

---

## 🔹 Sheets Overview

### 1. **Summary**
- **Purpose:** Provides a snapshot of distributor SCR status as of month-end.  
- **Functions/Tools Used:**
  - Linked formulas from `Details` and `DH Wise Ach` sheets.
  - Conditional formatting to flag DHs below/above target SCR (1.5 days).  
- **Details:**  
  - Shows **Robi Brand** and **Airtel Brand** side by side.  
  - Used for quick leadership review of coverage position.  

---

### 2. **Details**
- **Purpose:** Master table containing **distributor-level data**.  
- **Columns include:** Brand, Cluster, Region, Area, Distributor Name, Distributor Code, MSISDN, DH Type, SCR Targets, Actual SCR Days.  
- **Functions/Tools Used:**  
  - `SUMIFS()` to calculate sales/stock by distributor.  
  - `VLOOKUP()` / `INDEX-MATCH()` for distributor metadata.  
  - `IFERROR()` to handle missing distributor codes.  
- **Details:**  
  - Serves as the **data backbone** for all other sheets.  

---

### 3. **DH Wise Ach**
- **Purpose:** Distribution House–wise achievement vs SCR targets.  
- **Functions/Tools Used:**  
  - `Pivot Table` summarizing SCR achievement.  
  - Ratios (`=Actual/Target`) to track performance.  
- **Details:**  
  - Shows per-DH stock coverage in both value and days.  
  - Highlighted metrics indicate **under-coverage (<1.5 days)**.  

---

### 4. **DH Robi**
- **Purpose:** Robi brand-specific DH level data.  
- **Data Includes:** User name, mobile number, geography, parent hub, daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - Date-wise sales tracking (`SUMIFS()` with date criteria).  
  - Consolidation with regional hubs.  
- **Details:**  
  - Daily stock movement for Robi DHs → aggregated for SCR calculation.  

---

### 5. **DSR Robi**
- **Purpose:** Robi brand-specific **Distribution Sales Representative (DSR)** level tracking.  
- **Data Includes:** DSR name, parent distributor, owner hub, and daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - `SUMIFS()` for daily transactions.  
  - `INDEX-MATCH()` to link DSR with Distributor & Hub.  
- **Details:**  
  - Helps identify **DSR-level performance gaps**.  

---

### 6. **DH AT**
- **Purpose:** Airtel brand-specific DH level tracking.  
- **Data Includes:** Distributor names, owners, geography, and daily sales from 20–29 June.  
- **Functions/Tools Used:**  
  - Similar logic to **DH Robi** sheet.  
- **Details:**  
  - Used for Airtel’s distribution planning.  

---

### 7. **DSR AT**
- **Purpose:** Airtel brand-specific DSR level tracking.  
- **Functions/Tools Used:**  
  - Same structure as **DSR Robi**.  
- **Details:**  
  - Evaluates daily performance of each DSR under Airtel distributors.  

---

## ⚙️ Key Excel Functions Used
- `SUMIFS()` → aggregating sales/stock by distributor/date.  
- `VLOOKUP()` / `INDEX-MATCH()` → mapping distributor & DSR metadata.  
- `IFERROR()` → handling missing/mismatched data.  
- `Pivot Tables` → DH-wise & cluster-level aggregation.  
- `Conditional Formatting` → flagging low SCR.  

---

📌 **Note:**  
This file is the **master monthly reporting tool** for tracking stock coverage across Robi & Airtel Distribution Houses and their DSRs, ensuring visibility on coverage gaps.

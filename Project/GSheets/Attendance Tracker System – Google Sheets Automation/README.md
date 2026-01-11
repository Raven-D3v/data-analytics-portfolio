# 📊 Attendance Tracker System – Google Sheets Automation

A fully automated **Google Sheets–based Attendance Tracking System** designed to handle real-world HR policies, time rules, and payroll cut-offs — without manual computation.

This project focuses on **formula-driven automation**, ensuring accuracy, scalability, and minimal human error.

---

## 🚀 Project Overview

This Attendance Tracker was built to replace manual attendance computation with a **rule-based, automated system** using Google Sheets.

The system automatically processes:
- Time In / Time Out
- Working hours
- Late minutes
- Undertime
- Offset schedules
- Work-from-home cases
- Payroll cut-off summaries

All computations are handled using **ARRAYFORMULA-based logic**, allowing the system to scale automatically as new rows or employees are added.

---

## ⚙️ Core Automation Features

### ✅ **Automated Working Hours Calculation**
- Computes total working hours per employee
- Automatically deducts **1-hour lunch break**
- Enforces company work schedule boundaries:
  - Regular: **8:00 AM – 5:00 PM**
  - OFFSET: **9:00 AM – 6:00 PM**
- Prevents negative or invalid time results

---

### ✅ **Smart Late Detection System**
Late minutes are computed automatically based on attendance type:

| Attendance Type | Late Threshold |
|-----------------|----------------|
| Regular | After **8:15 AM** |
| OFFSET | After **9:15 AM** |
| WFH | After **8:00 AM** |

- Late minutes are calculated dynamically
- No manual tagging or calculations needed
- Supports daily, cut-off, and monthly aggregation

---

### ✅ **Policy-Based Attendance Recognition**
The system automatically detects attendance conditions using text-based rules:
- `OFFSET`
- `WFH`
- `VL` / `SL` / `ABSENT`

These entries automatically:
- Adjust working hour rules
- Exclude leave/absence days from calculations
- Apply correct late thresholds

---

### ✅ **Undertime (UT) Automation**
- Detects undertime for:
  - **AM (8:00–12:00)**
  - **PM (1:00–5:00)**
- Automatically deducts UT from total working hours
- Eliminates manual half-day checks

---

### ✅ **Cut-Off Based Summaries**
- Automatically computes **total late minutes per payroll cut-off**
  - 1st Cut-Off: **15th**
  - 2nd Cut-Off: **30th / 31st**
- No need to rewrite formulas every payroll period
- Designed to support monthly and yearly summaries

---

### ✅ **Scalable Formula Architecture**
- Built using:
  - `ARRAYFORMULA`
  - `LET`
  - `FILTER`
  - `REGEXEXTRACT`
  - `TIMEVALUE`
- Automatically applies calculations to new rows
- No dragging of formulas
- Minimal risk of human error

---

## 🧠 Automation Philosophy

This system was intentionally designed to:
- Minimize manual encoding
- Reduce formula duplication
- Enforce business rules consistently
- Scale easily as employee count grows
- Serve as a foundation for dashboards and yearly analytics

---

## 🛠 Tools & Technologies
- Google Sheets
- Advanced Spreadsheet Formulas
- Data Automation & Business Logic Modeling
- Conditional Formatting

---

## 📈 Possible Extensions
- Monthly & yearly attendance dashboards
- Employee-level performance summaries
- Payroll export integration
- Department-level attendance analytics

---

## 👤 Author
**Project Raven**  
Data & Spreadsheet Automation  
Custom Google Sheets Systems

---

## 📄 License
This project is shared for educational and portfolio purposes.

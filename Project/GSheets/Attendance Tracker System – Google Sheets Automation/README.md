# 📊 Attendance Tracker System – Google Sheets Automation

![Project Banner Screenshot](./screenshots/banner.png)

> A fully automated **Google Sheets–based Attendance Tracking System** designed to eliminate manual attendance computation, reduce human error, and enforce real-world HR policies through formula-driven automation.

---

## ❗ Problem Statement

Many small teams and growing companies rely on **manual attendance tracking** using basic spreadsheets.  
This often results in:

- Manual computation of working hours and lates
- Inconsistent enforcement of attendance policies
- High risk of human error
- Time-consuming payroll preparation
- Difficulty summarizing attendance across cut-off periods and months

As attendance data grows, these issues compound — making simple spreadsheets **unsustainable and unreliable**.

---

## ✅ Solution Overview

This project delivers a **rule-based, automated attendance system** built entirely in Google Sheets.

Instead of manual calculations, the system uses **advanced formulas and structured logic** to automatically:

- Compute working hours
- Detect lates based on policy
- Adjust schedules dynamically
- Exclude leave and absence days
- Summarize attendance per cut-off and per month

The result is a **scalable, low-maintenance attendance system** that works in real operational conditions.

---

## 🖼 Project Screenshots

> Replace these placeholders with actual images later.

![Monthly Attendance Sheet](./screenshots/monthly-sheet.png) 
![Automated Totals Section](./screenshots/automation.png)
![Cut-Off Summary](./screenshots/cutoff-summary.png)

---

## 🔗 Project Access & Demo

📄 **View-Only Google Sheet:**  
👉 `https://docs.google.com/spreadsheets/d/XXXXXXXXXXXX`

🎥 **Video Demo Walkthrough:**  
👉 `https://youtu.be/XXXXXXXXXXXX`

📸 **More Screenshots:**  
👉 `./screenshots/`

---

## 🚀 Core Automation Features

### ✅ Automated Working Hours Calculation
- Automatically computes total working hours per employee
- Deducts **1-hour lunch break** automatically
- Enforces official working schedules:
  - Regular: **8:00 AM – 5:00 PM**
  - OFFSET: **9:00 AM – 6:00 PM**
- Prevents negative or invalid results

---

### ✅ Smart Late Detection System
Late minutes are calculated automatically based on attendance type:

| Attendance Type | Late Threshold |
|-----------------|----------------|
| Regular | After **8:15 AM** |
| OFFSET | After **9:15 AM** |
| WFH | After **8:00 AM** |

- No manual tagging required
- Late minutes computed dynamically
- Supports daily, cut-off, and monthly summaries

---

### ✅ Policy-Based Attendance Recognition
The system automatically recognizes attendance conditions using text-based rules:

- `OFFSET`
- `WFH`
- `VL` / `SL` / `ABSENT`

These entries automatically:
- Adjust working hour boundaries
- Apply correct late thresholds
- Exclude non-working days from calculations

---

## 🧠 Automation-First Design

This project was designed with an **automation-first mindset**:

- Uses `ARRAYFORMULA` to auto-apply logic to new rows
- Centralized formula architecture (no dragging)
- Business rules enforced consistently
- Minimal maintenance required as data grows
- Ready foundation for dashboards and analytics

---

## 🛠 Tools & Technologies
- Google Sheets
- Advanced Spreadsheet Functions:
  - `ARRAYFORMULA`
  - `LET`
  - `FILTER`
  - `REGEXEXTRACT`
  - `TIMEVALUE`
- Conditional Formatting
- Business Logic Modeling

---

## 📈 Future Enhancements
- Interactive dashboards
- Yearly attendance summaries
- Payroll export support
- Department-level analytics

---

## 👤 Author
**Project Raven**  
Data & Spreadsheet Automation  
Custom Google Sheets Systems

---

## 📄 License
Shared for portfolio and educational purposes only.

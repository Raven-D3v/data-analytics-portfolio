# 📊 Sales Forecast & Employee Performance Dashboard  
### Centralized Sales Intelligence System Built with Google Apps Script

![Sales Dashboard Overview](screenshots/dashboard-overview.png)

---

## 📌 Overview

A lightweight **sales intelligence dashboard** built with **Google Sheets and Google Apps Script** to centralize reporting across multiple sales sheets.

The system consolidates distributed sales data into a structured dataset and presents it through interactive dashboards for **Forecast vs Actual tracking and employee performance monitoring**.

---

## 🚨 Problem

Sales reporting was fragmented across multiple sheets, requiring manual consolidation to generate reports.

This resulted in:

- Slow reporting cycles  
- Limited visibility of **Forecast vs Actual performance**  
- Manual employee performance tracking  
- Frequent cross-sheet navigation  

---

## 🛠 Solution

A centralized reporting system that:

- Aggregates sales data into a **Master Sheet using `IMPORTRANGE()`**
- Structures data into a **tabular dataset optimized for reporting**
- Uses **Google Apps Script** to process data and serve dashboards
- Displays results through **interactive charts and performance dashboards**

---

## 📊 Key Features

### Sales Dashboard

![Forecast Dashboard](screenshots/forecast-dashboard.png)

- Forecast vs Actual vs Goal tracking  
- Monthly and yearly KPI summaries  
- Chart-based performance visualization  

### Employee Performance Dashboard

![Employee Dashboard](screenshots/employee-dashboard.png)

- Quarterly quota tracking  
- Leaderboard ranking system  
- Goal completion pie charts  
- Performance percentage indicators  

---

## ⚙ Architecture

Sales Sheets  
→ `IMPORTRANGE()` Consolidation  
→ Structured Master Dataset  
→ **Google Apps Script Processing**  
→ Dashboard UI (Google Charts)

---

## 🛠 Tech Stack

- **Google Sheets** – Data storage  
- **Google Apps Script** – Backend automation & data processing  
- **HTML / JavaScript** – Dashboard UI  
- **Google Charts** – Data visualization  

---

## 📂 Project Structure


Apps Script Project
│
├── Code.gs
├── EmplDashbGS.gs
├── Dashboard.html
├── EmployeeDashboard.html
└── screenshots/


---

## 🎯 Impact

- Centralized reporting system  
- Faster monthly reporting  
- Reduced manual spreadsheet work  
- Clear employee performance visibility  

---

## 📌 Status

Implemented and ready for operational reporting.

---

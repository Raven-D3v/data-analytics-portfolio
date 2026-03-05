# 📊 Sales Forecast & Employee Performance Dashboard  
### A Centralized Sales Intelligence System Built with Google Apps Script

![Sales Dashboard Overview](screenshots/dashboard-overview.png)

---

# 📌 Overview

A custom-built **sales forecasting and employee performance reporting system** designed to replace fragmented spreadsheet reporting with a centralized intelligence dashboard.

The system consolidates sales data from multiple sheets, structures it into a normalized dataset, and presents it through interactive dashboards powered by **Google Apps Script and Google Charts**.

Instead of relying on heavy spreadsheet formulas, the platform uses **server-side Apps Script logic and a web-based UI layer** to deliver a scalable reporting workflow.

---

# 🚨 Problem

Before implementation:

- Sales data was distributed across multiple sheets
- Reporting required manual cross-referencing
- Forecast vs Actual performance visibility was limited
- Employee performance tracking required manual computation
- Monthly and quarterly reporting was time-consuming

This resulted in **slow reporting cycles and limited decision visibility**.

---

# 🛠 Solution

The system introduces a structured reporting architecture composed of:

### 1️⃣ Data Consolidation Engine

![Master Sheet Consolidation](screenshots/master-sheet-consolidation.png)

- Sales data stored across multiple input sheets
- Imported into a **centralized Master Sheet using `IMPORTRANGE()`**
- Ensures consistent data structure across all sales records
- Creates a **single source of truth**

---

### 2️⃣ Forecast & Performance Dashboard

![Forecast vs Actual Dashboard](screenshots/forecast-dashboard.png)

- Monthly and yearly **Forecast vs Actual vs Goal comparison**
- Real-time KPI summaries
- Dynamic filtering by month and quarter
- Interactive charts powered by **Google Charts**

---

### 3️⃣ Employee Performance Dashboard

![Employee Performance Dashboard](screenshots/employee-dashboard.png)

- Quarterly performance tracking per employee
- Visual **quota completion pie charts**
- Leaderboard ranking system
- Automated calculation of performance percentage vs quota

---

# ⚙ System Architecture

![System Architecture Diagram](screenshots/system-architecture.png)

The system follows a layered reporting architecture:

### Data Source Layer
Multiple independent **Sales Sheets** containing raw transactional data.

### Consolidation Layer
Data is aggregated into a centralized **Master Sheet** using:


IMPORTRANGE()


This allows the system to pull and standardize data across multiple sources.

### Transformation Layer
Imported data is normalized into a structured tabular dataset optimized for reporting and analysis.

### Application Layer (Google Apps Script)

Server-side Apps Script handles:

- Data processing and aggregation
- Quarter and month calculations
- Employee performance computations
- Ranking logic
- API-style functions used by the frontend dashboards

Key functions include:

- `getEmployeeQuarterSummary()` → Calculates quarterly employee performance
- `getEmployeeDetail()` → Returns employee monthly and quarterly metrics
- `getMonths()` → Extracts available months from the dataset
- `getEmplDashConfig()` → Retrieves system configuration (year settings)

### Visualization Layer

Interactive dashboards built with:

- **Google Apps Script HTML Service**
- **Google Charts API**

Features include:

- KPI summary cards
- Forecast vs Actual charts
- Quarterly employee quota pie charts
- Dynamic leaderboards

---

# 📊 Dashboard Features

## Main Sales Dashboard

![Main Sales Dashboard](screenshots/sales-dashboard.png)

- Forecast vs Actual tracking
- Monthly and yearly KPI summaries
- Chart-based performance visualization
- Dynamic filtering

---

## Employee Dashboard

![Employee Leaderboard](screenshots/employee-leaderboard.png)

- Quarterly quota completion charts
- Performance leaderboard
- Percent completion indicators
- Employee ranking system

---

# 🎯 Key Benefits

- Centralized reporting system
- Faster monthly and quarterly reporting
- Reduced manual spreadsheet work
- Transparent employee performance tracking
- Scalable architecture for future automation

---

# 🛠 Tech Stack

- **Google Sheets** – Data storage and management  
- **Google Apps Script** – Backend processing and automation  
- **HTML / CSS / JavaScript** – Custom dashboard UI  
- **Google Charts API** – Data visualization  

---

# 📂 Project Structure


/Apps Script Project
│
├── Code.gs
│ Core dashboard backend logic
│
├── EmplDashbGS.gs
│ Employee dashboard server functions
│
├── Dashboard.html
│ Main sales dashboard UI
│
├── EmployeeDashboard.html
│ Employee performance dashboard UI
│
└── screenshots/
├── dashboard-overview.png
├── forecast-dashboard.png
├── employee-dashboard.png
├── master-sheet-consolidation.png
├── system-architecture.png


---

# 🚀 Future Improvements

Potential enhancements include:

- Automated scheduled reporting
- Email summary reports
- Configurable employee quota system
- Role-based dashboard access
- Advanced forecasting models

---

# 📌 Implementation Status

System deployed and ready for operational reporting.

The architecture is designed to support scalable reporting workflows within the Google Workspace environment.

---

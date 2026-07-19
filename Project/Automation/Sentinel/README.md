# 📅 **SENTINEL:** License Renewal Alert System

An automated **License Renewal Alert System** that monitors software and account license expiration dates stored in **Google Sheets** and sends scheduled email notifications using **n8n**, **Google Calendar**, **Google Apps Script**, and **Gmail**.

This project was developed to eliminate manual license tracking, reduce the risk of expired subscriptions, and provide a simple, maintainable automation workflow for business users.

---

## 📌 Overview

Managing dozens (or hundreds) of software licenses manually is error-prone and time-consuming. This system automates the entire monitoring process by checking license expiry records and notifying stakeholders before licenses expire.

The solution also includes backend health logging, workflow error notifications, and a manual fallback trigger to improve reliability.

---

## ✨ Features

- 📊 Google Sheets-based license database
- 📧 Automated email notifications for expiring licenses
- 📅 Google Calendar-driven scheduling
- ⚡ Manual "Send Alert" button using Google Apps Script
- 🔄 n8n workflow automation
- 📝 Backend health logging
- 🚨 Automatic workflow error notifications
- 👥 Dynamic email recipients from Google Sheets
- 📈 Notification tracking to prevent duplicate alerts
- 🛠 Maintenance-friendly documentation

---

## 🏗 System Architecture

```text
Google Sheets
│
├── License Records
├── Email Recipients
└── Manual Send Alert
        │
        ▼
Google Apps Script
(Webhook)
        │
        ▼
      n8n
 ┌──────────────┐
 │              │
Google Calendar │
 Event Trigger  │
 │              │
 ▼              ▼
Email Alerts  Error Handler
 │              │
 ▼              ▼
Gmail       Error Notification
                │
                ▼
          Backend Log Sheet
```

---

## 🛠 Tech Stack

- **n8n**
- **Google Sheets**
- **Google Apps Script**
- **Google Calendar**
- **Gmail**
- **Render**
- **Supabase**

---

## 📂 Project Components

### 📄 Google Sheets

Acts as the primary database for:

- License records
- Expiry dates
- Notification counters
- Email recipients
- Backend logs

---

### ⚙ n8n

Responsible for:

- Reading license data
- Filtering expiring licenses
- Sending email notifications
- Logging executions
- Error handling
- Workflow automation

---

### 📅 Google Calendar

Used as the scheduling mechanism.

Instead of relying solely on cron expressions, business users can simply edit a calendar event named:

```
License Alert
```

to adjust notification schedules.

---

### 📧 Gmail

Sends:

- License renewal notifications
- Workflow error alerts

Recipients are managed dynamically from Google Sheets.

---

### 📝 Google Apps Script

Provides:

- Manual **Send Alert** button
- Webhook trigger
- Fallback execution when automation needs to be run manually

---

## 🚨 Reliability Features

This project includes several production-focused improvements:

### Backend Health Logger

A dedicated workflow runs daily to verify that the automation platform is operational.

It records:

- Timestamp
- Calendar polling status
- Event count

---

### Error Notification Workflow

Whenever an n8n workflow fails:

- An email alert is automatically sent
- Error details are logged
- Execution URL is included for debugging

---

### Manual Fallback

If scheduled automation is unavailable, users can trigger notifications directly from Google Sheets using the **Send Alert** button.

---

## 📸 Screenshots to Include

Include the following screenshots in the repository:

### 1. Google Sheets Dashboard
- License Renewal records
- Sample data
- Notification tracking columns

---

### 2. n8n Workflow
- Main License Renewal workflow
- Calendar trigger
- Email workflow
- Error notification workflow

---

### 3. Email Notification
- Sample License Renewal email
- Sample Workflow Error email

---

### 4. Backend Logs
- Google Sheets backend logging
- Error log sheet

---

### 5. Manual Send Alert
- Google Sheets custom menu/button
- Google Apps Script trigger

---

## 📈 Workflow

```text
Google Calendar Event
        │
        ▼
Google Calendar Trigger
        │
        ▼
Read Google Sheets
        │
        ▼
Filter Expiring Licenses
        │
        ▼
Generate Email
        │
        ▼
Send via Gmail
        │
        ▼
Update Notification Count
```

---

## 💡 Challenges Solved

- Reduced manual license monitoring
- Eliminated repetitive reminder emails
- Prevented duplicate notifications
- Improved automation reliability
- Added production monitoring
- Simplified maintenance for future administrators

---

## 🚀 Future Improvements

- Microsoft Teams / Slack notifications
- Dashboard for monitoring workflow health
- SMS notifications
- Multi-company support
- Configurable reminder intervals
- Analytics dashboard
- Audit trail and reporting

---

## 📚 Lessons Learned

This project provided hands-on experience in:

- Workflow automation using n8n
- Event-driven automation
- Google Workspace integration
- Error handling
- Monitoring and logging
- Production deployment
- Automation maintenance
- Workflow documentation

---

## 👨‍💻 Author

**RavenKlein T. Rubin**

BS Information Technology  
Data Analyst | Automation Developer

GitHub: https://github.com/Raven-D3v
LinkedIn: *(Add your LinkedIn profile)*

---

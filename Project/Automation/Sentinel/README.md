# 📅 SENTINEL: License Renewal Alert System

> **A production-ready automation system developed for a real client during my internship to automate license renewal monitoring and notifications.**

SENTINEL integrates **Google Sheets**, **n8n**, **Google Calendar**, **Google Apps Script**, and **Gmail** to automatically monitor software and account license expiry dates, send scheduled email alerts, and monitor workflow health.

> **Portfolio Note:** Company-specific information and business data have been anonymized to protect client confidentiality.

---

## 📌 Project Background

### Problem
The client managed license renewals through Google Sheets, requiring employees to manually monitor expiry dates and send reminder emails. As the number of licenses grew, the process became repetitive, time-consuming, and prone to human error.

### Solution
I designed and deployed **SENTINEL**, a business automation system that:

- 📊 Uses Google Sheets as the license database
- ⚙️ Automates monitoring with n8n
- 📅 Uses Google Calendar for configurable scheduling
- 📧 Sends renewal notifications via Gmail
- 🚨 Includes workflow error notifications and backend health logging
- 🔄 Supports manual execution through Google Apps Script

The solution was successfully deployed for internal business use.

---

## ✨ Key Features

- Automated license renewal email notifications
- Google Calendar-based scheduling
- Manual "Send Alert" button
- Dynamic email recipients
- Backend health logging
- Workflow error notifications
- Notification tracking
- Maintenance documentation

---

## 💼 My Role

As the sole developer during my internship, I was responsible for:

- Designing the automation architecture
- Developing the n8n workflows
- Integrating Google Workspace services
- Implementing backend monitoring and error notifications
- Writing deployment and maintenance documentation
- Deploying and testing the solution

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

- n8n
- Google Sheets
- Google Apps Script
- Google Calendar
- Gmail
- Render
- Supabase

---

## 📸 Screenshots

Include:

- Google Sheets dashboard
- Main n8n workflow
- Email notification
- Error notification
- Backend logs
- Manual "Send Alert" button

---

## 📈 Workflow

```text
Google Calendar
      │
      ▼
Read Google Sheets
      │
      ▼
Filter Expiring Licenses
      │
      ▼
Send Email via Gmail
      │
      ▼
Update Notification Count
```

---

## 🎯 Business Impact

- Reduced manual license monitoring
- Automated reminder emails
- Minimized missed renewals
- Added workflow monitoring and error alerts
- Improved long-term maintainability

---

## 🚀 Future Improvements

- Microsoft Teams / Slack integration
- SMS notifications
- Analytics dashboard
- Multi-company support
- Configurable reminder intervals

---

## 📚 Skills Demonstrated

- Workflow Automation
- Google Workspace Integration
- n8n Development
- Business Process Automation
- Error Handling & Monitoring
- Production Deployment
- Technical Documentation

---

## 👨‍💻 Author

**RavenKlein T. Rubin**

BS Information Technology  
Data Analyst | Automation Developer

GitHub: https://github.com/Raven-D3v
LinkedIn: *(Add your LinkedIn profile)*

# 📅 **SENTINEL:** License Renewal Alert System

> **A production-ready automation system developed for a real client during my internship to streamline software and account license renewal monitoring.**

SENTINEL is a business automation solution that integrates **Google Sheets**, **n8n**, **Google Calendar**, **Google Apps Script**, and **Gmail** to automatically monitor license expiration dates and notify stakeholders before licenses expire.

Rather than serving as a proof-of-concept, this system was designed, deployed, and documented for an actual business workflow to reduce manual monitoring, improve operational reliability, and minimize the risk of missed license renewals.

> **Portfolio Note:** Company-specific information, credentials, and business data have been removed or anonymized to protect client confidentiality.

---

## 📌 Project Background

This project was developed during my internship after identifying a recurring operational challenge in the client's workflow.

### The Problem
- License renewal dates were managed in Google Sheets.
- Employees had to manually monitor expiry dates and remember when to send reminder emails.
- As the number of licenses increased, the process became repetitive, time-consuming, and susceptible to human error.

---

### The Solution
I designed and implemented **SENTINEL**, an automated monitoring system that:

- 📊 Uses Google Sheets as the central license database.
- ⚙️ Monitors license records through n8n workflows.
- 📅 Uses Google Calendar as a configurable scheduling mechanism.
- 📧 Automatically sends renewal notifications through Gmail.
- 🚨 Detects workflow failures and sends error notifications.
- 📝 Records backend health logs to verify the automation is running correctly.
- 🔄 Includes a manual fallback trigger for business continuity.

The system was successfully deployed for internal use, helping automate a real business process while improving reliability and reducing manual administrative work.

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

## 💼 My Role

As the sole developer of this solution during my internship, I was responsible for:

- Designing the overall automation architecture
- Developing the n8n workflows
- Integrating Google Sheets, Gmail, Google Calendar, and Google Apps Script
- Implementing backend health logging
- Building workflow error notification and monitoring
- Writing deployment and maintenance documentation
- Deploying and testing the solution in the client's production environment

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

## 🎯 Business Impact

This solution helped the client by:

- ✅ Automating license renewal monitoring
- ✅ Eliminating repetitive manual reminder processes
- ✅ Reducing the risk of missed license renewals
- ✅ Allowing non-technical users to manage schedules through Google Calendar
- ✅ Providing backend monitoring for workflow health
- ✅ Sending automatic error notifications when automation fails
- ✅ Simplifying long-term maintenance through comprehensive documentation

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

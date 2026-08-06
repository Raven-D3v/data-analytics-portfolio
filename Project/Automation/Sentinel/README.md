# 📅 SENTINEL: License Renewal Alert System

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/94b3239edf70ed3b4723e66be9860ba32960f657/Project/Automation/Sentinel/src/SENTI_Email.png" alt="SENTINEL Banner" width="100%">
</p>

<p align="center">
  <strong>A production-ready automation system developed for a real client during my internship to automate license renewal monitoring and notifications.</strong>
</p>

---

SENTINEL integrates **Google Sheets**, **n8n**, **Google Calendar**, **Google Apps Script**, and **Gmail** to automatically monitor software and account license expiry dates, send scheduled email alerts, and monitor workflow health.

> **Portfolio Note:** Company-specific information, branding, and business data have been anonymized to protect client confidentiality.

---

# 📌 Project Background

## Problem

The client managed software and account license renewals using Google Sheets. Employees manually monitored expiry dates and sent reminder emails, making the process repetitive, time-consuming, and prone to human error.

## Solution

I designed and deployed **SENTINEL**, a business automation system that:

- 📊 Uses Google Sheets as the centralized license database
- ⚙️ Automates monitoring using n8n
- 📅 Uses Google Calendar for configurable scheduling
- 📧 Sends renewal notifications through Gmail
- 🚨 Includes workflow error notifications and backend health logging
- 🔄 Supports manual execution through Google Apps Script

The solution was successfully deployed for internal business use.

---

# 🏗️ System Architecture

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
Gmail      Backend Logs
```

---

# ✨ Key Features

- ✅ Automated license renewal email notifications
- 📅 Google Calendar-based scheduling
- 🖱️ Manual "Send Alert" button
- 👥 Dynamic email recipients
- 📊 Backend health logging
- 🚨 Workflow error notifications
- 📬 Notification tracking
- 📖 Maintenance documentation

---

# 📸 Project Preview

## 📊 Google Sheets Backend

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/04be5951cf1026f95495d4849c96fb637d4deffa/Project/Automation/Sentinel/src/SENTIL%20-%20DATA.png" alt="Google Sheets Backend" width="95%">
</p>

> **Shows:** License database, expiry dates, recipient management, and manual trigger interface.

---

## ⚙️ n8n Workflow

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/04be5951cf1026f95495d4849c96fb637d4deffa/Project/Automation/Sentinel/src/SENTI%20-%20SampWorkflow.png" alt="n8n Workflow" width="95%">
</p>

> **Shows:** Main automation workflow responsible for monitoring license renewals and sending notifications.

---

## 📧 Email Notification

<table align="center">
<tr>
<td align="center" width="70%">

**Desktop View**

<img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/dd3cd15543d615f7c35420049d43e4203fc04f6f/Project/Automation/Sentinel/src/SENTI_Email.png" alt="Desktop Email Notification" width="100%">

</td>

<td align="center" width="30%">

**Mobile View**

<img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/b00c51091a2e331001835a11f8ab36dd45ca72b8/Project/Automation/Sentinel/src/SENTIL%20-%20Email_Mob1.jpg" alt="Mobile Email Notification" width="100%">

</td>
</tr>
</table>

---

## 📈 Backend Monitoring

<p align="center">
  <img src="YOUR_MONITORING_IMAGE_LINK_HERE" alt="Backend Monitoring" width="95%">
</p>

> **Shows:** Workflow execution logs, health monitoring, and error notification system.

---

# 💼 My Role

As the **sole developer** during my internship, I was responsible for:

- Designing the automation architecture
- Developing the n8n workflows
- Integrating Google Workspace services
- Implementing backend monitoring and workflow error notifications
- Writing deployment and maintenance documentation
- Deploying, testing, and maintaining the solution

---

# 🛠️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| Automation | n8n |
| Database | Google Sheets |
| Scripting | Google Apps Script |
| Scheduling | Google Calendar |
| Notifications | Gmail |
| APIs | Google Workspace APIs |
| Monitoring | n8n Workflow Logs |

---

# 🚀 Business Impact

- Reduced repetitive manual license monitoring
- Centralized license renewal management
- Automated email reminders
- Improved workflow reliability through backend monitoring
- Minimized missed renewals caused by human error

---

# 🔒 Confidentiality Notice

This repository showcases the technical architecture and implementation approach used during a real-world internship project.

To protect client confidentiality:

- Company information has been removed.
- Business data has been anonymized.
- Sensitive workflow details have been omitted or simplified.

The project structure and automation logic remain representative of the production solution.

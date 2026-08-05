# 📅 SENTINEL: License Renewal Alert System

<p align="center">
  <img src="YOUR_IMAGE_LINK_HERE" alt="SENTINEL Banner" width="100%">
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

<p align="center">
  <img src="YOUR_ARCHITECTURE_IMAGE_LINK_HERE" alt="System Architecture" width="90%">
</p>

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
  <img src="YOUR_GOOGLE_SHEETS_IMAGE_LINK_HERE" alt="Google Sheets Backend" width="95%">
</p>

> **Shows:** License database, expiry dates, recipient management, and manual trigger interface.

---

## ⚙️ n8n Workflow

<p align="center">
  <img src="YOUR_N8N_WORKFLOW_IMAGE_LINK_HERE" alt="n8n Workflow" width="95%">
</p>

> **Shows:** Main automation workflow responsible for monitoring license renewals and sending notifications.

---

## 📧 Email Notification

<p align="center">
  <img src="YOUR_EMAIL_IMAGE_LINK_HERE" alt="Email Notification" width="75%">
</p>

> **Shows:** Sample automated renewal notification email sent to recipients.

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

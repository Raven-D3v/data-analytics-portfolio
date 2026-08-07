# 📅 SENTINEL: License Renewal Alert System

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/94b3239edf70ed3b4723e66be9860ba32960f657/Project/Automation/Sentinel/src/SENTI_Email.png" alt="SENTINEL Banner" width="100%">
</p>

<p align="center">
  <strong>A production-ready license renewal automation system designed and deployed for a real business to automate license monitoring, scheduled notifications, and workflow health reporting.</strong>
</p>

---

SENTINEL integrates **Google Sheets**, **n8n**, **Google Calendar**, **Google Apps Script**, and **Gmail** to automatically monitor software and account license expiry dates, send scheduled email alerts, and monitor workflow health.

> **Portfolio Note:** Company-specific information, branding, and business data have been anonymized for confidentiality.

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

# 📸 Solution Overview

## 📊 Google Sheets Backend

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/04be5951cf1026f95495d4849c96fb637d4deffa/Project/Automation/Sentinel/src/SENTIL%20-%20DATA.png" alt="Google Sheets Backend" width="95%">
</p>

> **Shows:** License database, expiry dates, recipient management, and manual trigger interface.

---


## 📅 Google Calendar Scheduler

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/fdbff7d0a8acdad4568b21580d29a1da7e4bc820/Project/Automation/Sentinel/src/SENTIL_Calendar.png" alt="Google Calendar Scheduler" width="95%">
</p>

> **Shows:** Google Calendar events used as configurable automation triggers. Administrators can easily adjust execution schedules by updating calendar events without modifying the automation workflow.

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

> **Shows:** Email alert notification sent on desktop and on mobile.

---

## 📈 Backend Monitoring

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/821496a29bb51bdd133434b0e25c782360ed9b41/Project/Automation/Sentinel/src/SENTIL_DailyLogs.png" alt="Backend Monitoring" width="95%">
</p>

> **Shows:** Automated daily execution logs for health monitoring.

<p align="center">
  <img src="https://github.com/Raven-D3v/data-analytics-portfolio/blob/821496a29bb51bdd133434b0e25c782360ed9b41/Project/Automation/Sentinel/src/SENTIL_WF-DailyLogs.png" alt="Backend Monitoring" width="95%">
</p>

> **Shows:** Workflow for automated health monitoring daily execution logs.

---

# 💼 My Role

As the **sole developer** of this project, I was responsible for:

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

| Before | After |
|--------|-------|
| 📋 Employees manually checked Google Sheets every day. | 🤖 SENTINEL monitors licenses automatically. |
| 👀 Expiring licenses had to be identified manually. | 🚨 Internal alerts are sent **3 months before** license expiration. |
| 📧 Staff manually notified the responsible teams. | 📬 Internal reminder emails are sent automatically. |
| ⏰ Daily monitoring was repetitive and time-consuming. | ⚙️ Scheduled automation handles the monitoring. |
| ⚠️ Missed checks could lead to missed renewals. | ✅ Early alerts reduce the risk of missed renewals. |

---

# 🔒 Confidentiality Notice

This repository showcases the technical architecture and implementation approach used during a real-world business project.

To protect confidentiality:

- Company information has been removed.
- Business data has been anonymized.
- Sensitive workflow details have been omitted or simplified.

The project structure and automation logic remain representative of the production solution.

---

## 📩 Demo Request 

If you'd like to see the system in action or walk through the architecture and workflows, feel free to reach out.

👉 **Message me for a live demo or system walkthrough.**

🌍 **[All Links & Socials](https://linktr.ee/projectRaven)**  
📧 project.raven2024@gmail.com

<p align="left">
  <a href="https://www.facebook.com/profile.php?id=61562294530876"><img src="https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white" /></a>
  <a href="https://www.instagram.com/project.raven2024"><img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/raven-klein-r-8705222b6"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white" /></a>
  <a href="https://www.tiktok.com/@project_raven2024"><img src="https://img.shields.io/badge/TikTok-%23000000.svg?logo=TikTok&logoColor=white" /></a>
  <a href="mailto:project.raven2024@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white" /></a>
</p>

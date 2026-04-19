# 🧩 EventSync  
### A System Integration Architecture for Automated Event Workflows

<p align="center">
  <img src="src/image4.png" alt="EventSync System Overview" width="600"/>
</p>

<p align="center">
  <em>System Overview: Event Creation • Registration • Payment • Attendance Validation</em>
</p>

---

## 🚀 Overview

This project is a **System Integration Architecture (SIA)** designed to solve a real operational problem: fragmented event management workflows.

Instead of building a monolithic system from scratch, this solution **connects, automates, and orchestrates existing tools** into a unified, event-driven system.

> 💡 Core Principle:  
> **“Connect, automate, and orchestrate — instead of rebuild.”**

---

<p align="center">
  <img src="src/Event Flow Image Apr 19, 2026.png" alt="System Flow Overview" width="500"/>
</p>

<p align="center">
  <em>Event-Driven System Flow: From Registration to Attendance Validation</em>
</p>

<p align="center">
  <sub>Note: This system flow diagram is AI-generated for visualization purposes.</sub>
</p>

---

## 🧠 Problem Context (Business-Level)

Most small organizations, schools, and event organizers operate using disconnected tools:

- Registration via forms or chat  
- Attendee tracking in spreadsheets  
- Manual email confirmations  
- Payment instructions sent manually  

### ❌ Root Problem  
The issue is **not lack of tools** — it is the **lack of integration between them**.

### ⚠️ Operational Impact

- Broken workflows across systems  
- Repetitive manual processes  
- Data inconsistencies and duplication  
- Poor attendee experience  

---

## 💡 Solution: Integration-First System Design

This project introduces a **cohesive system architecture** that:

- Integrates multiple tools into a single workflow  
- Automates event-driven processes  
- Maintains a **single source of truth**  
- Eliminates manual coordination between systems  

> ✅ The system does not replace tools — it **connects and orchestrates them**

---

## 🏗️ System Architecture

This system follows an **event-driven integration model**, where each action triggers automated workflows across layers.

### 🔄 High-Level Flow

1. Event is created → stored in the system  
2. Attendee submits registration  
3. System validates and processes input  
4. Orchestration engine triggers workflows:
   - Sends confirmation email  
   - Generates Participant ID  
   - Injects dynamic payment instructions  
5. Payment is verified → system updates status  
6. Attendance is validated in real-time using system data  

---

## ⚙️ Architecture Layers & Rationale

---

### 🧩 1. Data Layer — Google Sheets

<p>
  <img src="src/image3.png" alt="Google Sheets Data Layer Overview" width="400"/>
</p>

**Role:** Centralized data layer (Single Source of Truth)

**Manages:**
- Events  
- Attendees  
- Payments  
- System state tracking  

**Why this exists:**

Google Sheets was chosen as the data layer because it is already the primary tool used by event managers.

- Real-time collaborative database behavior
- Aligns with current tools already used in event operations  
- No backend infrastructure required  
- Accessible to non-technical users  
- Fast iteration and deployment  

> 📌 Lightweight data layer enabling rapid system development

---

### 🔧 2. Logic & API Layer — Google Apps Script

**Role:** Serverless backend / middleware layer

**Handles:**
- Data validation and processing  
- Participant ID generation  
- Event creation logic  
- API-like system interactions  

**Why this exists:**
- Bridges frontend input and automation layer  
- Eliminates need for traditional backend systems  
- Enables structured business logic inside the ecosystem  

> 📌 Middleware layer enabling business logic execution without infrastructure overhead

---

### 🔁 3. Orchestration Layer — n8n (Core Engine)

**Role:** Central workflow orchestration engine

> ⚠️ Not just automation — this is the **system brain**

**Handles:**
- Event-driven workflows  
- Email confirmation pipelines  
- Payment instruction automation  
- Cross-system coordination  

**Why this exists:**
- Decouples system logic from data layer  
- Enables scalable workflow design  
- Centralizes system behavior control  

> 📌 Orchestration layer connecting all system components into one automated flow

---

### 🌐 4. Input Layer — Lightweight Interface

<p>
  <img src="src/image2.png" alt="Google Sheets Data Layer Overview" width="400"/>
</p>

**Role:** User interaction layer

**Handles:**
- Event creation  
- Attendee registration  
- Payment submission  
- Attendance validation  

**Design Philosophy:**
- Functional over aesthetic complexity  
- Optimized for usability and speed  

> 📌 Minimal interface designed for efficient system input

---

---

## 🔐 Access Control & Role-Based System Design

This system implements a **multi-level administrative architecture**:

| Level | Role | Responsibility |
|------|------|----------------|
| Level 4 | Master Admin | System-wide control, event creation, data management |
| Level 3 | Event Manager | Manages specific events and attendees |
| Level 2 | Finance/Admin | Payment verification and configuration |
| Level 1 | Gatekeeper | Attendance validation during events |

### 🎯 Why this matters

- Prevents unauthorized system changes  
- Mirrors real-world organizational workflows  
- Enables delegation of responsibilities  
- Supports scalable operations  

---

## 🆔 Participant Identity Management

<p align="center">
  <img src="src/image13.png" alt="Email Confirmation with Participant ID" width="400"/>
</p>

- Unique Participant IDs are auto-generated  
- Serves as system-wide identifier  
- Used for registration, payment, and attendance tracking  

---

## 💳 Payment Processing Flow

<p align="center">
  <img src="src/image8.png" alt="Email Confirmation with Participant ID" width="400"/>
</p>

- Payment instructions dynamically configured per event  
- Attendees submit proof of payment  
- Admin verifies transactions  
- System updates payment status in real-time  

> 💡 Enables structured financial tracking without external payment systems

---

## 🎟️ Real-Time Attendance Validation

<p align="center">
  <img src="src/image7.png" alt="Email Confirmation with Participant ID" width="400"/>
</p>

- Participant ID is verified  
- Payment status is checked  
- Access granted if both conditions are valid  

> 📌 Rule-based validation system powered by live system data

---

## 🔗 System Integration Flow (Detailed)

| Step | Layer | Action |
|------|------|--------|
| 1 | Input Layer | User submits event/registration |
| 2 | Data Layer | Data stored in Google Sheets |
| 3 | Logic Layer | Validation + ID generation |
| 4 | Orchestration Layer | n8n triggers workflows |
| 5 | Output | Email + payment instructions sent |
| 6 | Data Layer | Payment status updated |
| 7 | Input Layer | Attendance validated in real-time |

---

## 🔄 Core System Logic

### 🆔 Identity System
- Participant ID acts as universal system key  
- Links registration, payment, and attendance  

### 💳 Payment System
- Dynamic payment configuration per event  
- Admin-controlled verification workflow  

### 🎟️ Attendance System
- Real-time validation using system state  
- Gate access based on rule checks  

---

## ✅ Current Features (MVP Scope)

- Event Creation System  
- Attendee Registration System  
- Automated Email Confirmation  
- Participant ID Generation  
- Payment Configuration per Event  
- Payment Verification Workflow  
- Real-Time Attendance Validation  

---

## 🧠 Architecture Decisions & Tradeoffs

### ⚖️ No Traditional Backend
- ❌ Less scalable  
- ✅ Faster development  
- ✅ Lower complexity  
- ✅ Accessible for non-engineers  

### ⚖️ Use of n8n Orchestration
- ❌ Added system complexity  
- ✅ Enables scalable automation  
- ✅ Decouples workflows  

### ⚖️ Event-Driven Architecture
- ❌ Requires structured data flow  
- ✅ Eliminates manual coordination  
- ✅ Enables automation at scale  

---

## 📈 Business Value

- ⚡ Reduced manual workload  
- 📊 Centralized and consistent data  
- 🔁 Reliable automated workflows  
- 😊 Improved user experience  
- 🧩 Scalable event operations  

---

## 🚧 MVP Constraints

- No overengineering  
- Focus only on core workflows  
- Designed for rapid deployment  

> 💡 Built as a **functional system, not a theoretical prototype**

---

## 🏁 Conclusion

EventSync demonstrates how **system integration and orchestration** can replace traditional development-heavy approaches.

Instead of building everything from scratch, this system proves that:

> **Real-world systems can be built by connecting tools intelligently, not reinventing them.**

---

<p align="center">
  <strong>Built with a System Architect mindset — not just a developer mindset.</strong>
</p>

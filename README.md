# 🚗 Vehicle Service Management Application

<p align="center">

### A Pega-powered solution for streamlined, automated vehicle service management

**Pega National Internship Program — Capstone Project**

</p>

<p align="center">

![Pega](https://img.shields.io/badge/Pega-Platform-00A9E0?style=for-the-badge\&logo=pega)
![App Studio](https://img.shields.io/badge/Pega-App%20Studio-0070C0?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)
![Internship](https://img.shields.io/badge/Pega%20NIP-Capstone-orange?style=for-the-badge)

</p>

---

## 📌 Project Overview

The **Vehicle Service Management Application** is a workflow-driven application developed using **Pega Platform App Studio** as part of the **Pega National Internship Program**.

The application is designed for **Urban Fleet Operations** to replace traditional service-request methods such as manual phone calls, emails, and unstructured communication with a centralized digital workflow.

It enables customers and service teams to manage the complete vehicle servicing lifecycle — from **service request submission and vehicle inspection to estimate approval, service execution, and final resolution**.

### 🎯 Project Goal

> Build a structured and automated vehicle service management system that improves service request tracking, operational visibility, customer approval handling, and overall service efficiency.

---

## ✨ Key Features

* 🚘 **Vehicle Service Request Intake**
* 🔍 **Vehicle Inspection Management**
* 📝 **Inspection Notes & Required Services**
* 💰 **Service Estimate Generation**
* 👤 **Customer Approval Workflow**
* 🗃️ **Customer & Vehicle Data Management**
* 📚 **Service History Tracking**
* 🔄 **Automated Case Routing**
* ✅ **End-to-End Service Lifecycle Management**
* 📊 **Case Status & Resolution Tracking**

---

## 🏢 Application Details

| Property                    | Details                                |
| --------------------------- | -------------------------------------- |
| **Program**                 | Pega National Internship Program       |
| **Project**                 | Vehicle Service Management Application |
| **Platform**                | Pega Platform                          |
| **Development Environment** | Pega App Studio                        |
| **Target Organization**     | Urban Fleet Operations                 |
| **Application Name**        | `NIP-VehicleService-Divyadharshini`    |
| **Case Type**               | `Vehicle Service Request`              |
| **Project Status**          | ✅ Completed                            |

---

# 🧩 User Stories Implemented

The application was developed based on six major user stories covering the complete vehicle service lifecycle.

## US-001 — Submit Vehicle Service Request

Customers can initiate a vehicle service request by providing relevant information such as:

* Customer details
* Vehicle details
* Reported vehicle issues
* Preferred service date
* Service-related requirements

This creates a structured **Vehicle Service Request case** instead of relying on manual email or phone-based communication.

---

## US-002 — Perform Vehicle Inspection

Service advisors can assess the vehicle and record inspection information.

The inspection stage supports:

* Vehicle inspection notes
* Identifying service requirements
* Recording recommended maintenance
* Capturing issues discovered during inspection

### Example Services

* Brake pad replacement
* Engine oil change
* General vehicle maintenance

---

## US-003 — Generate Service Estimate

After inspection, the service team can prepare the estimated service information.

The application supports:

* Service cost calculation
* Estimated completion date
* Service-related estimate information

This provides customers with structured information before service execution begins.

---

## US-004 — Approve Service Estimate

A dedicated customer approval stage is incorporated into the workflow.

The customer reviews the generated service estimate before the service proceeds.

### Approval Flow

```text
Service Estimate
       │
       ▼
Customer Review
       │
   ┌───┴────┐
   │        │
Approve   Decision
   │
   ▼
Service Execution
```

During testing, an unnecessary **Decline branch and connector** caused a routing issue. The redundant branch was removed and the approval flow was corrected.

---

## US-005 — Maintain Vehicle Data

The application maintains structured information related to:

### 👤 Customer

* Customer profile
* Contact information
* Service-related information

### 🚘 Vehicle

* Vehicle information
* Vehicle model
* Service requirements

### 📚 Service History

Previous service information can be associated with the vehicle and customer throughout the case lifecycle.

This provides a more organized approach to maintaining vehicle service information.

---

## US-006 — Review & Resolution

The final user story connects the different stages of the service lifecycle through automated case routing.

The application moves the case through the required stages until service completion and resolution.

---

# 🔄 End-to-End Workflow

The complete application workflow is:

```text
┌─────────────────────────┐
│   Request Intake        │
│                         │
│ Customer submits        │
│ service request         │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│   Service Assessment    │
│                         │
│ Vehicle inspection &   │
│ service identification │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│   Service Estimate      │
│                         │
│ Cost & completion       │
│ estimate generated      │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│   Customer Approval     │
│                         │
│ Estimate reviewed       │
│ and approved            │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│   Service Execution     │
│                         │
│ Required service        │
│ activities completed    │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Completion & Resolution │
│                         │
│ Case finalized          │
└─────────────────────────┘
```

### 🔁 Case Lifecycle

**Request Intake → Service Assessment → Customer Approval → Service Execution → Completion & Resolution**

---

# 🏗️ Application Architecture

The application follows a case-based workflow architecture using Pega Platform.

```text
                    ┌─────────────────────┐
                    │       Customer      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Vehicle Service     │
                    │ Request Case        │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
        Request Intake   Service Assessment   Estimate
              │                │                │
              └────────────────┼────────────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Customer Approval   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Service Execution   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Completion &        │
                    │ Resolution          │
                    └─────────────────────┘
```

---

# 🛠️ Technology Stack

| Technology               | Purpose                                       |
| ------------------------ | --------------------------------------------- |
| **Pega Platform**        | Application development & workflow automation |
| **Pega App Studio**      | Low-code application development              |
| **Pega Case Management** | Service request lifecycle                     |
| **Pega Workflow**        | Automated routing between stages              |
| **Pega Data Model**      | Customer, vehicle & service information       |
| **GitHub**               | Project repository & version management       |

---

# 🔍 Testing & Debugging

Testing was performed to validate the complete service request lifecycle.

## 🧪 End-to-End Test Case

**Test Case:** `V-1013`

The test verified that a vehicle service request successfully moved through the complete workflow:

```text
Request Intake
      ↓
Service Assessment
      ↓
Customer Approval
      ↓
Service Execution
      ↓
Completion & Resolution
```

### ✅ Final Result

The test case successfully completed the complete lifecycle and reached:

```text
RESOLVED-UNSPECIFIED
```

---

# 🐛 Issue Identified & Resolved

During testing, a routing issue was identified in the customer approval stage.

### Problem

An unnecessary **Decline branch and connector** was present in the approval flow, resulting in incorrect routing behavior.

### Resolution

The redundant branch and connector were removed and the workflow was retested.

### Result

✅ Approval routing worked correctly
✅ Case progressed to the next stage
✅ End-to-end lifecycle completed successfully

This debugging process helped validate the reliability of the configured workflow.

---

# 📊 Project Outcomes

The completed application demonstrates how a manual vehicle servicing process can be transformed into a structured digital workflow.

### Key Outcomes

* ✅ Centralized service request management
* ✅ Structured vehicle and customer information
* ✅ Automated case progression
* ✅ Standardized inspection process
* ✅ Transparent service estimates
* ✅ Customer approval before service execution
* ✅ Improved service history organization
* ✅ End-to-end case tracking
* ✅ Successful workflow testing and debugging

---

# 📸 Application Screenshots

> Add screenshots of your Pega application here to make the repository more visually attractive.

### 🏠 Application / Case Dashboard

screenshots/US-001-Submit-Service-Request.png

### 📝 Vehicle Service Request

```text
screenshots/US-001-Submit-Service-Request.png
```

### 🔍 Vehicle Inspection

```text
[ Add Screenshot Here ]
```

### 💰 Service Estimate

```text
[ Add Screenshot Here ]
```

### ✅ Customer Approval

```text
[ Add Screenshot Here ]
```

### 🎯 Case Resolution

```text
[ Add Screenshot Here ]
```

---

# 📁 Project Structure

```text
NIP-VehicleService-Divyadharshini/
│
├── README.md
│
├── Application/
│   ├── Case Types
│   ├── Data Models
│   ├── Workflows
│   └── UI Configuration
│
├── Documentation/
│   ├── Project Details
│   ├── User Stories
│   └── Testing
│
└── Screenshots/
    ├── Request-Intake.png
    ├── Inspection.png
    ├── Estimate.png
    ├── Approval.png
    └── Resolution.png
```

---

# 🚀 Future Enhancements

The application can be further enhanced with additional capabilities such as:

* 📱 Customer self-service portal
* 🔔 Automated SMS/email notifications
* 💳 Online service payment integration
* 📅 Service appointment scheduling
* 📊 Fleet maintenance dashboards
* 📈 Service analytics and reporting
* 🤖 AI-based maintenance recommendations
* 🔧 Predictive vehicle maintenance
* 📍 Service center tracking
* ⭐ Customer feedback and service ratings

---

# 🎓 Internship Learning Outcomes

This capstone project provided practical exposure to:

* Pega Platform application development
* Low-code application design
* Case lifecycle management
* Workflow configuration
* Data modeling
* Approval routing
* Case status management
* Application testing
* Debugging workflow issues
* End-to-end business process automation

---

# 🔗 Project Repository

The source/project repository is available on GitHub:

**Repository:**
https://github.com/divyadharshini2028/NIP-VehicleService-Divyadharshini

---

# 🏁 Project Status

<p align="center">

### ✅ CAPSTONE PROJECT COMPLETED

**Pega National Internship Program**

**Vehicle Service Management Application**

</p>

---

## 👩‍💻 Developer

**Divyadharshini**

🎓 **B.Tech – Artificial Intelligence and Data Science**

🎓 **Bannari Amman Institute of Technology**

### 💻 Passionate About

* 🤖 Artificial Intelligence
* 📊 Data Science
* ⚡ Low-Code Development
* 🔄 Workflow Automation
* 🧠 Intelligent Applications

---

<div align="center">

## ⭐ Thank You for Visiting This Project!

### 🚗 Transforming Vehicle Service Management Through Intelligent Workflow Automation

**Built with ❤️ using Pega Platform**

⭐ **If you found this project interesting, consider giving the repository a star!** ⭐

</div>

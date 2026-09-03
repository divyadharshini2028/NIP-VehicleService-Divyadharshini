# 🚗 Vehicle Service Management Application

<div align="center">

### 🚀 An Intelligent Digital Solution for Streamlining Vehicle Service Operations

**Built with Pega Platform (App Studio)**

[![Pega Platform](https://img.shields.io/badge/Platform-Pega-blue?style=for-the-badge)](https://www.pega.com/)
[![Internship](https://img.shields.io/badge/Program-Pega%20National%20Internship%20Program-orange?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)]()

---

**👩‍💻 Developed by Divyadharshini**

</div>

---

## 📌 Project Overview

The **Vehicle Service Management Application** is a digital workflow automation solution developed as part of the **Pega National Internship Program**.

The application is designed for **Urban Fleet Operations** to replace traditional manual vehicle service requests made through **emails and phone calls** with a structured, automated, and trackable digital workflow.

Using the **Pega Platform App Studio**, the application enables efficient management of vehicle service requests from initial request submission through inspection, service estimation, customer approval, service execution, and final resolution.

---

## 🎯 Problem Statement

Traditional vehicle service management often relies on manual communication methods such as:

* 📧 Email requests
* 📞 Phone calls
* 📝 Manual tracking
* ❌ Limited service visibility
* ❌ Difficulty tracking request progress
* ❌ Delays in approvals and service execution

These manual processes can lead to inefficiencies, communication gaps, and difficulties in monitoring the complete service lifecycle.

### 💡 Solution

The Vehicle Service Management Application provides a centralized and automated workflow that enables users to:

✔ Submit service requests digitally
✔ Track vehicle inspection activities
✔ Generate service estimates
✔ Obtain customer approval
✔ Execute required services
✔ Monitor requests throughout their lifecycle
✔ Automatically route cases between service stages

---

# 🏢 Target Organization

### **Urban Fleet Operations**

The application is designed to support organizations managing vehicle fleets by improving the efficiency, visibility, and automation of vehicle service operations.

---

# 🛠️ Technology Stack

| Technology                       | Usage                                     |
| -------------------------------- | ----------------------------------------- |
| 🟦 **Pega Platform**             | Application Development Platform          |
| 🎨 **Pega App Studio**           | Low-Code Application Development          |
| 🔄 **Case Management**           | Managing Vehicle Service Requests         |
| ⚙️ **Workflow Automation**       | Automating Service Processes              |
| 🗂️ **Data Modeling**            | Managing Vehicle and Customer Information |
| 🧭 **Case Lifecycle Management** | Tracking Service Request Progress         |

---

# 🏗️ Application Details

| Property                    | Details                             |
| --------------------------- | ----------------------------------- |
| **Application Name**        | `NIP-VehicleService-Divyadharshini` |
| **Case Type**               | `Vehicle Service Request`           |
| **Platform**                | Pega Platform                       |
| **Development Environment** | App Studio                          |
| **Target Organization**     | Urban Fleet Operations              |
| **Project Type**            | Capstone Project                    |
| **Program**                 | Pega National Internship Program    |

---

# 🔄 Application Workflow

The Vehicle Service Request follows a structured lifecycle from request creation to final resolution.

```text
┌─────────────────────┐
│   Request Intake    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Service Assessment  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Customer Approval   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  Service Execution  │
└──────────┬──────────┘
           │
           ▼
┌──────────────────────────┐
│ Completion & Resolution  │
└──────────────────────────┘
```

---

# ✨ Implemented User Stories

## 📝 US-001: Submit Vehicle Service Request

Customers can submit vehicle service requests through a structured digital intake process.

### Features

* 🚗 Capture vehicle details
* 📝 Record reported issues
* 📅 Select preferred service dates
* 📩 Create a structured service request

---

## 🔍 US-002: Perform Vehicle Inspection

Service advisors can inspect the vehicle and document the required service activities.

### Features

* 🔎 Perform vehicle inspection
* 📝 Capture inspection notes
* 🛠️ Identify required services
* 🚗 Record maintenance requirements

### Example Services

* Brake pad replacement
* Oil changes
* Other required vehicle maintenance

---

## 💰 US-003: Generate Service Estimate

The application enables service advisors to generate estimates for the required vehicle services.

### Features

* 💵 Configure service cost
* 📅 Provide estimated completion date
* 📊 Maintain service estimate information

---

## ✅ US-004: Approve Service Estimate

Before service execution begins, the generated estimate is routed for customer approval.

### Features

* 👤 Single-level customer approval
* 🔄 Automated approval routing
* ✅ Approval before service execution

This ensures that service work proceeds only after the required customer approval.

---

## 🗂️ US-005: Maintain Vehicle Data

The application maintains structured information throughout the case lifecycle.

### Data Managed

* 👤 Customer profiles
* 🚗 Vehicle information
* 🚘 Vehicle models
* 📜 Service history

This improves information accessibility and supports better service management.

---

## 🏁 US-006: Review & Resolution

The application automatically routes the Vehicle Service Request through all lifecycle stages until the service process is completed.

### Features

* 🔄 Automated case routing
* 📍 Lifecycle-based progress tracking
* 🏁 Final service execution
* ✅ Case resolution

---

# 🔁 Complete Case Lifecycle

```text
Customer
   │
   ▼
Submit Vehicle Service Request
   │
   ▼
Service Assessment
   │
   ▼
Vehicle Inspection
   │
   ▼
Generate Service Estimate
   │
   ▼
Customer Approval
   │
   ▼
Service Execution
   │
   ▼
Completion
   │
   ▼
Case Resolution
```

---

# 🧪 Testing & Validation

The application was tested to verify the complete end-to-end workflow.

## 🔧 Approval Flow Debugging

During testing, a routing issue was identified in the approval process.

### Issue

A redundant **Decline branch and connector** affected the approval flow routing.

### Resolution

The unnecessary branch and connector were removed, allowing the case to proceed correctly through the workflow.

✅ Approval routing successfully resolved.

---

# 🧪 End-to-End Test Case

### Test Case ID: `V-1013`

The complete Vehicle Service Request lifecycle was successfully tested.

### Verified Lifecycle

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

### Final Status

```text
RESOLVED-UNSPECIFIED
```

✅ The case successfully transitioned through all lifecycle stages.

---

# 📊 Key Features

✨ **Structured Digital Service Requests**
Replaces manual email and phone-based requests.

🔄 **Automated Workflow Routing**
Automatically moves cases through the required service stages.

🔍 **Vehicle Inspection Management**
Captures inspection details and required maintenance.

💰 **Service Estimate Generation**
Records service costs and estimated completion dates.

✅ **Customer Approval Workflow**
Ensures approval before service execution.

🗂️ **Centralized Data Management**
Maintains customer, vehicle, and service history information.

📈 **Improved Service Visibility**
Provides better tracking throughout the service lifecycle.

🏁 **Automated Resolution**
Guides cases through completion and final resolution.

---

# 🎯 Project Objectives Achieved

| Objective                             | Status      |
| ------------------------------------- | ----------- |
| Automate Vehicle Service Requests     | ✅ Completed |
| Replace Manual Communication          | ✅ Completed |
| Implement Vehicle Inspection Workflow | ✅ Completed |
| Generate Service Estimates            | ✅ Completed |
| Implement Customer Approval           | ✅ Completed |
| Maintain Vehicle Data                 | ✅ Completed |
| Automate Case Routing                 | ✅ Completed |
| Complete End-to-End Testing           | ✅ Completed |
| Successfully Resolve Cases            | ✅ Completed |

---

# 📈 Business Benefits

The application provides several benefits to Urban Fleet Operations:

### ⚡ Improved Operational Efficiency

Automation reduces dependency on manual communication and tracking.

### 👀 Better Visibility

Users can monitor service requests throughout the complete lifecycle.

### 🔄 Standardized Workflow

Every service request follows a structured and consistent process.

### 📊 Improved Data Management

Customer and vehicle information is maintained in a centralized workflow.

### ⏱️ Faster Processing

Automated routing helps reduce delays between service stages.

### ✅ Controlled Approvals

Service execution can proceed through the configured customer approval process.

---

# 🚀 Project Outcome

The **Vehicle Service Management Application** successfully demonstrates how **Pega's low-code platform and case lifecycle management capabilities** can be used to automate real-world business processes.

The project transformed a traditionally manual vehicle service request process into a structured digital application with:

* Automated workflows
* Case lifecycle management
* Data management
* Service estimation
* Customer approval
* End-to-end testing
* Automated resolution

---

# 🔗 Project Repository

💻 **GitHub Repository**

[NIP-VehicleService-Divyadharshini on GitHub](https://github.com/divyadharshini2028/NIP-VehicleService-Divyadharshini?utm_source=chatgpt.com)

---

# 🎓 Program

**Pega National Internship Program**

This project was developed and completed as part of the internship capstone experience using the **Pega Platform and App Studio**.

---

# 📦 Project Submission

The project was successfully submitted through the required platforms.

### ✅ University Submission

* Project template submitted through the University Google Form
* Application details provided before the deadline

### ✅ Skill Wallet Platform

* Project progress updated to **100%**
* Live Pega application instance linked
* Public GitHub repository linked

---

# 👩‍💻 Developer

### **Divyadharshini**

**B.Tech – Artificial Intelligence and Data Science**

🎓 Bannari Amman Institute of Technology

💻 Passionate about:

* Artificial Intelligence
* Data Science
* Low-Code Development
* Workflow Automation
* Intelligent Applications

---

<div align="center">

## ⭐ Thank You for Visiting This Project!

### 🚗 Transforming Vehicle Service Management Through Intelligent Workflow Automation

**Built with ❤️ using Pega Platform**

⭐ *If you found this project interesting, consider giving the repository a star!*

</div>

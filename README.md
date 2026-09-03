# Vehicle Service Management Application

> **A workflow automation solution developed using Pega Platform as part of the Pega National Internship Program.**

![Project Status](https://img.shields.io/badge/Project-Completed-success)
![Platform](https://img.shields.io/badge/Platform-Pega-blue)
![Environment](https://img.shields.io/badge/Environment-App%20Studio-orange)
![Program](https://img.shields.io/badge/Program-Pega%20National%20Internship%20Program-purple)

---

## Project Overview

The **Vehicle Service Management Application** is a workflow automation solution developed as part of the **Pega National Internship Program**.

The application is designed for **Urban Fleet Operations** to replace traditional manual vehicle service requests made through emails and phone calls with a structured, automated, and trackable digital workflow.

Using the **Pega Platform and App Studio**, the application manages the complete vehicle service request lifecycle from initial request submission through inspection, service estimation, customer approval, service execution, and final resolution.

### Key Improvements

- Request tracking
- Service visibility
- Workflow automation
- Operational efficiency
- Structured data management

---

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Application Details](#application-details)
- [Key Features](#key-features)
- [Implemented User Stories](#implemented-user-stories)
- [Complete Case Lifecycle](#complete-case-lifecycle)
- [Technology Stack](#technology-stack)
- [Testing and Debugging](#testing-and-debugging)
- [End-to-End Testing](#end-to-end-testing)
- [Application Preview](#application-preview)
- [Project Outcomes](#project-outcomes)
- [Business Benefits](#business-benefits)
- [Submission Status](#submission-status)
- [Developer](#developer)

---

# Problem Statement

Traditional vehicle service management often depends on manual communication methods such as:

- Email requests
- Phone calls
- Manual tracking of service requests

These manual processes can result in:

- Limited request visibility
- Difficulty tracking service progress
- Communication delays
- Inefficient workflow management
- Lack of a structured end-to-end service process

---

# Solution

The **Vehicle Service Management Application** provides a centralized and automated workflow for managing vehicle service requests.

The application enables users to:

- Submit vehicle service requests digitally
- Capture vehicle details
- Record reported vehicle issues
- Select preferred service dates
- Perform vehicle inspections
- Capture inspection notes
- Identify required services
- Generate service estimates
- Capture estimated completion dates
- Route service estimates through customer approval
- Execute vehicle services
- Maintain customer and vehicle information
- Track requests throughout the complete lifecycle
- Automatically route cases between lifecycle stages
- Complete and resolve vehicle service requests

---

# Application Details

| Property | Details |
|---|---|
| **Application Name** | `NIP-VehicleService-Divyadharshini` |
| **Case Type** | `Vehicle Service Request` |
| **Platform** | Pega Platform |
| **Development Environment** | Pega App Studio |
| **Target Organization** | Urban Fleet Operations |
| **Program** | Pega National Internship Program |
| **Project Status** | Completed |

---

# Key Features

### Digital Service Request Management

Vehicle service requests can be submitted through a structured digital workflow instead of relying on manual email and phone communication.

### Vehicle Inspection

Service advisors can inspect vehicles, record inspection notes, and identify required services.

### Service Estimation

The application supports service cost calculation and estimated completion date management.

### Customer Approval Routing

Service estimates follow a configured customer approval workflow before proceeding to service execution.

### Structured Data Management

The application maintains structured information related to customers, vehicles, vehicle models, and service history.

### Automated Case Routing

Cases are automatically routed through the configured lifecycle stages until final completion and resolution.

---

# Implemented User Stories

## US-001: Submit Vehicle Service Request

Built an intake form that allows customers to raise vehicle service requests.

### The intake process captures:

- Vehicle details
- Reported issues
- Preferred service dates

---

## US-002: Perform Vehicle Inspection

Enabled service advisors to inspect vehicles and capture inspection information.

### Features include:

- Vehicle inspection
- Inspection notes
- Identification of required services

### Examples of services include:

- Brake pad replacement
- Oil changes

---

## US-003: Generate Service Estimate

Configured fields for:

- Service cost calculation
- Estimated completion date

This allows the service team to prepare and manage estimates for required vehicle services.

---

## US-004: Approve Service Estimate

Implemented a **single-level customer approval routing step** before service execution.

The purpose is to ensure that the service estimate follows the configured customer approval workflow before the case proceeds to service execution.

---

## US-005: Maintain Vehicle Data

Created structured data models to maintain important information throughout the case lifecycle.

The application manages:

- Customer profiles
- Vehicle information
- Vehicle models
- Service history

---

## US-006: Review & Resolution

Configured automatic routing across all case lifecycle stages.

The workflow proceeds through the required stages, including service execution, completion, and final case resolution.

---

# Complete Case Lifecycle

```text
┌─────────────────────────────┐
│       REQUEST INTAKE        │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│     SERVICE ASSESSMENT      │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│     CUSTOMER APPROVAL       │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│     SERVICE EXECUTION       │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│  COMPLETION & RESOLUTION    │
└─────────────────────────────┘

# Blood Bank Management System

A web-based application for managing blood donations, donor records, blood inventory, blood requests, and blood issuance in a centralized system.

The aim of the project is to make blood bank operations easier to manage by reducing dependence on scattered records and providing a clear way to track donors, donations, available blood stock, requests, and issued blood.

---

## Overview

The Blood Bank Management System brings together the main activities involved in managing a blood bank.

Blood bank staff can register donors, record donations, monitor available blood stock, track expiry information, process blood requests, and issue blood when suitable stock is available.

Hospitals or other authorized requesting organizations can check blood availability, submit blood requests, and track the status of their requests.

Administrators oversee system access and reporting.

---

## Main Features

- Donor registration and donor record management
- Donation recording and donation history
- Blood inventory management by blood group
- Expiry and low-stock monitoring
- Blood availability search
- Blood request submission and tracking
- Blood request approval and rejection
- Blood issuance against approved requests
- Automatic inventory updates after donations and issues
- Reports and history
- Role-based access for different users
- Authentication and access control

---

## Users

### Blood Bank Staff

Responsible for day-to-day blood bank operations such as managing donors, recording donations, maintaining inventory, processing blood requests, and issuing blood.

### Hospital / Requesting Organization Staff

Can search for blood availability, submit blood requests, and track request status.

### Administrator

Manages administrative access and can view system information and reports.

---

## Basic Workflow

```text
Donor
   ↓
Donation Recorded
   ↓
Blood Inventory Updated
   ↓
Blood Availability Search
   ↓
Hospital / Organization Request
   ↓
Request Review
   ↓
Approve / Reject
   ↓
Blood Issue
   ↓
Inventory Updated
   ↓
Reports & History
```

---

## Technology Stack

### Backend

- Python
- Django

### Frontend

- HTML
- CSS
- JavaScript

### Database

- Relational Database

### Version Control

- Git
- GitHub

The exact database and deployment configuration may be updated as development progresses.

---

## Project Structure

The application is planned around separate functional areas such as:

```text
blood-bank-management-system/
│
├── donor-management/
├── donation-management/
├── inventory-management/
├── request-management/
├── blood-issue/
├── reports/
├── user-authentication/
│
├── templates/
├── static/
├── tests/
│
└── README.md
```

The final folder structure may change as the application is implemented.

---

## Blood Groups Supported

The system is designed to manage the standard blood groups:

- A+
- A-
- B+
- B-
- AB+
- AB-
- O+
- O-

---

## Inventory Management

Blood inventory is maintained according to blood group and availability.

The system is intended to:

- Add accepted donations to available stock
- Track stored blood units
- Monitor expiry information
- Prevent expired blood from being issued
- Identify low-stock blood groups
- Reduce available stock when blood is issued
- Prevent inventory from becoming negative

---

## Blood Request Process

A typical blood request follows this flow:

```text
Hospital submits request
        ↓
Request marked Pending
        ↓
Blood Bank Staff reviews request
        ↓
Check blood availability
        ↓
Approve / Reject request
        ↓
Approved request → Blood issued
        ↓
Inventory updated
```

---

## Security

The system is designed with role-based access so that users can only perform operations permitted for their role.

Protected functions require authentication, and sensitive operations such as modifying inventory, approving requests, and issuing blood are restricted to authorized users.

---

## Future Improvements

Possible future additions include:

- Donor self-service accounts
- Donation eligibility checks
- Nearby blood bank or donation centre search
- Notifications
- Improved analytics and dashboards
- Integration with external hospital systems
- Mobile-friendly donor services

---

## Team

Developed by Team 9.

---

## Status

Under Development

Core modules and workflows are currently being designed and implemented.

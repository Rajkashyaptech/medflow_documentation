# MedFlow

MedFlow is a role-based, multi-tenant hospital workflow management system designed to help hospitals and clinics manage doctors, patient visits, and prescriptions efficiently.

The system is built to be sold as a SaaS product to hospitals and healthcare providers.

---

## Purpose

Hospitals often struggle with:
- Manual paperwork
- Unstructured prescriptions
- Poor role separation
- Data access issues

MedFlow solves these problems using structured data, role-based access control, and automated prescription generation.

---

## Role-Based Access Model

MedFlow follows a strict role-based architecture:

### SuperAdmin (Platform Owner)
- Manages hospitals on the platform
- Onboards Hospital Admins
- No access to patient medical data

### HospitalAdmin (Hospital Management)
- Manages doctors, receptionists, and medical staff
- Controls hospital-level configuration
- Ensures staff belong to the correct hospital

### Doctor
- Consults patient visits
- Creates prescriptions
- Adds medicines with structured types
- Generates prescription PDFs

---

## Core Features

- Multi-hospital (multi-tenant) support
- Visit-based patient consultations
- Digital prescriptions with structured medicine data
- Predefined medicine types (tablet, syrup, injection, etc.)
- Printable PDF prescriptions
- Secure authentication and authorization
- Hospital-level data isolation

---

## Tech Stack

- Backend: Django
- Database: Relational DB (SQLite / PostgreSQL)
- Authentication: Django Auth
- PDF Generation: Service-based architecture

---

## One-Line Summary

MedFlow is a Django-based healthcare SaaS platform that digitizes hospital workflows using role-based access and structured prescription management.

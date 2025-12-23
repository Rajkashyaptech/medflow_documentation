# System Design – MedFlow

## Architecture Overview
MedFlow is a Django-based multi-tenant application following a modular architecture. Each domain is isolated into separate apps to ensure scalability and maintainability.

---

## Role-Based Access Control
The system enforces strict RBAC:
- SuperAdmin manages the platform and hospitals
- HospitalAdmin manages staff within a hospital
- Doctors access only their assigned visits

This ensures security, clarity, and efficiency.

---

## Data Model Relationships

User (Doctor / Admin)
Hospital
Visit
Prescription
PrescriptionItem

Flow:
Patient → Visit → Prescription → PrescriptionItem(s)

---

## Prescription & Medicine Design
Medicine data is structured using predefined types (tablet, capsule, syrup, injection). This eliminates ambiguity and ensures accurate dosage interpretation.

---

## PDF Generation
Prescription PDFs are generated via a service layer to keep business logic separate from presentation logic.

---

## Data Isolation & Security
Each hospital’s data is isolated. Doctors cannot access data outside their hospital or assigned visits. Unauthorized access returns HTTP 403 responses.

---

## Scalability
The modular design allows future features such as billing, pharmacy integration, and analytics without major architectural changes.

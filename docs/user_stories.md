# MedFlow – User Stories

## Overview

This document defines the **software requirements** for the MedFlow project using **User Stories**.  
User stories are written in the **ISBAT format**:

> **As a `<user>` I should be able to `<action>` so that `<benefit>`**

---

## 1: Authentication & Authorization

1. As a user, I should be able to log in using my credentials so that I can access the system securely.
2. As a user, I should be able to log out so that my account remains secure on shared devices.
3. As a hospital admin, I should be able to create user accounts for doctors and staff so that only authorized people access the system.
4. As a user, I should only be able to access features permitted to my role so that data security is maintained.
5. As a user, I should see an authorization error if I try to access a restricted page so that access rules are enforced.

---

## 2: Hospital & User Management

6. As a hospital admin, I should be able to manage doctors and staff so that hospital operations are controlled centrally.
7. As a hospital admin, I should be able to activate or deactivate a user so that access can be controlled when staff leave.
8. As a hospital admin, I should only see users belonging to my hospital so that data isolation is ensured.

---

## 3: Patient & Visit Management

9. As a receptionist, I should be able to register a patient so that their details are stored in the system.
10. As a receptionist, I should be able to create a visit for a patient so that the doctor can consult them.
11. As a doctor, I should be able to view my assigned visits so that I can consult patients efficiently.
12. As a doctor, I should only be able to consult visits assigned to me so that visit ownership is enforced.

---

## 4: Consultation & Prescription

13. As a doctor, I should be able to consult a patient visit so that medical advice can be recorded.
14. As a doctor, I should be able to create a prescription for a visit so that treatment is documented.
15. As a doctor, I should be able to add multiple medicines to a prescription so that complete treatment is provided.
16. As a doctor, I should be able to specify medicine type (tablet, capsule, syrup, injection) so that usage is clear.
17. As a doctor, I should be able to define dosage and duration so that patients follow correct treatment.

---

## 5: Medical Records Access

18. As a doctor, I should be able to view a patient’s past visits so that I can make informed medical decisions.
19. As a patient, I should be able to view my prescriptions so that I can access medical records anytime.
20. As a patient, I should be able to download my prescription so that I can keep a copy for reference.

---

## 6: Error Handling

21. As a user, I should see a 404 error page when accessing an invalid URL so that the system behaves predictably.
22. As a user, I should see a 403 error page when accessing unauthorized resources so that security rules are clear.
23. As a user, I should see validation errors when submitting invalid data so that mistakes can be corrected.

# Requirements Documentation

Elicitation techniques, requirements documents, and analysis artifacts.
# Requirements Documentation

Case Study: Pharmacy Management System

---

## 1. Elicitation Techniques Applied

| Technique | Purpose | Stakeholder |
|---|---|---|
| Interviews | Capture detailed daily workflow and pain points | Pharmacist, Cashier |
| Observation | Identify undocumented steps in the dispensing process | Pharmacy floor staff |
| Document Analysis | Review existing prescription forms and stock reports | Operations Manager |
| Workshops | Resolve conflicting priorities between departments | All stakeholders |

---

## 2. Stakeholder Analysis

| Stakeholder | Interest | Influence | Engagement Strategy |
|---|---|---|---|
| Pharmacist | High | High | Manage closely — primary system user |
| Cashier | High | Medium | Keep informed and involved in UAT |
| Operations Manager | High | High | Manage closely — approves requirements |
| Supplier | Low | Medium | Keep satisfied — inventory integration |
| Patient | High | Low | Keep informed — end beneficiary |

---

## 3. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | The system shall allow the pharmacist to record a prescription against a patient ID | Must Have |
| FR-02 | The system shall validate medications against the patient's recorded allergies | Must Have |
| FR-03 | The system shall display real-time stock quantity and expiry date per medication | Must Have |
| FR-04 | The system shall generate a unique order number for each prescription | Must Have |
| FR-05 | The system shall alert users when stock falls below the reorder threshold | Should Have |
| FR-06 | The system shall produce a daily dispensing summary report | Could Have |

Prioritization method: MoSCoW

---

## 4. Non-Functional Requirements

| ID | Requirement | Category |
|---|---|---|
| NFR-01 | The system shall return search results within 3 seconds | Performance |
| NFR-02 | The system shall restrict access based on user role | Security |
| NFR-03 | The system shall maintain an audit log of all dispensing transactions | Compliance |
| NFR-04 | The system shall support both Arabic and English interfaces | Usability |

---

## 5. Assumptions & Constraints

**Assumptions**
- Patient records already exist in a central database
- All staff have basic computer literacy

**Constraints**
- Must integrate with the existing supplier inventory system
- Must comply with local pharmaceutical regulatory requirements


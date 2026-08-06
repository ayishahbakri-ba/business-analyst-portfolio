# User Stories & Acceptance Criteria

Case Study: Pharmacy Management System

---

## US-01 | Prescription Entry

**As a** pharmacist  
**I want to** enter a patient's prescription into the system  
**So that** the order is recorded accurately before dispensing

### Acceptance Criteria

- **Given** I am logged in as a pharmacist  
  **When** I enter a patient ID that exists in the system  
  **Then** the patient's profile and allergy history are displayed

- **Given** I have entered a medication  
  **When** the medication conflicts with a recorded allergy  
  **Then** the system displays a warning and blocks submission

- **Given** all required fields are complete  
  **When** I submit the prescription  
  **Then** the system generates a unique order number

---

## US-02 | Stock Availability Check

**As a** pharmacist  
**I want to** see real-time stock levels for each medication  
**So that** I can inform the patient immediately if an item is unavailable

### Acceptance Criteria

- **Given** I search for a medication  
  **When** the item is in stock  
  **Then** the available quantity and expiry date are displayed

- **Given** stock quantity is below the reorder threshold  
  **When** the item is displayed  
  **Then** a low-stock indicator appears

---

## US-03 | Payment Processing

**As a** cashier  
**I want to** process payment against a prescription order number  
**So that** the transaction is completed and recorded

### Acceptance Criteria

- **Given** a valid order number is entered  
  **When** payment is confirmed  
  **Then** the order status changes to "Paid" and a receipt is generated

- **Given** payment fails  
  **When** the transaction is declined  
  **Then** the order remains open and an error message is displayed


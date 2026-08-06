# Process Modeling

BPMN diagrams and swimlane process maps.
# Process Modeling

BPMN 2.0 process models for the Pharmacy Management case study.

---

## Prescription Fulfillment Process

**Notation:** BPMN 2.0 — Swimlane (Cross-Functional) Diagram

### Participants

| Lane | Responsibility |
|---|---|
| Patient | Submits prescription, collects medication |
| Pharmacist | Validates prescription, checks stock, dispenses |
| Cashier | Processes payment, issues receipt |
| Inventory System | Updates stock levels, triggers reorder alerts |

---

### Process Flow

1. **Start Event** — Patient submits prescription
2. **Task** — Pharmacist verifies patient identity and prescription validity
3. **Exclusive Gateway** — Is the prescription valid?
   - No → Notify patient, terminate process
   - Yes → Continue
4. **Task** — Check medication stock availability
5. **Exclusive Gateway** — Is stock available?
   - No → Place supplier order, notify patient of delay
   - Yes → Continue
6. **Task** — Cashier processes payment
7. **Task** — Pharmacist dispenses medication
8. **Task** — Inventory System deducts dispensed quantity
9. **End Event** — Patient receives medication

---

### Modeling Notes

**Gateway usage**  
Exclusive (XOR) gateways are used where exactly one path can be taken. Each gateway is paired with a merge point so no sequence flow terminates without resolution.

**Common modeling errors avoided**
- Gateways left open without a converging merge
- Decision gateways with unlabeled outgoing flows
- Tasks placed in the wrong lane, misassigning responsibility
- Multiple start events in a single pool without justification

---

### Diagram

*(Diagram image below)*

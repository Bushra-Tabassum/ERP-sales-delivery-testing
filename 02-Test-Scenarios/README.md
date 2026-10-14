# Sales & Delivery – Test Scenarios

## Overview

This section contains selected test scenarios for the Sales Quotation and Sales Order workflows within the ERP Sales & Delivery module.

The scenarios focus on validating the end-to-end transaction flow, data consistency, business rules, status transitions, and integration between quotation and order processing.

---

## 1. Sales Quotation

- Verify a sales quotation can be created with valid customer, contact person, dates, and line-item information.
- Verify mandatory quotation fields cannot be left blank.
- Verify quotation expiry date cannot be earlier than quotation date.
- Verify customer and contact person combinations are validated correctly.
- Verify product / line-item details can be added successfully.
- Verify quantity accepts only valid values.
- Verify unit price is calculated or stored correctly.
- Verify discount calculation is applied correctly.
- Verify AIT / tax calculation is applied according to configuration.
- Verify quotation total is calculated correctly after quantity, price, tax, and discount changes.
- Verify invalid or negative financial values are rejected.
- Verify quotation can be saved and submitted successfully.
- Verify quotation status changes correctly during the approval workflow.
- Verify an approved quotation displays the correct completed status.
- Verify rejected or revised quotations follow the correct workflow.
- Verify quotation number is generated uniquely.
- Verify quotation search works using quotation number.
- Verify quotations can be filtered by customer.
- Verify quotations can be filtered by contact person.
- Verify date-range filtering returns the correct records.
- Verify AIT Included filter returns matching quotations.
- Verify Completed filter returns records matching the selected status.
- Verify Assigned to Me returns only the appropriate records.
- Verify Clear resets all search and filter fields.

---

## 2. Sales Order

- Verify a sales order can be created from an approved quotation.
- Verify only eligible / approved quotations can be linked to a sales order.
- Verify quotation reference is retained in the created sales order.
- Verify customer information is carried forward correctly from the quotation.
- Verify contact person is carried forward correctly.
- Verify product and line-item information is carried forward correctly.
- Verify quantity remains consistent between quotation and sales order.
- Verify unit price remains consistent unless modification is explicitly allowed.
- Verify discounts are transferred correctly.
- Verify tax / AIT information is transferred correctly.
- Verify billing and shipping information is populated correctly.
- Verify currency remains consistent between quotation and order.
- Verify order date is validated correctly.
- Verify expected delivery date cannot be earlier than order date.
- Verify shipping charges accept valid values.
- Verify line total is recalculated correctly when quantity, price, or discount changes.
- Verify a linked quotation cannot generate unintended duplicate sales orders.
- Verify order number is generated uniquely.
- Verify sales order status transitions correctly through the configured workflow.
- Verify completed sales orders display the correct final status.
- Verify search and filtering work correctly on the Sales Order list.
- Verify Clear resets the Sales Order search filters.

---

## 3. Quotation-to-Order Integration

- Verify approved quotation data is transferred accurately into the Sales Order.
- Verify the Sales Order remains linked to the correct source quotation.
- Verify customer and contact information remain consistent between both transactions.
- Verify product, quantity, price, discount, and tax values remain consistent.
- Verify changes made before order creation are reflected correctly in the Sales Order.
- Verify unrelated quotation data is not carried into the wrong Sales Order.
- Verify system prevents creating an order from an invalid quotation state.
- Verify duplicate processing does not create unintended transaction records.
- Verify failures during Sales Order creation do not leave partial or inconsistent data.

---

## 4. Workflow & State Validation

- Verify valid workflow actions are available for the current transaction status.
- Verify invalid state transitions are prevented.
- Verify completed transactions cannot be processed again unless explicitly supported.
- Verify next-action information matches the current workflow state.
- Verify workflow completion is reflected correctly in list and detail views.
- Verify transaction history remains consistent after workflow actions.

---

## 5. Role & Permission Testing

- Verify users only see actions allowed by their assigned role.
- Verify unauthorized users cannot create quotations.
- Verify unauthorized users cannot approve quotations.
- Verify unauthorized users cannot create sales orders.
- Verify frontend restrictions are also enforced by the backend.
- Verify users cannot access restricted transactions through direct navigation.

---

## 6. Validation & Negative Testing

- Verify required fields display validation messages when left blank.
- Verify invalid date combinations are rejected.
- Verify invalid numeric formats are rejected.
- Verify negative quantity, price, tax, or shipping values are handled correctly.
- Verify unsupported decimal precision is handled according to system rules.
- Verify duplicate submissions do not create duplicate transactions.
- Verify backend validation errors are shown clearly to the user.
- Verify failed requests do not leave partially saved transactions.

---

## 7. Regression Testing

- Verify Sales Quotation creation continues to work after workflow changes.
- Verify quotation approval does not break Sales Order creation.
- Verify pricing and tax calculations remain correct after updates.
- Verify search and filter functionality remains stable.
- Verify previously fixed quotation-to-order defects do not reappear.
- Verify changes in one transaction stage do not break downstream workflow behavior.

---

> All data and business information shown in this portfolio have been sanitized or recreated for demonstration purposes.

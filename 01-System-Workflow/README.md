# Sales & Delivery – System Workflow

## Overview

This document explains the core transaction workflow covered in this QA portfolio.

The selected flow focuses on how a sales transaction moves from an initial customer quotation into an approved sales order.

The workflow was used as the basis for designing end-to-end test scenarios, data consistency checks, workflow validation, and integration testing.

---

## Main Workflow

**Create Sales Quotation → Review / Approval → Customer Approval → Create Sales Order → Validate Order Details → Complete Sales Order Workflow**

---

## 1. Create Sales Quotation

A sales quotation is created for a selected customer and contact person.

The quotation may include:

- Customer information
- Contact person
- Quotation date
- Expiry date
- Product / line items
- Quantity
- Unit price
- Discount
- Tax / AIT information
- Additional commercial details

At this stage, the quotation enters the sales workflow.

---

## 2. Review / Approval

The quotation is reviewed according to the configured business workflow.

Testing at this stage focuses on:

- Required data
- Pricing accuracy
- Tax and discount calculation
- Date validation
- Status transition
- User permission
- Workflow action availability

---

## 3. Customer Approval

Once the quotation is accepted by the customer, the quotation status is updated accordingly.

The system should preserve the approved quotation information for use in the next transaction stage.

---

## 4. Create Sales Order

A Sales Order can be created from an approved quotation.

The Sales Order should remain correctly linked to its source quotation.

Important information expected to carry forward includes:

- Quotation reference
- Customer
- Contact person
- Product details
- Quantity
- Pricing
- Discount
- Tax / AIT information
- Billing details
- Shipping details

---

## 5. Validate Sales Order Details

The created Sales Order is reviewed to confirm that quotation data has transferred correctly.

Additional order-specific information may also be validated, including:

- Order date
- Expected delivery date
- Shipping charges
- Currency
- Billing address
- Shipping address
- Line-item totals
- Order status

---

## 6. Complete Sales Order Workflow

The Sales Order progresses through the configured workflow until the transaction reaches its completed state.

Testing focuses on ensuring:

- Valid status transitions
- Correct next actions
- Proper workflow restrictions
- Data consistency throughout the transaction lifecycle

---

## Key End-to-End Validation

The most important integration point in this workflow is:

**Sales Quotation → Sales Order**

The following values should remain consistent between the two transactions where applicable:

- Customer
- Contact person
- Quotation reference
- Product
- Quantity
- Unit price
- Discount
- Tax / AIT
- Address information
- Currency
- Transaction status

Any unexpected data change, missing value, or incorrect workflow transition should be treated as a potential defect.

---

## QA Coverage

This workflow supports testing of:

- Functional Testing
- End-to-End Testing
- Integration Testing
- Business Rule Validation
- Data Consistency Testing
- State Transition Testing
- Positive and Negative Testing
- Permission Testing
- Regression Testing

---

## Workflow Diagram

A visual workflow diagram is included in this folder to provide a quick overview of the transaction lifecycle.

---

> All transaction data, customer information, company details, and identifiers shown in this portfolio have been sanitized or recreated for demonstration purposes.

# Sales & Delivery – Test Cases

## Overview

This section contains selected manual test cases for two core workflows within the ERP Sales & Delivery module:

- Sales Quotation
- Sales Order

The test cases are curated for portfolio purposes to demonstrate practical QA coverage across transaction creation, validation, business rules, workflow behavior, permissions, and end-to-end data consistency.

---

## Test Coverage

The selected test cases include:

- Positive / Functional Testing
- Negative / Validation Testing
- Business Rule Validation
- Boundary / Edge Case Testing
- Integration / Data Consistency Testing
- Permission / Security Testing
- Regression Testing

The cases are grouped by testing type within each workbook to make the coverage easier to review.

---

## Sales Quotation

The Sales Quotation test cases focus on:

- Customer and contact-person selection
- Quotation creation
- Quotation and expiry-date validation
- Product / line-item handling
- Quantity and pricing validation
- Discount calculation
- AIT / tax behavior
- Quotation totals
- Workflow status transitions
- Customer approval
- Quotation-to-Sales-Order integration
- Role and permission validation

**Workbook:**  
`Sales_Quotation_Test_Cases.xlsx`

---

## Sales Order

The Sales Order test cases focus on:

- Creating Sales Orders from approved quotations
- Quotation reference validation
- Customer and contact-person consistency
- Product / line-item data transfer
- Quantity and pricing validation
- Discount and tax calculations
- Order and expected-delivery dates
- Billing and shipping information
- Shipping charges
- Order totals
- Workflow and status transitions
- Duplicate transaction prevention
- Role and permission validation
- End-to-end quotation-to-order consistency

**Workbook:**  
`Sales_Order_Test_Cases.xlsx`

---

## Test Case Structure

Each workbook contains:

- Test ID
- Test Case
- Test Steps
- Expected Result
- Actual Result
- Status

---

> All customer information, company details, transaction references, financial values, and other sensitive information shown in this portfolio have been sanitized or recreated for demonstration purposes.

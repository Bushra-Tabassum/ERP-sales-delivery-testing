# ERP Sales & Delivery – Manual QA Portfolio

## Project Overview

This project showcases my hands-on Manual QA experience testing the Sales & Delivery module of an ERP system.

The portfolio focuses on two core transaction workflows:

- Sales Quotation
- Sales Order

The main objective of testing was to validate the complete business flow from quotation creation and approval through sales order generation, while ensuring data consistency, workflow accuracy, pricing correctness, and proper system behavior across related transactions.

---

## Business Workflow Covered

The primary workflow tested in this project is:

**Sales Quotation → Customer Approval → Sales Order**

The testing also covers data carried forward between the quotation and order stages, including:

- Customer information
- Contact person
- Product / line-item details
- Quantity and pricing
- Discounts
- Tax / AIT information
- Billing and shipping details
- Delivery dates
- Transaction status

---

## Testing Scope

This project demonstrates testing across:

- Functional Testing
- End-to-End Workflow Testing
- Integration Testing
- Regression Testing
- Negative Testing
- Business Rule Validation
- Field Validation
- Data Consistency Testing
- Search and Filter Testing
- Role and Permission Testing
- UI/UX Testing
- API Testing where applicable

---

## Key Areas Tested

### Sales Quotation

Testing included:

- Creating sales quotations
- Customer and contact-person selection
- Quotation date and expiry-date validation
- Product and line-item handling
- Pricing and quantity validation
- Tax / AIT behavior
- Discount calculation
- Quotation status transitions
- Customer approval workflow
- Search and filtering

### Sales Order

Testing included:

- Creating sales orders from approved quotations
- Verifying quotation-to-order linkage
- Customer and contact information consistency
- Order and expected-delivery dates
- Shipping charges
- Billing and shipping addresses
- Product quantity and pricing
- Discount calculations
- Tax handling
- Order status and workflow transitions

---

## End-to-End Validation

Special attention was given to validating that information created in the Sales Quotation stage is transferred accurately into the Sales Order.

Examples include:

- Correct quotation reference
- Customer and contact-person consistency
- Product and pricing information
- Tax and discount values
- Address information
- Transaction status
- Workflow progression

---

## Defect Investigation Approach

When an issue was identified, I typically:

1. Reproduced the issue consistently
2. Identified the affected transaction stage
3. Checked frontend behavior and validations
4. Reviewed request/response data where required
5. Compared actual behavior with business requirements
6. Verified the impact on downstream transactions
7. Documented clear reproduction steps and supporting evidence

---

## Tools Used

- Browser Developer Tools
- Postman
- Excel / Google Sheets
- GitHub
- ERP Web Application

---

## Portfolio Deliverables

This repository includes:

- System Workflow
- Test Scenarios
- Detailed Test Cases
- Sample Bug Reports
- Supporting Evidence

---

## Confidentiality

All screenshots, company information, customer information, transaction references, financial data, and other identifiers shown in this portfolio are sanitized, blurred, or recreated for demonstration purposes.

No confidential client or production information is intentionally exposed.

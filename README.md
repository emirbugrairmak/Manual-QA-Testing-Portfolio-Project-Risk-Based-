# Manual QA Testing Portfolio Project (Risk-Based)

## Overview
This repository contains a **manual QA testing portfolio practice** on a demo e-commerce website. The demo website is : https://sauce-demo.myshopify.com/
The work is **risk-based** and includes:

- Business Requirements & Acceptance Criteria
- Test Plan
- Static Testing findings
- Smoke Testing execution
- Sanity Testing execution (**based on simulated changes**)
- Regression Testing (**black-box test design techniques applied**)
- Bug Reports
- Summary metrics

All artifacts are prepared in a single **Excel workbook**.

UPDATE : The “Bug Report” sheet in the Excel template has been migrated in a Jira-compatible format.

---

## Scope (High-Level)
Core user flows covered:

- Login / Logout
- Sign Up
- Search
- Product Details
- Add to Cart / View Cart
- Remove / Clear Cart (**if available**)
- Wishlist (Add / View)

---

## Test Types Included
### 1) Static Testing
Reviewed requirements and acceptance criteria for:
- missing details
- inconsistencies
- unclear or non-testable statements

### 2) Smoke Testing
Quick validation of critical flows to decide if the build is testable.

### 3) Sanity Testing (Simulated Changes)
Re-tested affected areas after **assumed changes** (because this is a practice project).  
Simulated change areas included (as documented in the Sanity sheet):
- Wishlist fix
- Search update
- Sign Up update

### 4) Regression Testing
Risk-based regression to check whether recent changes broke other areas.

---

## Regression Test Design Techniques Used (Black-Box)
Regression cases were designed using black-box techniques where applicable:

- **Decision Table** (e.g., Sign Up field validation combinations)
- **Equivalence Partitioning (EP)** (e.g., duplicate email categories, search inputs)
- **Boundary Value Analysis (BVA)** (e.g., minimum password length)
- **State Transition** (e.g., login/logout states and session behavior)
- **Use Case** (e.g., user flows like wishlist and product details)

> Note: Not every test case needs a unique table format.  
> The regression sheet stays standard; the **Technique** + **Technique Detail/Ref** columns explain EP/BVA/Decision Table/State Transition/Use Case logic.

---

## Project Artifacts (Excel Sheets)
The workbook includes:

- **İş Gereksinimi (Business Requirements)**
- **Test Plan**
- **Risk Önceliklendirme (Risk Prioritization)**
- **Statik Test (Static Test Findings)**
- **Smoke Test**
- **Sanity Test**
- **Regression Test**
- **Bug Report**
- **Summary**

✅ Evidence (screenshots/links) are referenced inside the workbook (e.g., “View the screenshot”).

---

## Summary Results (from Summary sheet)
- **Smoke:** Total 8 (Pass 6 / Fail 1 / Blocked 1)  
- **Sanity:** Total 9 (Pass 4 / Fail 2 / Blocked 3)  
- **Regression:** Total 31 (Pass 23 / Fail 4 / Blocked 4)

---

## Key Bugs Found (Examples)
- **Add to Wishlist button missing** on Product Details page (blocks Wishlist flow)
- **Password minimum length validation not enforced**
- **Unclear/generic validation messages** (email/password)

Full details are documented in the **Bug Report** sheet (including steps, expected vs actual, and evidence).

---

## Environment
- **OS:** macOS  
- **Browser:** Chrome

---

## How to Review
1. Open the Excel workbook: **`Manual Portfolio 1.xlsx`**
2. Start from **Summary** to see overall status.
3. Check **Bug Report** for defects and evidence references.
4. Review **Smoke / Sanity / Regression** sheets for execution details.
5. Use **Risk Önceliklendirme** to see why tests were prioritized.

---

## Author
Emir

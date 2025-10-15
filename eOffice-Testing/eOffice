# 🧩 eOffice Portal – Government Office Automation System (Manual Testing)

## 📘 Project Overview
This repository contains my **manual testing** work for the eOffice Portal — a government office automation system used for digital file and workflow management.

**Live URL:** https://services.eoffice.gov.in

**Purpose:** Validate workflow correctness, document upload/download & preview, form validation, role-based access, UI/UX consistency, and cross-browser/device compatibility.

---

## 📋 Table of Contents
- [Objectives](#objectives)  
- [Scope of Testing](#scope-of-testing)  
- [Modules Tested](#modules-tested)  
- [Tools & Environment](#tools--environment)  
- [Deliverables](#deliverables)  
- [Sample Test Cases](#sample-test-cases)  
- [Sample Bug Report Entries](#sample-bug-report-entries)  
- [How to Explore this Repo](#how-to-explore-this-repo)  
- [Key Findings & Recommendations](#key-findings--recommendations)  
- [Author](#author)

---

## 🎯 Objectives
- Verify file creation, forwarding, and note-sheet workflows operate as designed.  
- Validate document upload/download integrity and preview behavior.  
- Test authentication, role-based access control, and permissions.  
- Ensure UI consistency and responsiveness across desktop, tablet, and mobile.  
- Log defects with clear reproduction steps, screenshots, severity, and remediation suggestions.

---

## 🧩 Scope of Testing
- Functional Testing (workflows, authentication, search, notifications)  
- Regression Testing (post-fix verification)  
- UI/UX Validation (alignment, labels, form behavior)  
- Cross-browser & Device Testing (Chrome, Firefox, Edge; Desktop, Mobile)  
- Basic Accessibility Checks (tab order, form labels, alt text)

---

## 🧭 Modules Tested (representative)
- Login & Authentication  
- Dashboard & Inbox  
- File Creation & Note-sheet Workflow  
- Document Upload / Download / Preview  
- User Roles & Permissions (Officer, Clerk, Admin)  
- Search, Filters & Advanced Search  
- Notifications & Audit Trail / History  
- Settings & User Profile

---

## 🧰 Tools & Environment
| Category | Tools |
|---|---|
| Test Cases / Docs | Microsoft Excel / Google Sheets |
| Bug Tracking | Excel / Jira / GitHub Issues |
| Browsers | Chrome, Firefox, Edge |
| Devices | Desktop, Tablet, Mobile (Chrome DevTools or BrowserStack) |
| Other | Figma (UI ref), Chrome DevTools |

---

## 📦 Deliverables (in this folder)
- `TestPlan_eOffice.pdf` — Test strategy, entry/exit criteria, roles.  
- `TestCases_eOffice.xlsx` — 100+ detailed test cases (positive & negative).  
- `BugReport_eOffice.xlsx` — Structured bug log with screenshots and priorities.  
- `TestSummary_eOffice.pdf` — Execution summary, metrics, pass/fail counts.  
- `Screenshots/` — Evidence images (named like `BUG_eO_001.png`).  
- `README.md` — This file.

---

## 🧾 Sample Test Cases (extract)
Below are representative examples — full set is in `TestCases_eOffice.xlsx`.

| Test Case ID | Module | Title | Steps (brief) | Expected Result | Severity |
|---|---:|---|---|---|---:|
| TC_eO_001 | Login | Verify valid user login | Open login -> enter valid creds -> click Login | Dashboard loads | High |
| TC_eO_012 | File Workflow | Create file and forward to officer | Create File -> attach doc -> forward to Officer B | File appears in Officer B's inbox | High |
| TC_eO_020 | Document Upload | Verify PDF preview opens | Open file details -> click PDF attachment | PDF preview displays without error | Medium |
| TC_eO_034 | Permissions | Verify clerk cannot access Admin settings | Login as Clerk -> open header menu | Settings link not visible / access denied | High |
| TC_eO_050 | Search | Verify search by file number | Enter existing file number -> Search | Correct file in results | Medium |

---

## 🐞 Sample Bug Report Entries (extract)
Full bug list available in `BugReport_eOffice.xlsx`.

| Bug ID | TC ID | Module | Summary | Severity | Status |
|---|---:|---|---|---:|---|
| BUG_eO_001 | TC_eO_012 | File Workflow | 'Forward' button disabled after attaching doc | High | Open |
| BUG_eO_002 | TC_eO_020 | Document Upload | PDF preview shows 'unsupported format' error | Medium | Open |
| BUG_eO_004 | TC_eO_050 | Search | Exact file number search returns incomplete results | Major | Open |

---

## 🔎 How to Explore this Repo
1. Download or view the artifacts directly on GitHub: click the PDF / Excel files in this folder.  
2. Open `TestCases_eOffice.xlsx` to review the 100+ test cases.  
3. View `BugReport_eOffice.xlsx` (or convert entries to GitHub Issues for tracking).  
4. See `Screenshots/` for visual evidence linked to bug IDs.

---

## ✅ Key Findings & Recommendations (summary)
- **Critical:** Harden role-based access — permission leaks observed (fix P1).  
- **Major:** Improve document preview reliability — server-side validation for file types/sizes.  
- **UX:** Provide clearer success/confirmation messages for forwarding and saving note-sheets.  
- **Accessibility:** Ensure form labels, tab order and alt-text are present and correct.  
- **Process:** Automate core workflows (file creation & forwarding) to reduce regression risk.

---

## 📌 Commit Messages (suggested)
- `Add eOffice README and Test Plan`  
- `Upload TestCases_eOffice.xlsx (100 cases)`  
- `Upload BugReport_eOffice.xlsx (initial bugs)`  
- `Add screenshots and update README`

---

## 👩‍💻 Author / Contact
**Mariyam Usmani** — QA Analyst | Manual Testing | UI/UX Validation  
LinkedIn: https://www.linkedin.com/in/mariyam-usmani-3246a72

---

> ⚠️ **Note:** This is a demonstration/testing portfolio using publicly accessible pages and demo/test data. Do not upload any confidential or sensitive information into public repositories.

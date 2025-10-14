# 🧩 eOffice Portal – Government Office Automation System (Manual Testing)

## 📘 Project Overview
This repository contains my **manual testing** work for the eOffice Portal (https://services.eoffice.gov.in) — a government office automation system developed by NIC for digital file/workflow management.

The objective of this project was to validate **workflow correctness, document upload/download, form validation, role-based access, and UI/UX consistency** across devices and browsers.

---

## 🎯 Objectives
- Verify file creation, forwarding, and note-sheet workflows operate as designed
- Validate document upload/download integrity and file preview behavior
- Test authentication, role-based access control, and permissions
- Check UI consistency and responsiveness across desktop, tablet, and mobile
- Document defects with clear steps, screenshots, severity, and recommendations

---

## 🧩 Scope of Testing
- Functional Testing (workflows, authentication, search, notifications)  
- Regression Testing (post-fix verification)  
- UI/UX Validation (alignment, labels, form behavior)  
- Cross-Browser & Device Compatibility (Chrome, Firefox, Edge; Desktop, Mobile)  
- Accessibility checks (basic WCAG items: tab order, alt text, form labels)

**Modules Tested (examples):**
- Login & Authentication  
- Dashboard & Inbox  
- File Creation & Note Sheet Workflow  
- Document Upload / Download / Preview  
- User Roles & Permissions (Officer, Clerk, Admin)  
- Search, Filters & Advanced Search  
- Notifications & Audit Trail / History  
- Settings & User Profile

---

## 🧰 Tools & Environment
| Category | Tools |
|---|---|
| Test Cases / Docs | Excel / Google Sheets |
| Bug Tracking | Excel / Jira / GitHub Issues |
| Browsers | Chrome, Firefox, Edge |
| Devices | Desktop, Tablet, Mobile (Chrome DevTools or BrowserStack) |
| Other | Figma (for UI reference), Chrome DevTools |

---

## 📊 Deliverables
- **Test Plan (PDF)** — scope, strategy, roles, entry/exit criteria  
- **Test Cases (Excel)** — 100+ detailed test cases (positive & negative)  
- **Bug Report (Excel / Issues)** — structured defects with screenshots & priorities  
- **Test Execution Report (PDF)** — pass/fail counts, coverage, metrics  
- **Test Summary Report (PDF)** — key findings & recommendations  
- **Screenshots/** — evidence folder with named images (e.g., `BUG_eOffice_001.png`)

---

## 🧩 Sample Test Cases (extract)
See `TestCases_eOffice.xlsx` for the full list (100+). Below are representative test cases to show format and level of detail.

| Test Case ID | Module | Title | Steps to Execute | Test Data | Expected Result | Severity |
|---|---:|---|---|---|---|---|
| TC_eO_001 | Login | Verify valid user login | 1. Open login page<br>2. Enter valid username/password<br>3. Click Login | Valid user creds | User is logged in and dashboard loads | High |
| TC_eO_005 | Login | Verify password strength error on weak password change | 1. Login<br>2. Go to Change Password<br>3. Enter weak new password | Weak password | Error shows password strength requirements | Medium |
| TC_eO_012 | File Workflow | Create new file and forward to next officer | 1. Click 'Create File'<br>2. Fill metadata<br>3. Attach a document<br>4. Click 'Forward' to Officer B | Valid meta + doc | File created and appears in Officer B's inbox | High |
| TC_eO_020 | Document Upload | Verify PDF preview opens in browser | 1. Open file details<br>2. Click attachment (PDF) | PDF file | PDF opens in preview pane, no corruption | Medium |
| TC_eO_034 | Permissions | Verify clerk cannot access admin settings | 1. Login as Clerk<br>2. Attempt to open Admin -> Settings | Clerk account | Access denied or no Settings link visible | High |
| TC_eO_050 | Search | Verify search by file number returns correct file | 1. Open search<br>2. Enter existing file number<br>3. Click Search | Valid file number | Correct file appears in results | Medium |
| TC_eO_066 | Notifications | Verify notification appears when file forwarded | 1. Forward file from A to B<br>2. Log in as B<br>3. Check notifications | — | Notification received with link to file | Medium |
| TC_eO_080 | Responsiveness | Validate dashboard widgets render correctly on tablet | 1. Open dashboard in tablet viewport<br>2. Inspect widgets layout | Tablet viewport | Widgets resize, no overlaps | Medium |
| TC_eO_091 | Audit Trail | Verify audit trail records forward action | 1. Forward file<br>2. Open file audit trail | — | Entry in audit trail with user/time/action | High |
| TC_eO_099 | Form Validation | Verify mandatory fields on note sheet | 1. Create note sheet with missing mandatory fields<br>2. Click Save | Missing mandatory data | Validation error shown, cannot save | High |

---

## 🐞 Sample Bug Report Entries (extract)
See `BugReport_eOffice.xlsx` or GitHub Issues for all logged defects.

| Bug ID | Test Case ID | Module | Summary | Steps to Reproduce | Expected | Actual | Severity | Priority | Status |
|---|---|---|---|---|---|---|---:|---:|---|
| BUG_eO_001 | TC_eO_012 | File Workflow | 'Forward' button disabled after attach | 1. Create file<br>2. Attach doc<br>3. Try to forward | Forward succeeds | Forward button disabled | High | P1 | Open |
| BUG_eO_002 | TC_eO_020 | Document Upload | PDF preview shows 'unsupported format' error | 1. Open attachment PDF | PDF preview | 'Unsupported format' error | Medium | P2 | Open |
| BUG_eO_003 | TC_eO_034 | Permissions | Clerk sees Admin Settings link | 1. Login as Clerk<br>2. Open header menu | No Settings link | Settings visible | High | P1 | Open |
| BUG_eO_004 | TC_eO_050 | Search | Search returns incomplete results for exact file number | 1. Search exact number | File appears | No results / wrong results | Major | P1 | Open |
| BUG_eO_005 | TC_eO_080 | Responsiveness | Dashboard widgets overlap in landscape tablet | 1. Open dashboard in tablet landscape | Widgets aligned | Overlap observed | Medium | P2 | Open |

---

## 🧠 Key Findings & Recommendations (summary)
- Critical: Role-based access checks must be hardened (several permission leaks observed).  
- Major: Document preview reliability — some PDF types fail to preview; add server-side validation.  
- UX: Add clearer confirmation and success messages for file forwarding and note-sheet saves.  
- Accessibility: Ensure form labels and tab order follow WCAG basics.  
- Regression: Implement test automation for core workflows to avoid regressions.

---

## 🗂 Repository Contents (suggested)

# 📊 VWO Web Application – A/B Testing SaaS Platform (Manual Testing)

## 📘 Project Overview
This repository contains my **manual testing** work for the VWO web application (https://app.vwo.com) — a SaaS platform for experimentation, A/B testing, and analytics.

The objective of this project was to validate **authentication, project and experiment creation workflows, targeting, reporting, integrations, UI/UX consistency, and data accuracy** across browsers and devices.

---

## 🎯 Objectives
- Verify login/logout, session management, and session timeout behavior
- Validate project creation, experiment setup, and variation configuration
- Test targeting rules, audience segmentation, and traffic allocation
- Verify analytics reports, conversion tracking, and data accuracy
- Test integrations (e.g., tracking script behavior) and export features
- Ensure UI consistency, responsiveness, and accessibility

---

## 🧩 Scope of Testing
- Functional Testing (workflows, experiment flows, reports)
- Regression Testing (post-fix verification)
- UI/UX Validation (alignment, labels, responsive behavior)
- Cross-browser & Device Compatibility (Chrome, Firefox, Edge; Desktop, Mobile)
- Basic Accessibility Checks (tab order, ARIA attributes, contrast)

**Modules Tested (examples):**
- Authentication & Account Management
- Dashboard & Project Overview
- Experiment / Test Creation (A/B, Split URL, MVT)
- Variations & Visual Editor
- Targeting & Segmentation
- Analytics & Reports (Conversion, Revenue, Goals)
- Integrations & Tracking Script
- Billing & Account Settings
- Notifications & Audit Trail

---

## 🧰 Tools & Environment
| Category | Tools |
|---|---|
| Test Cases / Docs | Excel / Google Sheets |
| Bug Tracking | Excel / Jira / GitHub Issues |
| Browsers | Chrome, Firefox, Edge |
| Devices | Desktop, Tablet, Mobile (Chrome DevTools or BrowserStack) |
| Other | GA/Analytics knowledge helpful, Chrome DevTools, Postman (for API checks) |

---

## 📦 Deliverables (in this folder)
- `TestPlan_VWO.pdf` — Test strategy and entry/exit criteria
- `TestCases_VWO.xlsx` — 90+ detailed test cases (positive & negative)
- `BugReport_VWO.xlsx` — Structured bug log with screenshots & priorities
- `TestSummary_VWO.pdf` — Execution summary and key metrics
- `Screenshots/` — Evidence images (named like `BUG_VWO_001.png`)
- `README.md` — This file

---

## 🧾 Sample Test Cases (extract)
See `TestCases_VWO.xlsx` for the full list (90 cases). Representative examples below:

| Test Case ID | Module | Title | Steps (brief) | Expected Result | Severity |
|---|---:|---|---|---|---:|
| TC_VWO_001 | Authentication | Verify valid user login | Open login -> enter valid credentials -> click Login | Dashboard loads successfully | High |
| TC_VWO_012 | Project | Create new project and verify it appears in dashboard | Click 'New Project' -> Enter details -> Save | Project appears in Projects list | High |
| TC_VWO_025 | Experiment | Create A/B experiment with 2 variations | Create experiment -> Configure goals -> Start experiment | Variations display and traffic allocated | High |
| TC_VWO_038 | Visual Editor | Edit variation in visual editor and save changes | Open visual editor -> Modify element -> Save changes | Changes persist and preview shows update | Medium |
| TC_VWO_054 | Targeting | Configure audience targeting by URL and cookie | Set targeting rules -> Save -> Launch | Targeting applies as configured | High |
| TC_VWO_070 | Reports | Verify conversion report shows correct counts after simulated traffic | Run test traffic -> Open reports | Report shows conversions matching test data | Major |
| TC_VWO_085 | Integrations | Validate tracking script loads and sends events | Install script on test page -> Trigger event | Event received in VWO dashboard | Major |

---

## 🐞 Sample Bug Report Entries (extract)
See `BugReport_VWO.xlsx` for all logged defects.

| Bug ID | TC ID | Module | Summary | Severity | Status |
|---|---|---|---|---:|---|
| BUG_VWO_001 | TC_VWO_012 | Project | New project creation fails with 500 error | High | Open |
| BUG_VWO_002 | TC_VWO_025 | Experiment | Variation preview not rendering in visual editor | Major | Open |
| BUG_VWO_005 | TC_VWO_054 | Targeting | Audience rule ignores cookie condition | High | Open |
| BUG_VWO_009 | TC_VWO_070 | Reports | Conversion counts mismatch expected values | Major | Open |

---

## 🔎 How to Explore this Repo
1. Open `TestCases_VWO.xlsx` to review 90+ test cases.  
2. View `BugReport_VWO.xlsx` for sample defects with reproduction steps and screenshots.  
3. Check PDFs (`TestPlan_VWO.pdf`, `TestSummary_VWO.pdf`) for strategy and summary.  
4. See `Screenshots/` for visual evidence linked to bug IDs.

---

## ✅ Key Findings & Recommendations (summary)
- Critical: Fix experiment creation backend error to avoid test launch failures.  
- Major: Visual editor rendering issues need attention to prevent incorrect variation previews.  
- Major: Ensure tracking script robustness and provide clearer error messages for integration issues.  
- UX: Improve in-editor save confirmation and provide undo/redo in visual editor.  
- Process: Add regression tests for experiment creation and reporting pipelines.

---

## 🗂 Repository Contents (suggested)
```
VWO-Testing/
├── README.md
├── TestPlan_VWO.pdf
├── TestCases_VWO.xlsx
├── BugReport_VWO.xlsx
├── TestSummary_VWO.pdf
└── Screenshots/
    ├ BUG_VWO_001.png
    └ test-summary.png
```

---

## 👩‍💻 Author
**Mariyam Usmani** — QA Analyst | Manual Testing | UI/UX Validation  
LinkedIn: https://www.linkedin.com/in/mariyam-usmani-3246a72

## EchoGPT Sign-Up & Authentication Testing

### 📌 Project Overview

This repository contains the test case report and execution results for the EchoGPT.live Sign-Up & Authentication module. The objective of this testing is to validate the functionality, usability, security, and reliability of the registration and login flows.

The scope of testing covers Email-based sign-up (OTP flow) as well as third-party authentication (Google, Twitter, GitHub).

### 📂 Contents <br>
**1. EchoGPT_TestStrategy.pdf** <br>
A comprehensive document outlining the test approach, scope, objectives, environment, risk analysis, schedule, and deliverables for the EchoGPT.live Sign-Up & Authentication testing project.

**2. EchoGPT_TestCaseSuite.xlsx**

Contains detailed test cases, execution results, and bug tracking across multiple organized sheets:

- `Test Summary` – Provides an overview of planned vs executed cases, pass/fail counts, and overall progress.

- `Functional Test Cases` – Covers sign-up, OTP, and OAuth flows with preconditions, steps, expected vs actual results, and status.

- `Usability & Security Test Cases` – Focuses on error messages, accessibility, and session management scenarios.

**3. EchoGPT_Test Execution & Bug Reporting** <br>
A structured log of all identified issues with severity/priority levels and resolution status. <br>

### 🧾 Description of Excel Sheets
**Test Summary**

- High-level overview of planned vs executed test cases.

- Metrics such as pass rate, fail rate, and execution coverage.

**Functional Test Cases**

Structured with the following fields:

- Test Case ID

- Test Case Title

- Preconditions

- Test Steps

- Expected Results

- Priority

- Test Data Requirements

- Actual Results

- Status (Pass, Fail, Not Executed)


**Covers:**

- `Email Sign-Up with OTP verification.`

- `OAuth Sign-Up via Google, Twitter, GitHub.`

- `Input validation` for empty fields, invalid formats, and long text.

**Usability & Security Test Cases**

**Covers:**

- Navigation flow issues (sign-up vs sign-in).

- Error message visibility.

- Dark mode contrast issues.

- Session persistence problems.

- Accessibility validation.

### Bug Report

Each defect entry includes:

- Bug ID

- Title/Description

- Steps to Reproduce

- Expected vs Actual Results

- Priority & Severity

- Environment & Browser Info

- Screenshots/Videos

- Workarounds

### 🔍 Types of Testing Performed

- **Functional Testing** – Validates sign-up, OTP, and OAuth flows.

- **Usability Testing** – Evaluates navigation, error handling, and accessibility.

- **Security Testing** – Focuses on OTP integrity, session management, and invalid inputs.

- **Compatibility Testing** – Checked across multiple devices & browsers.

- **Negative Testing** – Ensures the system behaves correctly under invalid inputs.

### 📊 Test Case Summary
| Module                         | Total Cases | Passed | Failed | Not Executed | Pass Rate |
|--------------------------------|-------------|--------|--------|--------------|-----------|
| Email Sign-Up (OTP)            | 15          | 13     | 2      | 0            | 86.67%    |
| OAuth (Google, Twitter, GitHub)| 6           | 6      | 0      | 0            | 100%      |
| Validation & Error Handling    | 7           | 6      | 1      | 0            | 85.71%    |
| Session & Security             | 3           | 2      | 1      | 0            | 66.67%    |
| **Overall**                    | **31**      | **28** | **4**  | **0**        | **90.3%** |

### ⚠️ Defect Analysis
**High Severity Issues**

**1. Session Persistence (ECHO-AUTH-001 & ECHO-AUTH-002)**

- Multiple accounts remain logged in simultaneously.

- Risk of data privacy breach.

**2. Login Page Accessible While Authenticated (ECHO-AUTH-003)**

- Authenticated users can still access login page.

- No redirect or warning.

**Medium Severity Issues**

- Poor visibility of social login buttons in dark mode.

- Missing error messages for non-registered or duplicate emails.

### ✅ Overall Quality Assessment

* **Strengths:**
  * Smooth email sign-up with OTP.
  * OAuth integrations (Google, Twitter, GitHub) working correctly.
  * Strong input validation.
  * Consistent across devices and browsers.<br>
* **Weaknesses:**
  * `Critical session handling flaws.`
  * `Accessibility issues (low-contrast buttons).`
  * Unclear error handling in edge cases. <br>

### 🚀 Recommendations

**1. Fix session handling** – Prevent multiple active accounts.

**2. Improve error handling** – Add clear messages for invalid OTP, duplicate, and unregistered emails.

**3. Accessibility fixes** – Enhance button contrast (WCAG standard).

**4. Security improvements** – Add OTP attempt limits and session timeouts.

**5. Regression testing** – Re-run after fixes, with focus on session flows.

### 📌 Key Statistics

**Total Test Cases Planned:** 31

**Executed:** 31 (100%)

**Pass Rate:** 90.3%

**Defects Identified:** 3 high severity, 2 medium severity

### 💻 How to Run
**Clone the Repository**
```bash
https://github.com/Sumaiya-Meem/Echogpt_Manual-Testing-Projects.git
```
**OR** <br>
**Download the ZIP** <br>

### Let's Connect with Me <br>
Interested in my work? Feel free to reach out by email or on LinkedIn <br>
📧 sumaiyameem056@gmail.com <br>
📫 [LinkedIn](https://www.linkedin.com/in/sumaiya-meem-28534b2a4/)

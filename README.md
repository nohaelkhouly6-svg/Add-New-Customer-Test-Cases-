# Add New Customer Feature - Testing Portfolio

Test documentation for the Add New Customer feature including Test Scenarios, Test Cases, and Bug Report.

## 📊 Project Deliverables
* **Live Test Cases & Bug Report:** [Click Here to View the Google Sheet](https://docs.google.com/spreadsheets/d/1-0I62-IcfEiIAf8os6OoCBU0Av2m828RV2OKTnY9KfE/edit?usp=sharing)

---

## 🐛 Defect Log / Bug Reports Summary

Below is the structured defect log compiled during the execution of the test cases:

| Defect_ID | Defect Title | Pre-condition | Test Data | (Test-Steps) procedures | Expected Result | Actual Result | Priority | Severity | ProbCateg | Bug Status | Test Case ID | Req ID | Designed By |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **BUG_NC_001** | Customer Name field truncates input | Add New Customer page, Chrome | Hubert Blaine Wolfeschlegel... (40+ chars) | 1. Enter 40-char name.<br>2. Fill details.<br>3. Submit. | System accepts the name and proceeds Normally. | The field only accepted 23 letters and truncated the rest. | High | Medium | Functional Positive | New | TC_NC_002 | SIQ_19 | Noha |
| **BUG_NC_002** | Missing Inline Validation for Empty Name | Add New Customer page, Chrome | Customer Name: (empty) | 1. Leave Name empty.<br>2. Fill details.<br>3. Submit. | System displays an error beside the field: "Invalid Input". | No inline error; a message with (please fill all data appeared) at top. | Medium | Low | Functional Negative | New | TC_NC_004 | T6 | Noha |
| **BUG_NC_003** | Missing Inline Validation for Invalid Name Inputs | Add New Customer page, Chrome | "123456" or "Ahmed@Ali" | 1. Enter numbers/special chars.<br>2. Fill details.<br>3. Submit. | System displays an error beside the field: "Invalid Input". | No inline error; a message with (please fill all data appeared) at top. | High | Medium | Functional Negative | New | TC_NC_005, 006 | T4, T5 | Noha |
| **BUG_NC_004** | City/State Fields Boundary Limit Violation | Add New Customer page, Chrome | City/State: "Alexandriaa" (11 chars) | 1. Input > 10 chars.<br>2. Fill details.<br>3. Submit. | System displays an error beside the field: "Invalid Input". | System accepts the city/state and proceeds normally. | Medium | Medium | Functional Negative | New | TC_NC_028, 036 | SIQ_23 | Noha |
| **BUG_NC_005** | Invalid Email Format Validation Bypass | Add New Customer page, Chrome | "testgmail.com", "test@gmail" | 1. Enter invalid email.<br>2. Fill details.<br>3. Submit. | System displays an error beside the field: "Invalid e-mail". | System accepts the e-mail and proceeds normally. | High | High | Functional Negative | New | TC_NC_051 | T28, SIQ_25 | Noha |

---
## 🛠️ Tools Used
* **Test Management & Defect Tracking:** Google Sheets (Cloud-based tracking).
* **Environment:** Windows 11, Google Chrome Browser.

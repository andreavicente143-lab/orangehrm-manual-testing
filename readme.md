# OrangeHRM – Manual Testing Project

## 1. Project Overview

This is a personal manual testing project using the OrangeHRM demo application.

The objective is to practice software testing activities, including test case design, test execution, bug reporting and defect investigation.

**Application under test:** [OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/)

## 2. Tools Used

- Jira – Test and bug tracking.
- Chrome DevTools – Defect investigation and network analysis.
- Microsoft Excel – Test case documentation and execution results.
- Git and GitHub – Project documentation and version control.

## 3. Testing Scope

The project focuses on the Forgot Password functionality.

The following scenarios were considered:

- Password reset with a registered username.
- Password reset with a non-existent username.
- Password reset with an empty username.
- Cancel password recovery.

## 4. Testing Activities

- Requirement analysis.
- Positive and negative test scenarios.
- Test case design.
- Manual test execution.
- Test result documentation.
- Bug reporting using Jira.
- Defect investigation using Chrome DevTools.
- HTTP request and response analysis.

## 5. Test Results

Test cases and execution results are documented in the corresponding project files.

## 6. Defects Found

During testing, a 504 Gateway Time-out error was observed when submitting a password reset request with a registered username.

The issue was investigated using Chrome DevTools, identifying the failing HTTP request and its response status.

The root cause was not determined.

## 7. Project Structure

- `test-cases/` – Test case documentation.
- `test-execution/` – Test execution results.
- `bug-reports/` – Bug reports.
- `evidence/` – Screenshots and testing evidence.

## 8. Disclaimer

This is an independent learning project using a publicly available demo application. It is not professional QA experience or work performed for OrangeHRM.
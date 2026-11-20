# Forgot Password – Test Execution Results

## 1. Execution Summary

- **Application:** OrangeHRM Demo
- **Module:** Authentication
- **Functionality:** Forgot Password
- **Testing Type:** Manual Testing
- **Execution Date:** 2026-11-20

## 2. Test Execution Results

| Test Case ID | Test Description | Actual Result | Status |
|---|---|---|---|
| CP01 | Reset password with a registered username | Page remained loading and returned a 504 Gateway Time-out error. | Failed |
| CP02 | Reset password with a non-existent username | Confirmation message displayed: "Reset Password link sent successfully". | Passed |
| CP03 | Reset password with an empty username | The validation message "Required" was displayed. | Passed |
| CP04 | Cancel password recovery | User was redirected to the Login page. | Passed |
| CP05 | Cancel password recovery after entering a username | Not executed. | Not Run |
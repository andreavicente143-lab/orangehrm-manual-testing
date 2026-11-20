# Bug Report 001 – Password Reset Returns 504 Gateway Time-out

## 1. Bug Information

- **Bug ID:** BUG-001
- **Title:** Password reset request returns 504 Gateway Time-out
- **Module:** Authentication
- **Feature:** Forgot Password
- **Environment:** OrangeHRM Demo
- **Severity:** To be determined
- **Priority:** To be determined
- **Related Test Case:** CP01

## 2. Preconditions

- The Forgot Password page is open.
- A registered username is available.

## 3. Steps to Reproduce

1. Open the OrangeHRM Demo login page.
2. Click on "Forgot your password?".
3. Enter the registered username `Admin`.
4. Click on "Reset Password".
5. Wait for the response.

## 4. Expected Result

The application should process the password reset request and display a confirmation message.

## 5. Actual Result

The page remains loading for approximately one minute and then displays a 504 Gateway Time-out error.

## 6. Technical Evidence

- **Request URL:** `/web/index.php/auth/requestResetPassword`
- **Request Method:** POST
- **HTTP Status Code:** 504 Gateway Time-out
- **Response Server:** nginx/1.18.0 (Ubuntu)


## 8. Additional Notes

The issue was observed during manual testing. The root cause has not been determined. It may be related to the demo server or its infrastructure.
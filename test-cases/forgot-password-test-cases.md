# Forgot Password – Test Scenarios and Test Cases

## 1. Application Under Test

- **Application:** OrangeHRM Demo
- **URL:** https://opensource-demo.orangehrmlive.com/
- **Module:** Authentication
- **Functionality:** Forgot Password
- **Testing Type:** Manual Testing

## 2. Test Scenarios

| Scenario ID | Test Scenario | Test Type |
|---|---|---|
| TS01 | Password reset with a registered username | Positive |
| TS02 | Password reset with a non-existent username | Negative |
| TS03 | Password reset with an empty username | Negative |
| TS04 | Cancel the password recovery process | Functional |
| TS05 | Cancel password recovery after entering a username | Functional |

## 3. Test Cases

### CP01 – Reset password with a registered username

**Preconditions:**
- The Forgot Password page is open.
- A registered test username is available.

**Test Steps:**
1. Enter a registered username.
2. Click on "Reset Password".

**Test Data:**
- Username: `Admin`

**Expected Result:**

The system should process the password reset request and display a confirmation message.

---

### CP02 – Reset password with a non-existent username

**Preconditions:**
- The Forgot Password page is open.

**Test Steps:**
1. Enter a non-existent username.
2. Click on "Reset Password".

**Test Data:**
- Username: `admin897`

**Expected Result:**

The system should handle the request according to the specified requirements and display the appropriate message.

---

### CP03 – Reset password with an empty username

**Preconditions:**
- The Forgot Password page is open.

**Test Steps:**
1. Leave the username field empty.
2. Click on "Reset Password".

**Test Data:**
- Username: Empty.

**Expected Result:**

The system should prevent the request and display a message indicating that the username field is required.

---

### CP04 – Cancel password recovery

**Preconditions:**
- The Forgot Password page is open.

**Test Steps:**
1. Click on "Cancel".

**Test Data:**
- Not applicable.

**Expected Result:**

The system should cancel the password recovery process and redirect the user to the Login page.

---

### CP05 – Cancel password recovery with a username entered

**Preconditions:**
- The Forgot Password page is open.

**Test Steps:**
1. Enter a registered username.
2. Click on "Cancel".

**Test Data:**
- Username: `Admin`

**Expected Result:**

The system should cancel the password recovery process and redirect the user to the Login page.
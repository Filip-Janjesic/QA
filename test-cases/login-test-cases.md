# Login Feature – Test Cases

## Test Case 1

**Test Case ID:** TC-LOGIN-001  
**Title:** Successful login with valid credentials

**Preconditions**
- User account exists

**Steps**
1. Open the login page
2. Enter a valid email address
3. Enter the correct password
4. Click the "Login" button

**Expected Result**
User is successfully logged in and redirected to the dashboard.

---

## Test Case 2

**Test Case ID:** TC-LOGIN-002  
**Title:** Login with incorrect password

**Preconditions**
- User account exists

**Steps**
1. Open the login page
2. Enter a valid email address
3. Enter an incorrect password
4. Click the "Login" button

**Expected Result**
System displays an error message: "Invalid email or password".

---

## Test Case 3

**Test Case ID:** TC-LOGIN-003  
**Title:** Login with empty fields

**Steps**
1. Open the login page
2. Leave email and password fields empty
3. Click the "Login" button

**Expected Result**
Validation message appears asking the user to fill in required fields.

---

## Test Case 4

**Test Case ID:** TC-LOGIN-004  
**Title:** Login with invalid email format

**Steps**
1. Open the login page
2. Enter an invalid email (example: user@)
3. Enter any password
4. Click "Login"

**Expected Result**
System shows validation error for invalid email format.

---

## Test Case 5

**Test Case ID:** TC-LOGIN-005  
**Title:** Password field masking

**Steps**
1. Open the login page
2. Type password in the password field

**Expected Result**
Password characters are masked (shown as dots or asterisks).
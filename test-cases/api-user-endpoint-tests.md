# API Test Cases – User Endpoint

## Endpoint

GET /api/users/{id}

---

## Test Case 1

**Test Case ID:** TC-API-001  
**Title:** Retrieve user with valid ID

**Preconditions**
- User with ID = 1 exists in the system

**Steps**
1. Send GET request to `/api/users/1`

**Expected Result**
- Status code: 200 OK
- Response contains user data (id, name, email)

---

## Test Case 2

**Test Case ID:** TC-API-002  
**Title:** Retrieve user with non-existing ID

**Steps**
1. Send GET request to `/api/users/9999`

**Expected Result**
- Status code: 404 Not Found
- Error message returned

---

## Test Case 3

**Test Case ID:** TC-API-003  
**Title:** Invalid ID format

**Steps**
1. Send GET request to `/api/users/abc`

**Expected Result**
- Status code: 400 Bad Request
- Validation error returned

---

## Test Case 4

**Test Case ID:** TC-API-004  
**Title:** Unauthorized access

**Steps**
1. Send GET request without authentication token

**Expected Result**
- Status code: 401 Unauthorized

---

## Test Case 5

**Test Case ID:** TC-API-005  
**Title:** Response structure validation

**Steps**
1. Send GET request to `/api/users/1`

**Expected Result**
Response JSON contains:

- id
- name
- email
- created_at
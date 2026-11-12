# Login Test Cases

## Overview

This document defines the test cases for the OrangeHRM login functionality.
Each test case is identified by a unique ID and covers a specific login scenario.

## Test Case Format

| Field | Description |
|-------|-------------|
| **Test ID** | Unique identifier for the test case |
| **Title** | Short descriptive name |
| **Description** | What the test case validates |
| **Preconditions** | State required before executing the test |
| **Steps** | Ordered actions to perform |
| **Expected Result** | What should happen if the system behaves correctly |
| **Priority** | High / Medium / Low |
| **Severity** | Critical / Major / Minor |

---

## Test Cases

### TC-LOGIN-001: Valid Login with Correct Credentials

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-001 |
| **Title** | Valid Login with Correct Credentials |
| **Description** | Verify that a user can successfully log in with valid username and password |
| **Preconditions** | User account exists and is enabled; login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Enter a valid username<br>3. Enter a valid password<br>4. Click the Login button |
| **Expected Result** | User is redirected to the dashboard page; session is established |
| **Priority** | High |
| **Severity** | Critical |

---

### TC-LOGIN-002: Invalid Username

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-002 |
| **Title** | Invalid Username |
| **Description** | Verify that login fails when an invalid username is provided |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Enter an invalid username<br>3. Enter a valid password<br>4. Click the Login button |
| **Expected Result** | Error message is displayed; user remains on the login page |
| **Priority** | High |
| **Severity** | Critical |

---

### TC-LOGIN-003: Invalid Password

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-003 |
| **Title** | Invalid Password |
| **Description** | Verify that login fails when an invalid password is provided |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Enter a valid username<br>3. Enter an invalid password<br>4. Click the Login button |
| **Expected Result** | Error message is displayed; user remains on the login page |
| **Priority** | High |
| **Severity** | Critical |

---

### TC-LOGIN-004: Empty Username and Password

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-004 |
| **Title** | Empty Username and Password |
| **Description** | Verify that login fails when both username and password fields are left empty |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Leave username field empty<br>3. Leave password field empty<br>4. Click the Login button |
| **Expected Result** | Error message is displayed; user remains on the login page |
| **Priority** | High |
| **Severity** | Major |

---

### TC-LOGIN-005: Empty Username Only

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-005 |
| **Title** | Empty Username Only |
| **Description** | Verify that login fails when only the username field is left empty |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Leave username field empty<br>3. Enter a valid password<br>4. Click the Login button |
| **Expected Result** | Error message is displayed; user remains on the login page |
| **Priority** | Medium |
| **Severity** | Major |

---

### TC-LOGIN-006: Empty Password Only

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-006 |
| **Title** | Empty Password Only |
| **Description** | Verify that login fails when only the password field is left empty |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Enter a valid username<br>3. Leave password field empty<br>4. Click the Login button |
| **Expected Result** | Error message is displayed; user remains on the login page |
| **Priority** | Medium |
| **Severity** | Major |

---

### TC-LOGIN-007: Remember Me Checkbox

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-007 |
| **Title** | Remember Me Checkbox |
| **Description** | Verify that the Remember Me checkbox persists the session across browser restarts |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Enter valid credentials<br>3. Check the Remember Me checkbox<br>4. Click the Login button<br>5. Close the browser<br>6. Reopen the browser and navigate to the application |
| **Expected Result** | User is automatically logged in and redirected to the dashboard |
| **Priority** | Medium |
| **Severity** | Major |

---

### TC-LOGIN-008: Lost Password Link

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-008 |
| **Title** | Lost Password Link |
| **Description** | Verify that the Lost Password link navigates to the password reset page |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Click the Lost Password link |
| **Expected Result** | User is redirected to the password reset page |
| **Priority** | Low |
| **Severity** | Minor |

---

### TC-LOGIN-009: Login Page Accessibility

| Field | Value |
|-------|-------|
| **Test ID** | TC-LOGIN-009 |
| **Title** | Login Page Accessibility |
| **Description** | Verify that the login page has no WCAG A/AA accessibility violations |
| **Preconditions** | Login page is accessible |
| **Steps** | 1. Navigate to the login page<br>2. Run an accessibility audit against the page |
| **Expected Result** | No accessibility violations are found |
| **Priority** | Medium |
| **Severity** | Major |

---

## CSV Data Reference

The corresponding test data for parameterized execution is available in `login-testcases.csv`.
# Security Report

## Identified Vulnerabilities and Fixes

1. **SQL Injection**
   - **File:** `risk_script2.py`
   - **Description:** The login route was vulnerable to SQL injection due to the use of string interpolation in SQL queries.
   - **Fix:** Implemented parameterized queries to prevent SQL injection.

2. **Cross-Site Scripting (XSS)**
   - **File:** `index.html`
   - **Description:** The application was vulnerable to XSS attacks due to the use of `innerHTML` to insert user input directly into the DOM.
   - **Fix:** Changed to use `textContent` to safely insert user input.

## Recommendations
- Regularly review and update dependencies to mitigate vulnerabilities.
- Implement input validation and sanitization for all user inputs.
- Consider using security headers to enhance protection against XSS and other attacks.

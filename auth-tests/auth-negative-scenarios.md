# Authentication API – Negative Test Scenarios

## Scenario 1: Missing Authorization Token
- Request sent without Authorization header
- Expected Status Code: 401 Unauthorized
- Purpose: Verify API blocks unauthenticated access

## Scenario 2: Invalid Token
- Authorization token is malformed or incorrect
- Expected Status Code: 401 Unauthorized
- Purpose: Ensure invalid tokens are rejected

## Scenario 3: Expired Token
- Authorization token is expired
- Expected Status Code: 403 Forbidden
- Purpose: Ensure expired sessions are not allowed

## Scenario 4: Wrong Token Type
- Authorization header uses incorrect token format
- Expected Status Code: 401 Unauthorized
- Purpose: Validate strict auth format enforcement

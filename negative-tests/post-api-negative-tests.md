# POST API – Negative Test Scenarios

## Scenario 1: Missing Request Body
- Method: POST
- Expected Result: 400 Bad Request
- Reason: API should not accept empty payload

## Scenario 2: Invalid Content-Type Header
- Header: Content-Type: text/plain
- Expected Result: 415 Unsupported Media Type

## Scenario 3: Invalid JSON Structure
- Payload: Malformed JSON
- Expected Result: 400 Bad Request

## Scenario 4: Wrong HTTP Method
- Method: GET instead of POST
- Expected Result: 405 Method Not Allowed

# Lab 16 — ErrorResponse JSON Draft

## Fields
status · message · correlationId — all three required in every error payload.

## Sample (CUS-9999)
```json
{ "status": 404, "message": "Customer not found", "correlationId": "lab-request-001" }

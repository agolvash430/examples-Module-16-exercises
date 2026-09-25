# Lab 16 — Failure to Status Map

| Failure | Status |
| --- | --- |
| CUS-9999 not found | 404 |
| Illegal activate (Amina) | 409 |
| Validation blank/email | 400 |
| Unexpected bug | 500 |

## Conflict choice reason
Illegal transitions are not client‑format errors (400) and not missing resources (404). They are business‑rule conflicts — the client asked for something structurally valid but semantically impossible.

## Never
Never return 200/201 on failures; never leak stack traces or internal exception names in the payload.

## Scope
Pre-lab only.

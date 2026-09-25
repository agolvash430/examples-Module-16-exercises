# Lab 16 — Correlation on Every Error

## Success path
CorrelationId is accepted from the inbound header and passed through unchanged in the success response.

## Failure path
Every error payload must include the same correlationId so the client can trace the failing request end‑to‑end.

## Missing header policy
If the client omits the correlation header, generate a synthetic correlationId server‑side and return it in both success and error responses.

## Scope
Pre-lab only.

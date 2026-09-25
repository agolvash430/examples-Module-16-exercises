# Lab 16 — Fill Message Hygiene TODOs

Safe not-found message: "Customer not found"
Unsafe message anti-pattern: "Customer CUS-9999 not found" (leaks identifiers / internals)

Correlation always field: Always include `correlationId` in every error payload.

Log stack trace (server)? Yes — log it privately on the server for diagnostics.

Return stack trace to client? No — never expose stack traces or internal exception names.

@ControllerAdvice live in this pre-lab? No — design only; do not implement the live handler in pre-lab.

## Scope
Pre-lab only.

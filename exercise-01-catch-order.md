# Lab 16 — Catch Order

## Step 1 — List types
Checked the exception types in my design: `IllegalArgumentException`, `NotFoundException`, and the generic `Exception` fallback.

## Step 2 — Order (top → bottom)
1. Most specific: `IllegalArgumentException`
2. Mid‑specific: `NotFoundException`
3. Least specific: `Exception`

## Step 3 — Why
Catch blocks must run from most specific to least specific so that narrower exceptions are handled correctly and not swallowed by a broad catch placed too early.

## Scope
Pre-lab only.

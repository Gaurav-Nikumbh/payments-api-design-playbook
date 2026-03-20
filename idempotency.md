# Idempotency

Idempotency ensures that repeated API requests do not create duplicate transactions.

## Why It Matters

Network retries, timeouts, or client errors can cause the same request to be sent multiple times.

Without idempotency, this may result in duplicate payments.

---

## Implementation Concept

Each request includes a unique idempotency key.

The system:

- checks if the key has already been used
- returns the previous result instead of reprocessing

---

## Example

Client sends payment request with idempotency key.

If request is retried:

- no duplicate payment is created
- same response is returned

---

## Key Rule

Idempotency is non-negotiable in payment systems.

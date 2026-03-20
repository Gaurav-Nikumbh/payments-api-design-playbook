# API Design Principles

Payment APIs must prioritize correctness over convenience.

## Core Principles

- clear and predictable request structure
- explicit validation rules
- consistent response formats
- strong error messaging

---

## Stateless vs Stateful

Payment APIs should be stateless at the interface level but backed by stateful orchestration systems.

---

## Synchronous vs Asynchronous

- synchronous APIs for request acceptance
- asynchronous processing for execution

This prevents blocking and improves reliability.

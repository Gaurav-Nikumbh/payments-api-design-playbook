# Integration Patterns

Payment APIs support multiple integration patterns.

## Common Models

- synchronous request + async processing
- webhook callbacks for status updates
- polling for transaction state

---

## Best Practice

Combine synchronous acknowledgement with asynchronous updates.

---

## Example Flow

Client sends request → API acknowledges → processing happens async → status updated via webhook

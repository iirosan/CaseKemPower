# Domain Model - RoomLight Middleware

This document identifies the key concepts and relationships for the RoomLight management system, focusing on the centralized logical control of hotel lighting.

---

## 1. Key Concepts (Nouns)

- **Administrator:** The hotel facility manager or IT staff member who configures the system.
- **Profile:** A logical template (e.g., "Standard Room") that defines how switches and lights behave (REQ-02).
- **Function:** The specific logic assigned to a control point, such as _Toggle_, _Dim_, or _Master Off_.
- **Room:** A virtual representation of a physical hotel room that receives configurations.
- **Light Entity:** The individual light device within a room that can be switched or dimmed.
- **Controller (Middleware):** The central system that manages the synchronization of profiles to rooms (REQ-03).

---

## 2. Conceptual Diagram

```text
+---------------+          +---------------+          +---------------+
| Administrator | (uses)   |  Controller   | (manages) |     Room      |
+---------------+          +---------------+          +---------------+
      |                          |                          |
      | (configures)             | (deploys to)             | (contains)
      V                          V                          V
+---------------+          +---------------+          +---------------+
|    Profile    |----------|   Function    | -------->| Light Entity  |
+---------------+ (defines) +---------------+ (triggers) +---------------+
```

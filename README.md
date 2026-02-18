# System-Architecture-Diagram

This project is a single habit tracking application designed to support daily supplement adherence through a streak based calendar interface. The system is intentionally simple, deterministic, and state driven. Every visible metric including streak count and calendar state is derived from one source of truth, the habit log dataset.

The architecture follows a unidirectional data flow model. User interaction updates state. State updates trigger recalculation of derived values. The interface re renders based on the updated state.

There is no duplicated logic and no stored streak values. All behavioral outputs are computed from normalized daily records.

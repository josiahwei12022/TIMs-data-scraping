TIM Intel Skeleton v3 (Time-aware)

This package contains only the deliverables skeleton (no real data).

Key design: time dimension is first-class across core records.

- published_at: when the source/content was published.
- event_time: when the described event occurred (if different from published).
- observed_at: when our system observed/extracted the information.
- valid_from/valid_to: effective interval of a fact in the real world.

Bi-temporal spirit: valid_* (effective time) + observed_at/_meta.created_at (transaction time).

Analytics layer is intentionally omitted in this skeleton (per project plan).


## Added in v3.1
- analytics/ skeleton (optional; derived layer)

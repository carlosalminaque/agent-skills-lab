---
name: stay-within-usage-limits
description: "Manage long agent work using actual visible usage telemetry, bounded waves and a verified resume checkpoint."
---

# Stay within usage limits

Needs: Host usage telemetry; if unavailable, report that limitation.

## Use exposed limits only

Inspect current task or account telemetry and its window identifier. Use an explicit user threshold; absent one, use a conservative 95% threshold for an exposed active limit. Never infer hidden tokens, billing or reset times.

- Valid: record the actual exposed percentage and window.
- Invalid: invent an account reset from elapsed time.

## Bound waves and pause safely

Recheck between substantial waves. At the threshold, stop new work and collect safe in-flight work. Save completed work, remaining actions, proof steps and the exact telemetry check needed to resume. Do not create monitoring without user authorization.

- Valid: save a resume packet and inspect usage again before the next wave.
- Invalid: start new workers after the threshold or create an unsolicited recurring job.

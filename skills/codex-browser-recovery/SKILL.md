---
name: codex-browser-recovery
description: "Recover an uncontrollable visible Codex browser by discovering the supported runtime and exact backend, then resume the original task."
---

# Codex browser recovery

Needs: Codex browser control runtime and the intended browser tab.

## Discover the real control channel

Read the installed browser tool documentation, initialize its supported runtime, enumerate browser backends and bind the exact returned backend identifier. Do not assume a literal backend name.

- Valid: select the discovered in-app backend and inspect its current tabs.
- Invalid: conclude the browser is unavailable from one stale binding.

## Verify session state on the exact tab

Match URL and title, then inspect current visible content before reporting authentication state. Embedded and extension browsers can have different sessions.

- Valid: report the sign-in page observed in the intended backend.
- Invalid: call an embedded tab logged out because an API request failed.

## Resume and preserve security

Resume the original task after recovery. If the required backend remains absent, report its inventory and exact error. Do not extract cookies or credentials or bypass user-only security checks.

- Valid: continue at the saved checkpoint after rebinding.
- Invalid: scrape a token to bypass a security prompt.

---
name: user-basic-tooling-unfamiliar
description: User is unfamiliar with basic Windows GUI tools (didn't know what Notepad is) — prefer single-command copy-paste solutions over multi-step GUI walkthroughs
metadata:
  type: user
---

User did not recognize "Notepad" (Bloco de Notas) when given manual GUI steps to create a file. **Why:** signals lower general computer-literacy / limited experience with basic OS tools, not just unfamiliarity with dev-specific tooling — plain jargon like app names shouldn't be assumed known. **How to apply:** default to the simplest single-command solution (e.g. a PowerShell one-liner run via the `!` chat prefix) instead of multi-step GUI instructions whenever one exists. If a GUI walkthrough is unavoidable, explain each UI element/app in plain terms rather than assuming familiarity.

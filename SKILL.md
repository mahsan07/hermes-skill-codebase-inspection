---
name: hermes-skill-codebase-inspection
description: Measure a codebase’s size, languages, and composition without changing it. Use when a user asks for this workflow or a closely related task.
---

# Codebase Inspection

Inspect repositories with read-only analysis. Produce evidence-backed summaries of languages, line counts, file distribution, dependency surfaces, and unusually large or risky areas.

## Workflow

1. Confirm the repository root and ignore generated, vendor, build, and secret-bearing paths.
2. Inventory files and languages; use `pygount` when available and record the command.
3. Identify entry points, tests, configuration, scripts, and deployment files.
4. Report counts and ratios with paths that a maintainer can verify.
5. Separate measured facts from inferences.

Never print secret contents, tokens, private keys, or full environment files.

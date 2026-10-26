---
name: bug-bounty
description: Entry-point alias for the canonical in-repository bug bounty skill; route only explicitly scoped, authorized tasks.
---

# Bug Bounty entry point — one source of truth

The full methodology lives in [skills/bug-bounty/SKILL.md](skills/bug-bounty/SKILL.md). This root file is a **non-recursive alias**, not a second workflow. Read the canonical skill **once if applicable**; do not reload this root file from the canonical skill.

For permission/scope/stop rules and WIP=1 use [AGENTS.md](AGENTS.md). Selection: bug-bounty main for general guidance; a single specialist in `skills/*/SKILL.md` for a known narrower task; `skills/triage-validation/SKILL.md` only when validating a finding; `skills/report-writing/SKILL.md` only when drafting a requested report. Do not automatically run recon, exploit probes, credential tests, reports or continuous monitoring just because this skill was loaded.

**Outcome:** deliver the user's specific requested result and stop. Document actual runs separately from examples, plans and hypothetical findings.

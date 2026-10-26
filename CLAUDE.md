# Claude Code adapter — Agentic-Bug-Hunter

**Canonical agent instructions:** [AGENTS.md](AGENTS.md). Read and apply that file for scope, authorization, evidence, execution, non-duplication, and completion. This adapter must not repeat, contradict, or override its safeguards.

## Claude-specific routing

- For Claude Code start with `claude` in an explicitly approved local checkout. Commands and skills are only available if the plugin is actually installed; do not infer capability from documentation.
- Use an applicable command such as `/recon`, `/hunt`, `/validate` or `/report` **only when relevant to the current task**. `skills/bug-bounty/SKILL.md` is the master methodology; `skills/bb-methodology/SKILL.md` is advisory. Select one specialist skill for the active lead instead of chaining all skill files.
- Refer to [tools/README.md](tools/README.md) for concrete installed tool interfaces; verify availability before invoking. Claude-specific settings reside under `.claude/`, while `OPENCODE.md` documents a different harness.
- Follow the target program's precise authorization/scope and request-rate constraints. Use benign/synthetic proof whenever possible; live validation requires the owner's authorization and a bounded impact hypothesis.
- Preserve one evidence and outcome record per verified lead; reuse the existing lead board instead of creating duplicate recon inventories or repeated reports.

**Do not treat this text as a command to run scanning tools.** If the user asked for a review, documentation correction, or local code fix, complete exactly that task without network probing. On completion use the concise result contract from `AGENTS.md` and stop when Done.

# Agentic-Bug-Hunter — SecurityWorkspace portfolio boundary (2026-11-14)

**Scope:** GitHub source-tree/README/manifest review only, without code execution or network-credential testing. Not a production attestation. [Central evidence-backed matrix](https://github.com/devwebsec/DESIGN-BY-SECURITY/blob/docs/portfolio-dependency-graph-20261114/docs/SECURITYWORKSPACE-CROSS-REPO-DEPENDENCY-AUDIT-20261114.md).

## Source/provenance and capabilities

- The root README retains AwareXone branding, upstream badges and support/installation notes. There is no evidence in the reviewed main tree of a source-to-Wazuh production authority contract.
- `requirements.txt` declares `requests>=2.31.0`, `pytest>=8.0.0` without an upper-bound/lock file. Runtime compatibility, supply-chain provenance and SCA **NOT VERIFIED** by this documentation-only audit.
- This repo **is not a third SecurityWorkspace operational agent**; do not give its commands implicit read access to Wazuh, production Gitea, Vaultwarden or Fleet.
- Its independent PR #1 is open; no merge or code modifications are authorized by portfolio documentation.

## Relationships / non-inheritance

- [DESIGN-BY-SECURITY](https://github.com/devwebsec/DESIGN-BY-SECURITY) owns design/governance, but sharing a GitHub account does **not** establish CI import, runtime calls, API tokens or deployment.
- [WAZUH](https://github.com/devwebsec/WAZUH) host L3 Hotfix002 `deployment/smoke/SOAK10=PASS` is operator-reported and separate; `LIVE_E2E=NOT_ATTESTED`. This repository has **no attested production Wazuh dependency**.
- [Security Copilot](https://github.com/devwebsec/security-copilot-local-agent) and [Developer Copilot](https://github.com/devwebsec/developer-coding-copilot-local-agent) are independently scoped, not inherited SDKs or approval authorities.
- GitHub Project #1 membership, Gitea mirror, GitHub About metadata and transitive dependency vulnerabilities were not verified in this review.

## Proposed GitHub About description (not applied)

> Независимый bug-bounty toolkit AwareXone-style; интеграция с SecurityWorkspace/Wazuh не подтверждена.

**Decision:** preserve repository history. Mark unsupported statements `HISTORICAL/UNVERIFIED`, require owner-reviewed source+CI changes before a claim of PASS. No merge, clean-up, rebranding, or auto-archive performed.

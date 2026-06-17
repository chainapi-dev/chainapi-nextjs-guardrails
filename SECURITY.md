# Security Policy

## Supported versions

Only the most recent release of the ChainAPI Anti-Debt Guardrails pack is actively
supported with security corrections.

| Version | Supported |
|---------|-----------|
| 1.x (latest) | ✅ Yes |
| < 1.0 | ❌ No |

---

## What counts as a security issue here

This repository contains Cursor rule files (`.mdc`) and agent context files
(`AGENTS.md`, `CLAUDE.md`). A security issue means:

- A **security rule that incorrectly permits a dangerous pattern** — for example,
  `400-security-boundaries.mdc` allowing string-interpolated SQL, or
  `402-owasp-auditor.mdc` missing a known OWASP Top 10 injection vector.
- A **`NEVER Do` boundary in `AGENTS.md` that inadvertently allows harmful agent
  behavior** — for example, a missing prohibition on executing shell commands with
  user-supplied input.
- A **CI workflow vulnerability** — for example, the `validate-mdc.yml` workflow
  being exploitable via a malicious `.mdc` filename or content injection.

It does **not** cover:
- Codebases that use these rules (those are the buyer's responsibility).
- AI models generating insecure code despite the rules being active (report to
  the relevant AI provider).

---

## Reporting a vulnerability

**Do not open a public GitHub issue for security vulnerabilities.**

Report privately using GitHub's built-in security advisory feature:

> **Repository → Security tab → "Report a vulnerability"**

Or email: **security@chainapi.dev**

Include:
- The specific file and directive that contains the issue
- A concrete code example demonstrating the incorrect behavior
- The version of the pack affected

We aim to:
- Acknowledge receipt within **48 hours**
- Provide a fix or workaround within **7 days** for confirmed issues
- Credit reporters in the CHANGELOG unless they prefer to remain anonymous

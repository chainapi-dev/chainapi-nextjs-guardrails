# Changelog

All notable changes to the ChainAPI Next.js & React Anti-Debt Guardrails pack.

Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html)

---

## [Unreleased]

---

## [1.0.0] — 2025-07-01

### Added

**17 scope-controlled Cursor `.mdc` rule files:**

- `000-core-stack.mdc` — TypeScript strict, Python 3.12+, zero AI conversational output
- `001-output-optimization.mdc` — Token economy, differential output, no pleasantries
- `100-anti-debt-enforcer.mdc` — Typed errors, explicit imports, structured logging
- `101-state-management.mdc` — Zustand/TanStack, immutable updates, granular selectors
- `102-dry-principles.mdc` — AHA principle, magic string isolation, pure utilities
- `200-nextjs-app-router.mdc` — RSC by default, App Router only, typed routes
- `201-react-components.mdc` — Functional-only, interface-typed props, exhaustive deps
- `202-tailwind-mastery.mdc` — Utility-first, cn() merging, design-token extension
- `300-api-contract-zod.mdc` — Zod boundary parsing, single-source types, .strict() schemas
- `301-database-migrations.mdc` — Zero-downtime expand/contract, CONCURRENTLY indexes
- `302-async-performance.mdc` — Promise.all(), no sequential awaits, p-map batching
- `400-security-boundaries.mdc` — Auth-first, parameterized queries, no hardcoded keys
- `401-webhook-security.mdc` — HMAC verification, raw body, idempotent event processing
- `402-owasp-auditor.mdc` — OWASP Top 10, Argon2, path traversal prevention
- `500-tdd-vitest.mdc` — AAA structure, behavioral test names, scoped mock lifecycle
- `501-playwright-e2e.mdc` — Semantic locators, no waitForTimeout, isolated test state
- `600-deployment-preflight.mdc` — SHA-pinned images, Zod env parsing, pre-deploy migrations

**Agent context files:**

- `AGENTS.md` — Three-Tier Linux Foundation model (Always Do / Ask First / Never Do), verified under 150-line hard limit
- `CLAUDE.md` — WHAT-WHY-HOW framework with Claude Code three-layer merging model explicitly documented
- `README.md` — Full onboarding guide with NeurIPS / CMU SEI academic citations and token-scope table

**Repository infrastructure:**

- Free preview rules in `/preview/`: `000-core-stack.mdc`, `001-output-optimization.mdc`
- `.github/workflows/validate-mdc.yml` — CI frontmatter linter (recursive glob check, required key check)
- GitHub issue templates: bug report and feature request (`.yml` form format)
- Pull request template with scope-limiting checklist
- `CONTRIBUTING.md`, `SECURITY.md`, `LICENSE` (MIT preview + commercial notice)

### QA baseline

- All 17 rule glob patterns verified recursive (`["**/*.ext"]` format — no bare `"*"`)
- All 17 rules confirmed to include `## Anti-Patterns (NEVER do these)` with ❌/✅ snippets
- `AGENTS.md` verified at 60 lines (well under 150-line inference cost limit)
- `alwaysApply: true` confirmed on `000`, `001`, `102`, `400`, `402` (cross-cutting concerns)
- `alwaysApply: false` confirmed on all scope-specific rules

---

[Unreleased]: https://github.com/chainapi/chainapi-nextjs-guardrails/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/chainapi/chainapi-nextjs-guardrails/releases/tag/v1.0.0

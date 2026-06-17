<p align="center">
  <img src=".github/assets/logo.png" alt="ChainAPI" width="280" />
</p>

<h1 align="center">ChainAPI Next.js & React Anti-Debt Guardrails</h1>

<p align="center">
  17 scope-controlled Cursor rules that stop AI from accumulating technical debt in your Next.js codebase.
</p>

<p align="center">
  <a href="https://chainapi.gumroad.com/l/chainapi-nextjs-guardrails">
    <img src="https://img.shields.io/badge/Get%20Full%20Pack-%2447-6366f1?style=flat-square" alt="Gumroad" />
  </a>
  <img src="https://img.shields.io/badge/Cursor%20Rules-17%20files-6366f1?style=flat-square" alt="17 rules" />
  <img src="https://img.shields.io/badge/TypeScript-strict-3178c6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Preview-MIT-22c55e?style=flat-square" alt="MIT" />
  <img src="https://img.shields.io/badge/Full%20Pack-Commercial-f59e0b?style=flat-square" alt="Commercial" />
</p>

---

## Why this exists

AI coding assistants ship features fast. They also ship:

- Props typed as `any` with zero compiler enforcement
- Empty `catch (e) {}` blocks swallowing production errors silently
- Sequential `await` chains where `Promise.all()` would run 2â€“3Ã— faster
- `req.body as MyType` â€” zero runtime validation on untrusted API payloads
- `"use client"` on page-level layouts, disabling every RSC optimization
- SQL queries assembled by string concatenation

Research published at NeurIPS and cited by Carnegie Mellon's SEI quantifies this:

> **Unguarded AI code generation correlates with a 41% increase in structural
> complexity and a 30% surge in static analysis warnings in production codebases.**

The AI is not the problem. Missing constraints are.

---

## What's in the full pack

17 rules across five layers. Every rule ends with an Anti-Patterns section â€”
concrete Wrong / Right code snippets, because AI agents learn from examples.

### Core Layer â€” active on every file
| File | Enforces |
|------|----------|
| `000-core-stack.mdc` | TypeScript strict, Python 3.12+, zero AI filler output |
| `001-output-optimization.mdc` | Token economy, differential output, no preambles |
| `102-dry-principles.mdc` | AHA principle, magic string isolation, pure utilities |

### React & Next.js Layer â€” tsx/jsx/ts files
| File | Enforces |
|------|----------|
| `200-nextjs-app-router.mdc` | RSC by default, App Router only, typed routes |
| `201-react-components.mdc` | Functional-only, interface-typed props, exhaustive deps |
| `202-tailwind-mastery.mdc` | Utility-first, cn() merging, design-token extension |
| `101-state-management.mdc` | Zustand/TanStack separation, immutable updates |

### Backend & Data Layer â€” ts/py files
| File | Enforces |
|------|----------|
| `100-anti-debt-enforcer.mdc` | Typed errors, explicit imports, structured logging |
| `300-api-contract-zod.mdc` | Zod boundary parsing, single-source types, .strict() |
| `301-database-migrations.mdc` | Zero-downtime expand/contract, CONCURRENTLY indexes |
| `302-async-performance.mdc` | Promise.all(), no sequential awaits, p-map batching |

### Security Layer â€” always active
| File | Enforces |
|------|----------|
| `400-security-boundaries.mdc` | Auth-first, parameterized queries, no hardcoded keys |
| `401-webhook-security.mdc` | HMAC verification, raw body, idempotent events |
| `402-owasp-auditor.mdc` | OWASP Top 10, Argon2, path traversal, no eval() |

### Quality & Deployment Layer
| File | Enforces |
|------|----------|
| `500-tdd-vitest.mdc` | AAA structure, behavioral test names, scoped mocks |
| `501-playwright-e2e.mdc` | Semantic locators, no waitForTimeout, isolated state |
| `600-deployment-preflight.mdc` | SHA-pinned images, Zod env parsing, pre-deploy migrations |

**[â†’ Get the full pack on Gumroad ($19)](https://chainapi.gumroad.com/l/chainapi-nextjs-guardrails)**

---

## Free preview â€” try in 30 seconds

```sh
mkdir -p .cursor/rules

curl -sO --output-dir .cursor/rules \
  https://raw.githubusercontent.com/chainapi/chainapi-nextjs-guardrails/main/preview/000-core-stack.mdc

curl -sO --output-dir .cursor/rules \
  https://raw.githubusercontent.com/chainapi/chainapi-nextjs-guardrails/main/preview/001-output-optimization.mdc
```

Or clone and copy:

```sh
git clone https://github.com/chainapi/chainapi-nextjs-guardrails
cp chainapi-nextjs-guardrails/preview/*.mdc .cursor/rules/
```

---

## Glob scoping protects your token budget

| Task | Rules loaded | Rules saved |
|------|-------------|-------------|
| Editing a Playwright test | 4 rules | 13 |
| Editing a Prisma schema | 4 rules | 13 |
| Writing a Zod API route | 6 rules | 11 |
| Editing a GitHub Actions workflow | 3 rules | 14 |

---

## Full pack installation

```sh
mkdir -p .cursor/rules
cp SaaS_AntiDebt_Mega_Pack/.cursor/rules/*.mdc .cursor/rules/
cp SaaS_AntiDebt_Mega_Pack/AGENTS.md SaaS_AntiDebt_Mega_Pack/CLAUDE.md .

touch CLAUDE.local.md
echo "CLAUDE.local.md" >> .gitignore
```

---

## References

[1] Sculley, D., et al. (2015). *Hidden Technical Debt in Machine Learning Systems.* NeurIPS 28.
[2] Tamburri, D.A. (2020). *Sustainable Architectures for AI Pipelines.* IEEE SEI Technical Report.

---

<p align="center">
  Built by <strong>ChainAPI</strong> &nbsp;Â·&nbsp;
  <a href="https://chainapi.gumroad.com/l/chainapi-nextjs-guardrails">Get the full pack â†’</a>
</p>
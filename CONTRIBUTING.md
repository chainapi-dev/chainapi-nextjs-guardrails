# Contributing

Thank you for your interest in ChainAPI Next.js & React Anti-Debt Guardrails.

## This is a commercial product

The 17 rule files in the full pack are a paid commercial product and are not
open for public contribution. The two preview rules in `/preview/` are MIT-licensed
and open for community fixes.

---

## What we accept

**Bug reports**
Incorrect frontmatter, broken glob patterns, conflicting rule directives, or
anti-pattern code snippets that contain errors. Use the [bug report template](.github/ISSUE_TEMPLATE/bug_report.yml).

**Rule suggestions**
Ideas for new anti-patterns, missing coverage in an existing rule, or improvement
to AGENTS.md or CLAUDE.md directives. Use the [feature request template](.github/ISSUE_TEMPLATE/feature_request.yml).

**Documentation fixes**
Typos, broken links, outdated install instructions, or unclear README sections.
Open a PR directly for these — no issue required.

**CI improvements**
Enhancements to the `.github/workflows/validate-mdc.yml` frontmatter validator.

---

## What we do not accept

- Pull requests that modify the logic or content of the commercial rule files
- PRs that add new `.mdc` files to the repository
- Requests to open-source the full 17-rule pack
- Issues asking for refunds — direct those to Gumroad support

---

## Opening a pull request

1. Fork the repository and create a branch from `main`.
2. Make your change. Keep it scoped — one fix per PR.
3. Confirm the `validate-mdc.yml` workflow passes locally if you touch any `.mdc` files:
   ```sh
   python3 .github/workflows/validate-mdc.yml  # or run the CI action
   ```
4. Fill out the pull request template completely.
5. Open the PR against `main`.

---

## Code of conduct

Be direct, be specific, and be kind. Issues and PRs that are vague, abusive, or
off-topic will be closed without discussion.

For anything not covered here, reach out via X: [@ChainAPI](https://x.com/chainapi)

# scanaislop.com

**AI slop detector and deterministic quality gate for AI coding agents.**

[![aislop on npm](https://img.shields.io/npm/v/aislop.svg?label=aislop)](https://www.npmjs.com/package/aislop)
[![npm downloads](https://img.shields.io/npm/dm/aislop.svg)](https://www.npmjs.com/package/aislop)
[![GitHub Actions](https://github.com/scanaislop/aislop/actions/workflows/ci.yml/badge.svg)](https://github.com/scanaislop/aislop/actions/workflows/ci.yml)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/scanaislop/aislop/blob/main/LICENSE)

[`scanaislop.com`](https://scanaislop.com) is the product home for the
open-source
[`aislop`](https://github.com/scanaislop/aislop) CLI and hosted quality
platform for engineering teams using Claude Code, Cursor, Codex, Copilot,
OpenCode, Windsurf, and other AI coding agents.

The problem is simple: AI-generated code can pass tests, lint, and review while
still leaving behind swallowed exceptions, `as any` casts, hallucinated imports,
duplicated helpers, dead code, TODO stubs, oversized functions, hardcoded
values, and security risks. `aislop` catches those repeatable patterns with
deterministic static analysis. No LLM runs in the scan path.

## Run an AI Slop Scan

From any project root:

```bash
npx aislop scan
```

For a fresh one-off run against the latest npm release:

```bash
npx aislop@latest scan
```

Useful variants:

```bash
npx aislop@latest scan --changes      # scan files changed from HEAD
npx aislop@latest scan --staged       # scan staged files before commit
npx aislop@latest scan --json         # machine-readable output
npx aislop@latest scan --sarif        # GitHub code scanning output
npx aislop@latest fix                 # auto-fix safe mechanical issues
npx aislop@latest ci                  # CI mode with thresholded exit code
npx aislop@latest hook install        # install per-edit agent quality hooks
```

Prefer a pinned local install for CI and repeatable team workflows:

```bash
npm install --save-dev aislop
npx aislop ci
```

## What aislop Catches

- AI slop in agent-written code: narrative comments, trivial wrappers, fake
  completeness, and over-broad fallbacks.
- Code quality issues that survive normal linting: dead code, duplicated
  helpers, generic naming, oversized functions, and unused dependencies.
- TypeScript, JavaScript, Python, Go, Rust, Ruby, and PHP findings across 50+
  deterministic rules.
- Security and reliability risks: swallowed exceptions, hardcoded secrets,
  dangerous `eval`, SQL injection patterns, and unsafe type escapes.
- Pull request and CI/CD regressions before they become production technical debt.

## Links

| Resource | Link |
| --- | --- |
| Open-source CLI | [github.com/scanaislop/aislop](https://github.com/scanaislop/aislop) |
| npm package | [npmjs.com/package/aislop](https://www.npmjs.com/package/aislop) |
| Website | [scanaislop.com](https://scanaislop.com) |
| Documentation | [scanaislop.com/docs](https://scanaislop.com/docs) |
| CI/CD guide | [scanaislop.com/docs/ci](https://scanaislop.com/docs/ci) |
| Rules reference | [scanaislop.com/docs/rules](https://scanaislop.com/docs/rules) |
| Changelog | [scanaislop.com/changelog](https://scanaislop.com/changelog) |
| Blog | [scanaislop.com/blog](https://scanaislop.com/blog) |
| Discussions | [github.com/scanaislop/aislop/discussions](https://github.com/scanaislop/aislop/discussions) |
| Agent skill | [github.com/scanaislop/skills](https://github.com/scanaislop/skills) |

## Keywords

AI slop detector, AI code review, AI-generated code, AI coding agents, agentic
coding, vibe coding, static analysis, code quality CLI, pull request quality
gate, pre-commit hook, GitHub Actions CI, CI/CD code quality, TypeScript
linter, Python code quality, secure code scanning, technical debt detection.

## Why Teams Use It

AI coding tools move fast. Review capacity does not. `aislop` gives teams a
consistent merge bar for agent-written changes: scan, score, fix what is
mechanical, and hand the remaining findings back to the coding agent or reviewer
with concrete diagnostics.

Same code in, same score out. Sub-second on typical projects. MIT-licensed.
Built for local development, pre-commit checks, pull requests, and CI.

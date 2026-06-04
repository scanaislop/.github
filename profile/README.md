# scanaislop.com

**Scan your code for AI slop before it reaches production.**

[![aislop on npm](https://img.shields.io/npm/v/aislop.svg?label=aislop)](https://www.npmjs.com/package/aislop)
[![npm downloads](https://img.shields.io/npm/dm/aislop.svg)](https://www.npmjs.com/package/aislop)
[![GitHub Actions](https://github.com/scanaislop/aislop/actions/workflows/ci.yml/badge.svg)](https://github.com/scanaislop/aislop/actions/workflows/ci.yml)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/scanaislop/aislop/blob/main/LICENSE)

[`scanaislop.com`](https://scanaislop.com) is the product home for
[`aislop`](https://github.com/scanaislop/aislop), the open-source AI slop
detector and deterministic quality gate for AI-generated code.

`aislop` helps teams using Claude Code, Cursor, Codex, Copilot, OpenCode,
Windsurf, and other AI coding agents catch repeatable problems before they
reach pull requests, CI, or production.

## Scan Your Code for AI Slop

Run this from any project root:

```bash
npx aislop scan
```

## What aislop Catches

- Agent-written code that looks finished but carries hidden quality debt.
- Narrative comments, TODO stubs, duplicated helpers, and dead code.
- Swallowed exceptions, unsafe type escapes, hallucinated imports, and oversized
  functions.
- Security and reliability risks that normal linting can miss.

Same code in, same score out. No LLM runs in the scan path.

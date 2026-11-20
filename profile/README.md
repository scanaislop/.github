# Scan AI Slop

[aislop](https://github.com/scanaislop/aislop) is an open-source code-quality scanner for teams using AI coding agents. It flags problems such as swallowed exceptions, duplicated helpers, and unsafe type casts. Each finding points to the code that triggered it.

## Run your first scan

From your project root, run the CLI with Node.js 20 or later.

```sh
npx aislop@latest scan
```

Review the findings locally, install an agent hook to check edits as you work, or run the same checks on pull requests. The scanner uses deterministic rules and runs without an LLM.

- [Language support](https://github.com/scanaislop/aislop#language-support) lists the supported targets, including Scala (beta).
- [Installation](https://github.com/scanaislop/aislop#installation) covers npm, Bun, Yarn, Homebrew, and Python.
- [Agent skills](https://github.com/scanaislop/skills) help your coding agent act on findings.
- [Documentation](https://docs.scanaislop.com) covers rules, configuration, and CI.

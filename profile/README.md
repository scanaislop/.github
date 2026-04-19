# scanaislop

**The code-quality gate for teams shipping AI-assisted code to production.**

AI agents write code that compiles, passes tests, and still ships broken — narrative comments, `as any` casts, swallowed errors, duplicate logic, dead exports, template-string SQL. scanaislop exists to catch that before it reaches production, so your team can ship AI-assisted code without inheriting its slop.

## What we ship

| | What | Where |
|---|---|---|
| **aislop** | Open-source CLI. Scans a project across six engines (format, lint, code-quality, ai-slop, security, architecture), scores it 0–100, auto-fixes the mechanical findings, hands the rest to your coding agent. MIT. | [scanaislop/aislop](https://github.com/scanaislop/aislop) |
| **aislop-skill** | Drop-in agent skill. Installs aislop as a code-quality gate and coding guardrail in Claude Code, Cursor, Codex, Gemini CLI, Windsurf, Cline, and 40+ more agents. MIT. | [scanaislop/aislop-skill](https://github.com/scanaislop/aislop-skill) |
| **scanaislop** | Hosted platform. PR gates on every repo, standards hierarchy (org → team → project), per-team dashboards, agent attribution, visual rules manager. | [scanaislop.com](https://scanaislop.com) |

## Start here

```bash
# score any project in a couple of seconds
npx aislop scan

# turn aislop into a skill every coding agent runs per turn
npx skills add scanaislop/aislop-skill
```

## Links

- [scanaislop.com](https://scanaislop.com) — product overview
- [Docs](https://scanaislop.com/docs) — commands, configure, agent handoff, skill install, CI gate
- [Blog](https://scanaislop.com/blog) — essays on shipping AI-assisted code without the slop
- [Pricing](https://scanaislop.com/pricing)
- [Changelog](https://scanaislop.com/changelog)

## Languages supported

TypeScript · JavaScript · Python · Go · Rust · Ruby · PHP · Expo / React Native

## License

The CLI (`aislop`) and the agent skill (`aislop-skill`) are MIT. The hosted platform is proprietary.

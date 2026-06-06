# scanaislop.com

This repository controls the public GitHub organization profile for
[`scanaislop.com`](https://scanaislop.com). It is not the main source
repository for the product.

The profile that appears on the organization page is
[`profile/README.md`](profile/README.md). That is the most important public
surface in this repository.

## Main Project

[`aislop`](https://github.com/scanaislop/aislop) is the open-source CLI behind
scanaislop.com. It scans AI-generated code for repeatable quality issues before
they reach pull requests, CI, or production.

Run this from any project root, no install required:

```bash
npx aislop scan
```

Prefer a persistent install? `brew install scanaislop/tap/aislop` or `pipx install aislop`, then run `aislop scan`.

Use [`scanaislop/aislop`](https://github.com/scanaislop/aislop) for source
code, issues, releases, and installation details. Use
[`scanaislop.com`](https://scanaislop.com) for the public product site.

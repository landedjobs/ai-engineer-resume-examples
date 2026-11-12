# Contributing

Thanks for helping improve this collection of AI engineer resume examples. Contributions are welcome, and they clear a quality bar. This file is that bar.

Maintained by [Landed](https://www.landed.jobs/?utm_source=github&utm_medium=referral&utm_campaign=github-ai-engineer-resume-examples&utm_content=contributing). No affiliation with any company or tool named in this repo.

---

## What we accept

- **Example resumes** for roles we don't cover yet (AI infra engineer, AI researcher moving to industry, AI solutions architect, AI safety engineer). See [`examples/`](examples/).
- **Bullets** for the [bullet banks](bullets/), in the formula: action, what you built, scale or number, outcome.
- **Before/after rewrites** for the table in the [README](README.md#before-and-after-20-bullet-rewrites).
- **Template fixes** that keep the [templates](templates/) single column and ATS-friendly.
- **Fixes**: broken links, unclear advice, stale facts about hiring or tools.

## The non-negotiables

### 1. Example people are fictional

Every example resume uses a fictional person, fictional employers and fictional schools. Never submit your own resume, a friend's, or anything derived from a real person's private data. Use `example.com` for emails and sites and `(555) 010-xxxx` style phone numbers. Mark each example file with the fictional-person note at the top.

### 2. Numbers are plausible for the level

A junior engineer doesn't save $6M a year. A staff engineer's bullets show scope across teams. If a number would make an experienced hiring manager raise an eyebrow, change it.

### 3. Bullets use the formula and placeholders

Bullet bank entries use `[N]`, `[X%]`, `[A]`/`[B]` placeholders so readers fill in their own numbers. One idea per bullet. No bullet without a measurable outcome or scope.

### 4. Style

- Plain words. No "spearheaded synergies", no "passionate", no "leveraged cutting-edge AI".
- Sentence case headings, straight quotes, no em dashes.
- Tables over prose for anything comparable.
- Every example ends with "why this works" and "what to change" for a lab, a startup and an enterprise.

### 5. License discipline

This repo ships **MIT** (see [`LICENSE`](LICENSE)). Don't paste resume text or templates from other sources unless their license is MIT, Apache-2.0 or CC0, and credit them. When in doubt, write it fresh.

## How to contribute

1. Open an issue using a [template](.github/ISSUE_TEMPLATE/), or go straight to a PR for small fixes.
2. Fork, branch, edit.
3. Keep internal links relative (`../bullets/evals.md`) and check they resolve. CI runs [lychee](.github/workflows/links.yml) on every PR.
4. Open a PR and fill in the [PR checklist](.github/PULL_REQUEST_TEMPLATE.md).

## Example file format

```markdown
# Example NN: <role> (<level>)

> **Fictional person.** <Name>, their employers and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** ... **Target roles:** ... **Background:** ...

---

## The resume

...

---

## Why this works

- ...

## What to change for each kind of employer

**Frontier lab.** ...

**Startup.** ...

**Enterprise.** ...
```

## Recognition

Contributors are credited in release notes.

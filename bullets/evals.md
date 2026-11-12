# Bullet bank: evals

20 bullets for evaluation, testing and quality work on LLM systems. Hiring managers read these first in 2026. Replace every `[placeholder]` with your own numbers and nouns.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values.

1. Built the eval harness (golden sets, automated metrics, LLM-as-judge) that gates every prompt and model change across [N] services.
2. Wrote a [N]-example golden set with [domain experts / support leads / customers], now the acceptance test for [feature].
3. Calibrated an LLM judge to [X%] agreement with human labels on [N] examples, replacing [N] hours a week of manual review.
4. Added eval runs to CI so every pull request touching prompts reports a per-category score diff; [N] changes shipped through it with no quality regressions reaching users.
5. Built online evals that score [X%] of production traffic for [groundedness / relevance / policy], catching a regression within [N] hours of a deploy.
6. Turned [N] production failures into regression tests within a week of each incident, growing the eval set from [A] to [B] cases.
7. Measured inter-annotator agreement on the labeling guide and rewrote it, raising agreement from [A] to [B] before using the labels for evaluation.
8. Ran a model comparison across [N] models on [N] tasks with cost and latency, leading to a switch that cut cost [X%] at equal quality.
9. Built a red-team set of [N] adversarial prompts ([injection, jailbreak, PII extraction]) run weekly against [product].
10. Designed pass@k and pass^k metrics for the agent eval to separate "can it ever" from "does it reliably", changing the launch decision for [feature].
11. Set up human review sampling of [X%] of outputs with a structured rubric, feeding a weekly quality report to [N] teams.
12. Found that the existing eval set over-represented easy cases; rebalanced it to match production traffic, which revealed a [X%] gap on [category] that we then fixed.
13. Built a hallucination check that verifies each factual claim against retrieved sources, cutting unsupported claims from [A]% to [B]%.
14. Created synthetic test data for [rare cases] with [method], validated against [N] real examples, adding [N] cases to the eval set.
15. Defined launch criteria for AI features (target score, max failure rate, cost ceiling) adopted as the standard by [N] teams.
16. Built an eval dashboard tracking quality, cost and latency per release, used in every [weekly / release] review.
17. Ran a [N]-week A/B test comparing [prompt / model / retrieval] variants on [metric], with offline evals predicting the winner correctly.
18. Reduced eval run time from [A] minutes to [B] minutes by caching model outputs and parallelizing, so engineers run it before every change.
19. Built task-specific metrics (field-level F1, citation precision, tool-call accuracy) to replace a single generic quality score.
20. Published an open eval set of [N] examples for [domain], used by [N] external projects.

# Bullet bank: agents and tool use

25 bullets for agents, tool calling, workflows and MCP. Replace every `[placeholder]` with your own numbers and nouns.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values.

1. Shipped a tool-using agent that [reconciles invoices / resolves support tickets / triages alerts] across [N] systems, completing [X%] of cases end to end.
2. Rebuilt a single-prompt bot as a planner with [N] tools, raising task completion from [A]% to [B]% on [N] replayed real conversations.
3. Designed tool schemas and descriptions for [N] tools, cutting wrong-tool calls from [A]% to [B]% in traced production runs.
4. Capped agent runs at [N] steps with a graceful hand-off to a human, removing runaway loops that had cost [$N] in a single week.
5. Added a confirmation step before irreversible actions ([refunds / writes / emails]), with zero unintended actions across [N]K runs since launch.
6. Built an MCP server exposing [N] internal tools ([search, tickets, billing]) to [N] agent clients, with per-tool auth and audit logging.
7. Replaced a free-form agent with a fixed workflow for the [X%] of requests that follow a known path, cutting cost by [Y%] and failure rate by [Z%].
8. Built trajectory evals that score both the outcome and each tool call on [N] scenarios, catching [N] regressions before release in [period].
9. Added retry and fallback logic for flaky downstream APIs, raising agent success during [provider] incidents from [A]% to [B]%.
10. Cut median agent run time from [A]s to [B]s by running independent tool calls in parallel.
11. Built a sandboxed code-execution tool for the agent with [CPU / memory / network] limits, used in [N]K runs a week with no escapes in red-team testing.
12. Implemented long-term memory for a [assistant / agent] using [summaries / a profile store], raising returning-user task success by [X%].
13. Hardened the agent against prompt injection from [web pages / uploaded files / emails] with input sanitization and tool permission tiers; blocked [X%] of a [N]-case red-team set.
14. Built a multi-agent setup ([planner, researcher, writer]) for [task], then measured it against a single agent and kept the simpler one, which scored [X%] higher at [Y%] lower cost.
15. Added human-in-the-loop review for low-confidence actions, routing [X%] of runs to reviewers and keeping the error rate on executed actions under [Y%].
16. Instrumented every agent run with traces (inputs, tool calls, outputs, cost), cutting time to diagnose a failed run from [A] to [B].
17. Built a browser-use agent that completes [task] on [N] sites, with a [X%] success rate on a [N]-task benchmark we built from real requests.
18. Designed the agent's state and resume logic so long tasks survive restarts; [N]-hour runs now finish at a [X%] rate, up from [A]%.
19. Built a voice agent that [books appointments / qualifies leads] over the phone, handling [N] calls a week with [X%] completion and [N]ms response latency.
20. Wrote the team's agent design guide (when to use a workflow vs an agent, tool design, step limits, evals), adopted by [N] teams.

## More bullets (Nov 2026)

These add the conditions that make a number checkable: the size of the test set, the baseline, the load and the date. Every number is still a placeholder; keep a condition only if it is true for your work. See [evaluation vocabulary to get right](README.md#evaluation-vocabulary-to-get-right) for the terms.

Last checked: 17 Nov 2026

21. Raised verified task completion from [A]% to [B]% on [N] held-out workflow cases by replacing free tool choice with typed actions, input validation and explicit recovery paths, checked against final system state.
22. Cut cost per successful agent task from [$A] to [$B] with model routing and context trimming, keeping completion above [X%] on the same [N]-case eval set.
23. Added resumable execution and idempotent tool calls to the [workflow] agent, recovering [X%] of interrupted runs and cutting duplicate external actions from [A] to [B] per [N] tasks over [period].
24. Added approval gates for [refunds / deletes / outbound email] that stopped execution in all [N] unauthorized-action tests, with median reviewer handling time under [N] seconds across [N] reviews.
25. Replaced a multi-agent prototype with a fixed workflow plus one model step, cutting p95 completion time from [A]s to [B]s with no drop in task success on [N] held-out cases.

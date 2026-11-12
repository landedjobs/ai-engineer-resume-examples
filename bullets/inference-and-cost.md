# Bullet bank: inference, latency and cost

20 bullets for serving, latency and cost work. Replace every `[placeholder]` with your own numbers and nouns.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values, `[$N]` a dollar amount.

1. Cut monthly inference spend from [$A] to [$B] by routing [X%] of traffic to a smaller model, with no drop on the quality eval.
2. Brought p95 latency of [endpoint] from [A]s to [B]s with streaming, prompt caching and parallel retrieval.
3. Cut time-to-first-token from [A]ms to [B]ms by moving static instructions into a cached prefix.
4. Self-hosted [model] on [N] [GPU type] with [vLLM / TGI / SGLang], serving [N] requests a second at [X%] of the hosted API cost.
5. Raised GPU utilization from [A]% to [B]% with continuous batching and request scheduling, cutting serving cost per million tokens by [X%].
6. Quantized [model] to [INT8 / FP8 / 4-bit], keeping quality within [N] points on the eval while doubling throughput.
7. Built a model router that picks a model per request by task and difficulty, cutting average cost per request by [X%].
8. Added semantic caching for repeated questions, serving [X%] of traffic from cache at [N]ms.
9. Reduced average prompt length from [A] to [B] tokens by trimming instructions and retrieval context, saving [$N] a month.
10. Built per-feature cost tracking and budgets, letting [N] teams see spend per request; two teams cut their costs by [X%] within a month.
11. Moved [batch workload] to a batch API, cutting its cost by [X%] with results still delivered within [N] hours.
12. Distilled a large model into a [size] model for [task], matching quality on [N] eval cases at [1/N] the cost.
13. Set up fallback across [N] model providers, keeping [feature] at [X%] availability through [N] provider outages.
14. Implemented speculative decoding for [model], cutting generation latency by [X%] at the same output quality.
15. Tuned KV cache and context settings for [model], supporting [N]K-token contexts at [N] concurrent requests per GPU.
16. Built autoscaling for the inference cluster on queue depth, cutting idle GPU hours by [X%] while keeping p95 under [N]s.
17. Load-tested the serving stack to [N] requests a second and fixed [N] bottlenecks before launch.
18. Negotiated and measured a move to [provider / committed-use pricing], saving [$N] a year with no code changes to callers.
19. Profiled the agent's token use per step and removed [N] redundant calls, cutting cost per task by [X%].
20. Wrote the cost and latency budget for every AI feature at launch, reviewed with finance each quarter.

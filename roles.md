# AI engineer vs ML engineer vs LLM engineer: what each resume must prove

The three titles overlap, and companies use them loosely. One company's "ML engineer" builds LLM agents all day. Another's "forward deployed engineer" spends the week tuning post-training runs. So don't write your resume for the title. Write it for the work the posting describes.

This page splits the work into five kinds of role. For each one: what the job is, what your resume has to prove, the evidence that counts, the bullets to lead with, the example resume closest to it, and real postings that show it.

*Last checked: 17 Nov 2026. Job postings close and change. Each one below says when it was published and what it asked for on the day we checked. If a link is dead, the company's careers page will have a similar role.*

## Contents

- [The short version](#the-short-version)
- [AI engineer](#ai-engineer)
- [ML engineer](#ml-engineer)
- [LLM engineer](#llm-engineer)
- [Research engineer](#research-engineer)
- [Forward-deployed engineer](#forward-deployed-engineer)
- [When the title and the work disagree](#when-the-title-and-the-work-disagree)
- [One inventory, five opening arguments](#one-inventory-five-opening-arguments)

## The short version

| Role | The job | What the top third of your resume must prove | Closest example |
|---|---|---|---|
| AI engineer | Build products on top of models: retrieval, agents, evals, latency, cost | You shipped an AI feature real users depend on, you measured its quality, and you are a strong software engineer | [03](examples/03-mid-level-ai-engineer.md), [04](examples/04-senior-ai-engineer.md) |
| ML engineer | Train, evaluate, serve and monitor models: data, features, offline metrics, A/B tests | You moved a model metric that mattered, with a sound eval, and ran the model in production | [06](examples/06-ml-engineer-to-llm.md) |
| LLM engineer | Adapt and run the models themselves: fine-tuning, post-training, distillation, serving | You built the dataset, picked the method, beat a baseline on held-out data, and know what it cost | [06](examples/06-ml-engineer-to-llm.md) |
| Research engineer | Build the experiments, environments and training code that research runs on | You design experiments, write reliable research infrastructure and can explain a result | [10](examples/10-research-engineer.md) |
| Forward-deployed engineer | Build production AI inside a customer's systems | You write production code and customers trust you: deployments, renewals, field feedback that became product | [07](examples/07-forward-deployed-engineer.md) |

## AI engineer

**The job.** Build product features on top of models someone else trained. The hard parts are retrieval quality, agent reliability, evals, latency and cost. Most of the code is ordinary backend code, and a lot of it is error handling.

**What the resume must prove.** Three things, in this order:

1. You shipped an AI feature that real people use, and you can say how many.
2. You know whether it works, because you measured it.
3. You are a strong software engineer, not only someone who writes prompts.

**Evidence that counts.**

- A production feature with a user count, ticket volume or request rate.
- An eval set with a size, a metric and a before/after number.
- Latency and cost numbers with the change that moved them.
- Harness work: tool design, step limits, retries, guardrails, tracing.

**Bullets to lead with.**

- [Agents and tool use](bullets/agents-and-tool-use.md): #1 (agent completes cases end to end), #4 (step caps and hand-off), #16 (tracing every run).
- [Evals](bullets/evals.md): #1 (eval harness that gates changes), #4 (evals in CI).
- [Inference and cost](bullets/inference-and-cost.md): #2 (p95 latency), #1 (routing to cut spend).
- [Product impact](bullets/product-impact.md): #1 (weekly usage).

**Example resume.** [03, mid-level AI engineer](examples/03-mid-level-ai-engineer.md) for 3 to 5 years. [04, senior AI engineer](examples/04-senior-ai-engineer.md) for 6 to 9. [02](examples/02-junior-ai-engineer.md) and [01](examples/01-new-grad-career-switcher.md) if you are earlier.

**Postings that show it.**

- [Baseten, AI Engineer](https://jobs.ashbyhq.com/baseten/b13ec426-d09d-4122-8112-cf25adbd7d60) (San Francisco, published 20 Aug 2026). Asks for 5+ years shipping software and for AI or agent products "that real users depend on". It also wants "the ability to clear a real technical bar, not just prompt well". Evals and agent observability are listed as nice to have. We use this posting for the worked example in [tailoring.md](tailoring.md).
- [Elicit, AI Engineer](https://elicit.com/careers/d27d51d7-b318-4cb0-9b88-c37de18905f3) (Oakland or remote in US time zones, listed on [Elicit's careers page](https://elicit.com/careers) on 17 Nov 2026; the page shows no publish date). It pitches the role to backend engineers who like concurrency, fault tolerance and distributed systems. The work sits between the product's endpoints and the models. Same title as Baseten, different proof: here a streaming or fault-handling bullet beats an internal-tooling one.

## ML engineer

**The job.** Train models, evaluate them, serve them and keep them healthy. Ranking, recommendations, classification, forecasting and speech all live here. More and more ML engineer roles now include LLM work too.

**What the resume must prove.**

1. You moved a model metric, and the eval behind it was sound (held-out data, a baseline, an online test where possible).
2. You own the loop around the model: data, features, deployment, monitoring.
3. You make trade-offs between quality, latency and cost in production.

**Evidence that counts.**

- Offline metric plus online result: "NDCG@10 up 4%, then +2.1% click-through in a 2-week A/B test."
- Serving numbers: latency at a stated request rate.
- Data and pipeline work that made training reproducible.
- Monitoring that caught drift or a regression.

**Bullets to lead with.**

- [RAG and search](bullets/rag-and-search.md): #9 (hybrid retrieval in an A/B test), #15 (fine-tuned embeddings, NDCG).
- [Fine-tuning](bullets/fine-tuning.md): #4 (classifier with held-out F1 and latency), #17 (retraining loop under drift).
- [Evals](bullets/evals.md): #17 (A/B test that offline evals predicted).
- [Data pipelines](bullets/data-pipelines.md): #8 (data quality checks).

**Example resume.** [06, ML engineer moving to LLM work](examples/06-ml-engineer-to-llm.md). It shows how to frame ranking and forecasting work as the hard part of LLM work.

**Postings that show it.**

- [Perplexity, Machine Learning Engineer, Ranking Quality (Search)](https://jobs.ashbyhq.com/Perplexity/19d8bcfd-e493-4b3a-b8fd-11a2a6502da2) (Belgrade, published 12 Aug 2026). Classic ML engineering. It covers training and evaluating retrieval and ranking models, plus low-latency inference and multi-stage cascades. It asks for proven ownership of a large production ranking system. Lead with your ranking metric and your serving numbers.
- [Cresta, Senior Machine Learning Engineer](https://job-boards.greenhouse.io/cresta/jobs/4741283008) (US remote, first published 29 May 2025, updated 19 Oct 2026). The title says ML; the work is mostly LLM agents, RAG and evals for non-deterministic systems. It names hallucinations, tool misuse and context drift as failure modes to fix. One track also asks for strong pre-LLM ML foundations. A resume for this role needs both: an LLM system with quality metrics, and proof of ML depth from before LLMs.

## LLM engineer

**The job.** Used loosely. Some companies mean "AI engineer". When it means something different, it means working on the model itself: building training data, fine-tuning or post-training, distilling, evaluating checkpoints and serving the result.

**What the resume must prove.**

1. You built the dataset and know where it came from.
2. You chose the method for a reason (prompting vs retrieval vs fine-tuning) and compared against a baseline.
3. The gain held on data the model never saw, and you know what it cost to train and serve.

**Evidence that counts.**

- Dataset size and source, with how you cleaned it.
- Method named precisely: LoRA, DPO, SFT, distillation. Only the one you used.
- Baseline, held-out eval and the gap between them.
- Training cost or GPU hours, and serving cost per request.
- Checks for regressions on general ability and safety.

**Bullets to lead with.**

- [Fine-tuning](bullets/fine-tuning.md): #1 (LoRA matching a frontier model at lower cost), #3 (fine-tuning vs prompting vs retrieval), #9 (eval on every checkpoint), #10 (removing eval leakage).
- [Inference and cost](bullets/inference-and-cost.md): #4 (self-hosting with vLLM or similar), #6 (quantization within N points on the eval).
- [Data pipelines](bullets/data-pipelines.md): #13 (feedback to labeled examples).

**Example resume.** [06, ML engineer moving to LLM work](examples/06-ml-engineer-to-llm.md) is the closest. If your LLM work is mostly building products, use [03](examples/03-mid-level-ai-engineer.md) or [04](examples/04-senior-ai-engineer.md) instead.

**Postings that show it.**

- [Together AI, Forward Deployed Engineer, Post-Training](https://job-boards.greenhouse.io/togetherai/jobs/5274195007) (San Francisco, published 23 Oct 2026). FDE in the title, LLM engineering in the body. It wants recent hands-on post-training of LLMs: SFT, LoRA, DPO and RL methods such as GRPO and PPO. It also asks for ablations and evals that separate real gains from noise, and for building training datasets. A resume for this needs a training bullet with a baseline and a held-out number in the top third.
- [Databricks, Staff Machine Learning Engineer, CustomerLake (ML/LLM)](https://job-boards.greenhouse.io/databricks/jobs/8923831002) (New York, published 29 Oct 2026). A mixed role. It asks you to evaluate ML and LLM approaches for personalization, inspect individual traces in production, and know RAG, prompt design and fine-tuning. It also wants evals tied to purchases and retention, not opens and clicks. Lead with a model you improved against a business metric.

For more open roles of this kind, landed keeps a list at [llm-engineer-jobs](https://github.com/landedjobs/llm-engineer-jobs).

## Research engineer

**The job.** Build what research runs on: training code, RL environments, verifiers, eval harnesses, and the pipelines that make experiments fast and repeatable. You also help design experiments and read the results.

**What the resume must prove.** That you are a strong engineer who works well with research. You can design an experiment, build reliable infrastructure for it, and explain why a result happened.

**Evidence that counts.** An experiment you designed (hypothesis, baseline, ablation, result, what you decided). A harness, sandbox or verifier you built and who used it. A training or eval pipeline you made faster or more reliable, with numbers. Papers only with the code or artifact linked.

**Bullets to lead with.** [Evals](bullets/evals.md) #10 (pass@k vs pass^k changed a launch decision) and #19 (task-specific metrics). [Agents and tool use](bullets/agents-and-tool-use.md) #11 (sandboxed code execution). [Fine-tuning](bullets/fine-tuning.md) #8 (multi-GPU training time) and #13 (documented sweeps).

**Example resume.** [10, research engineer](examples/10-research-engineer.md). Link a public eval report; the [eval report template](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/templates/eval-report.md) shows the shape.

**Posting that shows it.** [Anthropic, Research Engineer, Code RL](https://job-boards.greenhouse.io/anthropic/jobs/5254364008) (San Francisco or New York, first published 11 Jun 2026, updated 21 Aug 2026). You design RL environments and coding tasks, build reward signals and verifiers, run training experiments and speed up the pipelines. It asks for deep Python including async and concurrent code, end-to-end ownership of systems, and rigor in experimental design. RL or fine-tuning experience is listed as a plus, not a must. So is having built coding agents, sandboxes, eval harnesses or verifiers.

## Forward-deployed engineer

**The job.** Build production AI systems inside a customer's environment, then turn what you learn into product. Half engineer, half the person the customer calls.

**What the resume must prove.** You ship production code yourself, and customers trust you with it. Most FDE resumes lean too far one way. Pair every technical bullet with a customer outcome.

**Evidence that counts.** Deployments with time to production. Renewals and expansions. Connectors and evals you wrote per customer. Field requests that became product features. Travel willingness in the header if the role needs it.

**Bullets to lead with.** [Product impact](bullets/product-impact.md) #18 (demos and evals that closed deals) and #10 (manual review cut for a customer). [Agents and tool use](bullets/agents-and-tool-use.md) #6 (MCP server with auth and audit logs). [Data pipelines](bullets/data-pipelines.md) #3 (connectors with permission mirroring).

**Example resume.** [07, forward-deployed engineer](examples/07-forward-deployed-engineer.md).

**Postings that show it.** FDE roles split into an application layer and an infrastructure layer:

- [Anthropic, Forward Deployed Engineer](https://job-boards.greenhouse.io/anthropic/jobs/5423029008) (London, published 14 Sep 2026). Application layer. You build production apps with Claude inside customer systems and deliver MCP servers, sub-agents and agent skills. You also codify repeatable deployment patterns. It asks for 4+ years in a technical customer-facing role, production LLM experience and 25 to 50% travel.
- [Cohere, Forward Deployed Engineer, Inference](https://jobs.ashbyhq.com/cohere/8df498e9-aba8-487f-80ba-362b492bad09) (United States, published 28 Oct 2026). Infrastructure layer. Model serving topologies, multi-tenant setups, cross-datacenter failover and benchmarking customer LLM workloads. It wants 8+ years and deep production Kubernetes. Lead with serving and reliability numbers, not agent demos.

More open roles: [forward-deployed-engineer-jobs](https://github.com/landedjobs/forward-deployed-engineer-jobs).

## When the title and the work disagree

Three of the postings above have a title that undersells or misnames the work: Cresta's ML engineer builds LLM agents, Together's FDE runs post-training, and Databricks's ML engineer works on LLM systems. Cohere also hires a [Senior/Staff Back-End Software Engineer, Inference](https://jobs.ashbyhq.com/cohere/14aef6d9-763e-4f56-a498-206fb31dd0c6) (Canada, published 15 Oct 2026) whose work is identity, billing, metering and tenant isolation for the inference platform. That is backend engineering at a model company. A strong distributed-systems bullet should lead there, not a RAG bullet.

Our advice: read the responsibilities and the "you may be a good fit" list, then ask what this person will build, run or measure in their first six months. Pick your opening bullets for that answer. Keep your real job titles on your resume whatever the posting calls the role.

## One inventory, five opening arguments

Keep one master list of everything you have done, with the real numbers. For each application, pick the three bullets from it that answer the posting's main question, and put them at the top of your most recent role. The facts stay the same in every version. Only the order and the emphasis change.

[tailoring.md](tailoring.md) walks through that step by step with a worked example. For live roles to try it on, see [ai-engineer-jobs](https://github.com/landedjobs/ai-engineer-jobs). For the interviews that follow, see [awesome-ai-engineer-interview](https://github.com/landedjobs/awesome-ai-engineer-interview).

---

<sub>No affiliation with the companies named. Postings are quoted briefly and summarized as they read on the dates given. All example people in this repo are fictional.</sub>

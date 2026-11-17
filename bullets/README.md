# Bullet banks

191 resume bullets for AI engineering roles in 8 banks, 22 to 25 each. Each bank ends with a "More bullets (Nov 2026)" section whose bullets also name the test set, baseline, load or date behind the number. Every bullet follows the formula from the [main README](../README.md#the-bullet-formula): action, what you built, scale or number, outcome.

| Bank | Use it for | File |
|---|---|---|
| RAG and search | Retrieval, search relevance, knowledge assistants | [rag-and-search.md](rag-and-search.md) |
| Agents and tool use | Agents, tool calling, workflows, MCP, voice and browser agents | [agents-and-tool-use.md](agents-and-tool-use.md) |
| Evals | Golden sets, LLM-as-judge, online evals, red-teaming | [evals.md](evals.md) |
| Inference and cost | Latency, serving, routing, caching, GPU work | [inference-and-cost.md](inference-and-cost.md) |
| Fine-tuning | LoRA, DPO, distillation, embedding and reward models | [fine-tuning.md](fine-tuning.md) |
| Data pipelines | Ingestion, parsing, labeling, PII, connectors | [data-pipelines.md](data-pipelines.md) |
| Product impact | Adoption, revenue, time saved, A/B tests | [product-impact.md](product-impact.md) |
| Leadership | Architecture, standards, hiring, mentoring, incidents | [leadership.md](leadership.md) |

## How to use them

1. Pick 3 to 5 bullets per role that match work you actually did.
2. Replace every placeholder with your real number. If you don't have the number, find it (dashboards, old Slack threads, your manager) or describe the scope instead.
3. Rewrite the nouns into your system's words. A bullet copied word for word reads like a template.
4. Read each one aloud and ask: could I talk about this for five minutes in an interview? If not, cut it.

Don't invent numbers. Interviewers ask "how did you measure that?" and the answer has to be real.

## Evaluation vocabulary to get right

Last checked: 17 Nov 2026

Interviewers test the words in your bullets. A smaller number with a clear metric, test set and baseline holds up better than a big number whose meaning shifts when someone asks a follow-up. Our checklist:

| Term | What it means | Common slip |
|---|---|---|
| Accuracy vs precision and recall | Accuracy is the share of all predictions that were right. Precision is the share of flagged items that were right; recall is the share of true items you found. | Writing "95% accuracy" for a PII filter or a detector, where recall on the rare class is the number that matters. |
| recall@k, NDCG@k | Retrieval metrics: did the right document appear in the top k, and how high was it ranked. | Calling a retrieval gain an "accuracy" gain without saying whether retrieval or generation improved. |
| Held-out set | Examples the system never saw while you built, tuned or trained it. | Reporting a score on the same examples you used to tune prompts or pick checkpoints. |
| Baseline | The thing you compared against: the old system, the prompted base model, a single agent. | Comparing against different baselines in different bullets, or not naming one. |
| pass@k vs pass^k | pass@k: at least one of k tries succeeds. pass^k: all k tries succeed. Anthropic's [agent evals guide](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents) shows a 75% per-try success rate gives about 42% for passing all three tries. | Quoting pass@k for a customer-facing agent where users need it to work every time. |
| p50 vs p95 | p50 is the median request; p95 is the slowest 5% boundary. Cresta's [voice latency post](https://cresta.com/blog/engineering-for-real-time-voice-agent-latency) notes its figures are roughly medians and that a good median is not enough. | Presenting a median gain as a tail-latency gain, or model latency as end-to-end latency. |
| Offline vs pilot vs production | Where the number was measured. | Turning an offline benchmark into a production claim. |

Two more checks from vendor guidance. OpenAI's [evaluation best practices](https://platform.openai.com/docs/guides/evaluation-best-practices) advise test data with typical, edge and adversarial cases, and calibrating automated scoring with human feedback. Microsoft's [Foundry observability docs](https://learn.microsoft.com/en-us/azure/foundry/concepts/observability) list agent measures such as tool call accuracy and task completion apart from quality and safety. So "eval score improved" is weak; name what the evaluator measures.

### Case study: why a bare "90.2%" is not a complete bullet

Anthropic [reported](https://www.anthropic.com/engineering/built-multi-agent-research-system) that a multi-agent system (Claude Opus 4 as lead, Claude Sonnet 4 subagents) "outperformed single-agent Claude Opus 4 by 90.2%" on its internal research eval. Read it carefully:

- **It is a relative gain on one internal eval**, not 90.2 points of accuracy and not a result for every agent task.
- **The baseline is a single agent.** The same post says agents use about 4x the tokens of chat and multi-agent systems about 15x. That cost comparison is against chat, not against the single-agent baseline.
- **Fit matters.** The post says multi-agent systems pay off only when the task is valuable enough, and that tasks with heavy shared context or tight dependencies suit them less.

If your own bullet carries a number like this, keep quality, baseline and cost apart and name each one. For example: "Raised [metric] [X%] over a single-agent baseline on [N] internal research tasks, at [N]x the tokens per task." The rest of the protocol can live in a linked eval report (see the [eval report template](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/templates/eval-report.md)).

## Real bullets from public resumes

Last checked: 17 Nov 2026

The example bullets in the banks are placeholders. These are real bullets, paraphrased with short excerpts, from resumes their owners publish on their own sites. They show how specific numbers read. They are not achievements to copy.

| Person | What the bullet says | What makes it work |
|---|---|---|
| [Animikh Aich](https://animikh.me/assets/pdfs/Animikh-Aich-Resume.pdf) | Cut annual infrastructure costs by over $1M (about 95%) by designing a 6x faster ML pipeline that replaced Databricks and moved models to independently scalable NVIDIA Triton servers. | The cost number comes with the mechanism, so an interviewer can ask about the architecture. |
| [Animikh Aich](https://animikh.me/assets/pdfs/Animikh-Aich-Resume.pdf) | Led "a cross-functional team of 14 engineers" deploying 90+ real-time video analytics use cases across 20K+ CCTV cameras. | Team size, number of use cases and fleet size give scope without a vague "led a team". |
| [Saurabh Singh](https://saurabhportfolio.com/resources/resume.pdf) | Built an LLM contract-discovery tool over 300k PDFs (156GB), cutting document processing time by 90%. | Corpus size and format make the data work concrete. |
| [Saurabh Singh](https://saurabhportfolio.com/resources/resume.pdf) | Led an AI assistant that reaches 100+ Snowflake databases through MCP servers using generated SQL. | Specific scale. A linked report would still need to cover permissions and how correctness was checked. |
| [Mikhail Jacob](https://www.mikhailjacob.in/assets/docs/cv/Mikhail%20Jacob%20-%20Senior%20Applied%20Scientist%20-%20September%202025.pdf) | Shipped bots in two VR games, trained with deep RL and imitation learning (RLlib and Unity) and run on device. | Shows shipped ML without forcing a revenue number. |

What most of these leave out is the test set and baseline behind the number. The "More bullets (Nov 2026)" sections in each bank show where those go.

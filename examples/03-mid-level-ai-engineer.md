# Example 03: Mid-level AI engineer (3 to 5 years, RAG and agents in production)

> **Fictional person.** Aisha Kapoor, her employers and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** mid. **Target roles:** AI engineer, senior AI engineer (stretch), LLM engineer, agent engineer. **Background:** 4 years, the last 2 building RAG and agents for a customer support product.

This is the most competitive band. Many candidates have "built RAG." The resume has to show scale, measurement and the problems that only appear in production.

---

## The resume

**Aisha Kapoor**
Seattle, WA (open to remote) · aisha.kapoor@example.com · (555) 010-7832
github.com/akapoor-example · Write-up: "What broke when our support agent hit 50K tickets a week" (aishakapoor.example.com)

**Experience**

**AI Engineer**, Cobalt Support (fictional) · Seattle, WA · *Mar 2024 to present*
*Series C, 300 people, customer support platform used by 1,200 companies*
- Built and run the retrieval layer behind the support answer agent: hybrid search and reranking over 2.1M help-center articles from 1,200 customer workspaces, with per-tenant isolation; answer accuracy on a 600-question golden set went from 71% to 88%.
- Rebuilt the agent from a single prompt into a planner with 7 tools (search, order lookup, refund, escalate and others); it now resolves 43% of 50K weekly tickets with no human touch, up from 19%.
- Designed the agent eval suite: 900 replayed real conversations scored for outcome and for tool-call correctness, plus an LLM judge calibrated to 91% agreement with support leads; every release must pass it.
- Cut cost per resolved ticket from $0.31 to $0.11 with prompt caching, a smaller model for classification and summarization, and capping agent steps at 8 with a graceful hand-off.
- Found and fixed a prompt-injection path through customer-uploaded articles; added content sanitization and a tool-permission check, and wrote the red-team set (400 cases) now run weekly.
- Brought p95 time-to-first-token from 3.2s to 0.9s with streaming and parallel retrieval.

**Software Engineer**, Cobalt Support (fictional) · Seattle, WA · *Jul 2022 to Mar 2024*
- Built the ticket ingestion pipeline (Kafka, Python) that processes 2M events a day; moved embedding generation into it, cutting article-to-searchable time from 6 hours to 4 minutes.
- Shipped the first LLM feature at the company, a reply-suggestion box; 62% of agents used it daily within 2 months of launch.

**Software Engineer**, Halden Bank (fictional) · Charlotte, NC · *Aug 2021 to Jun 2022*
- Built internal APIs for the loan servicing team in Java and Spring; cut a nightly batch job from 5 hours to 50 minutes.

**Skills**

Languages: Python, TypeScript, Java, SQL
Retrieval and agents: hybrid search, cross-encoder reranking, query rewriting, tool calling, planner-executor agents, MCP
Evals and ops: golden sets, replay evals, LLM-as-judge calibration, tracing, red-teaming, prompt caching, model routing
Infra: AWS, Kafka, Postgres + pgvector, OpenSearch, Redis, Kubernetes, Terraform

**Education**

**BS, Computer Science**, Lakeshore State University (fictional) · *2021*

---

## Why this works

- **Every agent claim is measured.** Resolution rate (19% to 43%), accuracy on a named golden set, cost per resolved ticket. A reader can tell this agent is real.
- **The eval suite is specific.** Replayed conversations, tool-call correctness, and a judge calibrated against human labels. That one bullet answers the question most mid-level resumes skip.
- **Security shows up.** The prompt-injection bullet is rare on resumes and shows she has run an agent where customers control part of the input.
- **The promotion is visible.** Two roles at the same company show growth from pipeline work to owning the AI system.
- **The old job is one bullet.** Banking backend work from 2021 earns one line, which is right.
- **The write-up link** gives the interviewer something to read before the call, and its title promises production lessons.

## What to change for each kind of employer

**Frontier lab (applied AI, product engineering).** Labs build agents and evals too, and they will dig into mechanism. Lead with the eval suite and the judge calibration. Add one line about what you learned about model behavior (for example, where the planner failed on long tool chains and how you measured it). Cut the bank role to make room.

**Startup.** Lead with resolution rate and cost per ticket: those are the numbers founders care about. Mention team size if you shipped this with very few people ("one of 3 engineers on the agent"). Keep the write-up link high.

**Enterprise.** Lead with per-tenant isolation, the prompt-injection fix and the red-team set. Keep the bank role, since regulated-industry experience counts here. Add any compliance work you did (SOC 2 evidence, data retention rules). Use the posting's terms, such as "knowledge assistant" or "AI copilot", where they describe your system.

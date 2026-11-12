# Example 02: Junior AI engineer (1 to 2 years)

> **Fictional person.** Daniel Reyes, his employers, projects and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** junior. **Target roles:** AI engineer, LLM engineer, applied AI engineer. **Background:** 18 months as a software engineer on a team that ships LLM features, one open-source contribution, one side project.

At this level you have one real job to show. The goal is to prove you owned pieces of a production LLM system, not that you were near one.

---

## The resume

**Daniel Reyes**
Chicago, IL · daniel.reyes@example.com · (555) 010-2290
github.com/dreyes-example · danielreyes.example.com

**Experience**

**Software Engineer, AI Features**, Kestrel Docs (fictional) · Chicago, IL · *Jun 2024 to present*
*Series B, 80 people, contract review software for mid-size law firms*
- Owned the clause-extraction service that pulls 23 clause types from uploaded contracts; raised field-level F1 on a 1,100-contract labeled set from 0.81 to 0.92 by moving to schema-constrained JSON output and a second-pass validator.
- Built the eval pipeline that runs the labeled set on every pull request touching prompts or models, with a per-clause diff report; the team has shipped 40 prompt changes through it with no extraction regressions reaching customers.
- Cut p95 latency for a 30-page contract from 19s to 7s by splitting documents into sections and extracting in parallel, then merging with a dedup step.
- Reduced model spend per contract by 46% by sending short, low-risk clause types to a smaller model, with routing rules checked against the eval set.
- Handled on-call for the extraction service (1 week in 5); wrote 6 runbooks and added alerts on schema-validation failure rate.

**Software Engineer Intern**, Patchwork Retail (fictional) · Remote · *Jun to Aug 2023*
- Built a product-description generator for 18K catalog items with human review in the loop; editors accepted 74% of drafts without changes.

**Open source**

**Contributor**, an open-source LLM evaluation library (2 merged PRs)
- Added a JSON-schema match metric with partial credit for nested fields, used by the library's structured-output examples.
- Fixed a race in the async batch runner that dropped results under high concurrency.

**Projects**

**Lease Q&A**, RAG over residential lease law for tenants · Python, LlamaIndex, Qdrant, Next.js · *2025*
- Indexed 3,200 pages of state housing statutes and court help pages; 1,100 monthly visitors with a 4.5/5 average answer rating from 300 ratings.
- Published an eval report with a 150-question golden set written with a tenant-rights volunteer; answer accuracy 87%, with every answer citing a statute section.

**Education**

**BS, Computer Engineering**, Riverside Institute of Technology (fictional) · *2024*

**Skills**

Languages: Python, TypeScript, SQL
LLM: structured output, function calling, RAG, prompt and model routing, eval pipelines
Infra and tools: AWS (ECS, SQS, S3), Postgres, Redis, Docker, Datadog, GitHub Actions

---

## Why this works

- **Ownership is clear.** "Owned the clause-extraction service" and "handled on-call" tell the reader he is trusted with a production system after 18 months.
- **The best bullet comes first.** F1 from 0.81 to 0.92 on a named test set is specific, measurable and invites a good interview question.
- **The eval pipeline is its own bullet.** "40 prompt changes with no regressions reaching customers" shows he built a process as well as features.
- **Latency and cost both appear**, each with a mechanism (parallel section extraction, small-model routing).
- **The company context line** helps a reader who has never heard of Kestrel Docs. One line of italics is enough.
- **The open-source section is short and real.** Two merged PRs with what they did beats a vague "contributed to open source."
- **The side project has a domain partner** (a tenant-rights volunteer wrote golden questions). That detail makes the eval believable.

## What to change for each kind of employer

**Frontier lab.** Labs ask juniors about fundamentals. Add a line on what you know about the model side: a small fine-tuning comparison you ran, or a tokenizer or sampling experiment. Move the open-source section above projects, since lab engineers read code. Keep the eval pipeline bullet near the top.

**Startup.** Add speed and breadth. If you shipped a feature end to end (backend, prompt, UI), say so. Put the side project's traffic numbers in the first line. Startups also like on-call experience; keep it.

**Enterprise.** Emphasize reliability, compliance and process. Keep the runbooks and alerts bullet. If the extraction service handles confidential documents, add how data was handled ("tenant-isolated storage, no customer data in prompts logged to third parties"). Mirror the posting's terms (for example "document intelligence", "IDP", "NLP") where they fit.

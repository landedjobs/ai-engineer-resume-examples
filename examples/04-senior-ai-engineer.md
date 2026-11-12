# Example 04: Senior AI engineer

> **Fictional person.** Tomás Lindqvist, his employers and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** senior, 7 years. **Target roles:** senior AI engineer, senior LLM engineer, tech lead for an AI product team. **Background:** backend and search engineer who moved into LLM systems in 2023 and now leads the technical side of an AI product area.

At senior level the reader wants three things beyond strong bullets: decisions you made that others followed, systems at real scale, and evidence you raise the people around you.

---

## The resume

**Tomás Lindqvist**
New York, NY · tomas.lindqvist@example.com · (555) 010-5517
github.com/tlindqvist-example · Talk: "Evals as a release gate" (internal AI summit, recording on request)

**Summary**
Senior engineer, 7 years in search and backend systems, 3 in LLM products. Tech lead for document AI at a 900-person insurance software company; owns the retrieval, agent and eval platform used by 6 product teams.

**Experience**

**Senior AI Engineer, Tech Lead (Document AI)**, Harborview Insurance Software (fictional) · New York, NY · *Jan 2023 to present*
- Led the design of the claims document agent, which reads adjuster files (avg. 140 pages), extracts 60 fields and drafts the coverage summary; adjusters now spend 38 minutes per claim on review instead of 2.5 hours, across 22K claims a month.
- Set the architecture the 6 AI product teams build on: a shared retrieval service, a tool registry and a release gate that runs each team's golden set and blocks deploys that regress it; adopted by all 6 teams within two quarters.
- Chose to fine-tune an open 8B model for field extraction instead of calling a frontier model on every page; it matched the frontier model on a 3,000-document eval at 1/7 the cost, saving $1.1M a year at current volume.
- Built human-review sampling: 2% of agent outputs go to adjusters with a structured rubric, feeding a weekly drift report; it caught 3 extraction regressions from upstream form changes before customers did.
- Mentored 4 engineers into owning AI services; 2 were promoted to senior within 18 months.

**Senior Software Engineer, Search**, Quarry Analytics (fictional) · Boston, MA · *Jun 2020 to Dec 2022*
- Owned relevance for search across 400M business records; introduced learning-to-rank on top of BM25, raising click-through on the first result by 14% in an A/B test.
- Led the move from a self-managed Elasticsearch cluster to a managed service, cutting search incidents from 9 a quarter to 1.

**Software Engineer**, Quarry Analytics (fictional) · Boston, MA · *Jul 2018 to Jun 2020*
- Built the data ingestion service for public company filings, processing 50K documents a day.

**Skills**

Languages: Python, Go, SQL
LLM systems: RAG, document extraction, agents with tool registries, LoRA fine-tuning, vLLM serving, structured output
Evals and quality: golden sets, release gates, human-review sampling, drift monitoring, LLM-as-judge
Infra: AWS, Kubernetes, Postgres, Elasticsearch/OpenSearch, Kafka, Airflow, Terraform

**Education**

**MS, Computer Science**, Riverside Institute of Technology (fictional) · *2018*

---

## Why this works

- **The summary earns its place.** It explains the move from search to LLM work and states scope (6 product teams) in two lines.
- **The first bullet is about users' time.** 2.5 hours to 38 minutes per claim, at 22K claims a month, tells a business story and a technical one.
- **Decisions are explicit.** "Chose to fine-tune an open 8B model instead of calling a frontier model" names a trade-off, the eval behind it and the money. That's what senior means.
- **Platform influence is measured.** "Adopted by all 6 teams within two quarters" shows leadership without a manager title.
- **Search history is an asset.** The learning-to-rank and Elasticsearch bullets prove he understood retrieval long before RAG was a term.
- **Mentoring has an outcome** (2 promotions). "Mentored engineers" alone says nothing.

## What to change for each kind of employer

**Frontier lab.** Labs will want depth on the fine-tuning decision: data size, how the eval was built, what failed. Expand that bullet into two. Add any work on serving (batching, quantization, throughput numbers). Drop the oldest role.

**Startup.** Lead with what you built hands-on, not the platform you set for 6 teams. Startups worry seniors from big companies won't write code. Add a line that shows recent hands-on shipping ("wrote the extraction service's first version in 3 weeks"). Cut the mentoring bullet to make room if needed.

**Enterprise.** This resume is close to ready. Add compliance and governance details (model risk review, audit logs for agent actions, data residency) if you did them. Keep the platform and release-gate bullets near the top. Use the posting's language for the domain (claims automation, underwriting, document intelligence).

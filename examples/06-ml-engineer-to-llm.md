# Example 06: ML engineer moving to LLM work

> **Fictional person.** Kenji Watanabe-Cole, his employers, projects and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** mid to senior, 5 years. **Target roles:** AI engineer, LLM engineer, applied scientist (LLM). **Background:** classic ML engineer (ranking, forecasting) with one LLM project at work and one outside it.

The risk with this resume is that it reads as "ML engineer who read about LLMs." The fix is to frame classic ML experience as the hard part of LLM work (data, evaluation, serving) and put the LLM evidence first.

---

## The resume

**Kenji Watanabe-Cole**
Toronto, ON (open to US relocation or remote) · kenji.wc@example.com · (555) 010-8125
github.com/kwatanabecole-example · Eval report: kenjiwc.example.com/rerank-eval

**Summary**
ML engineer, 5 years shipping ranking and forecasting models at 20M-user scale. For the last year I've built LLM retrieval and evaluation, including a fine-tuned reranker now in production. I bring offline/online evaluation discipline to LLM systems.

**Experience**

**Machine Learning Engineer II**, Fernway Marketplace (fictional) · Toronto, ON · *Jan 2022 to present*
*Online marketplace, 20M monthly users*
- Led the company's first LLM feature in production: query understanding for marketplace search, using an LLM to rewrite vague queries into structured filters; it raised search-to-purchase rate by 4.1% in a 4-week A/B test on 10% of traffic.
- Fine-tuned a cross-encoder reranker on 600K click and purchase pairs; it beat the prior learning-to-rank model by 7% NDCG@10 offline and 2.3% on revenue per search online.
- Built the offline eval for the LLM query rewriter: 5,000 queries labeled by 3 annotators, inter-annotator agreement tracked, plus an LLM judge checked against the labels; this became the template for 2 later LLM features.
- Cut the rewriter's serving cost by 70% by distilling it into a small model for the 85% of queries that matched known patterns, keeping the large model for the long tail.
- Owned the ranking model (gradient-boosted trees, then a two-tower neural model) for 3 years; retrained weekly with drift checks, 99.95% serving availability.

**Data Scientist**, Sablefish Health (fictional) · Toronto, ON · *Jul 2020 to Dec 2021*
- Built demand forecasting for 40 clinics (LightGBM), reducing staffing overage cost by 12%.

**Projects**

**Open reranker benchmark for legal search** · *2025*
- Compared 5 open rerankers and 2 hosted ones on a 2,000-query legal retrieval set I built from public court opinions; published code, data card and results. 180 GitHub stars.

**Skills**

LLM: RAG, query rewriting, reranking, fine-tuning (LoRA, full fine-tune of small models), distillation, LLM-as-judge
Classic ML: ranking, learning-to-rank, two-tower retrieval, gradient-boosted trees, forecasting, A/B testing
Languages and tools: Python, PyTorch, Hugging Face, SQL, Spark, Airflow, GCP (Vertex AI, BigQuery), Kubernetes

**Education**

**MSc, Statistics**, Riverside Institute of Technology (fictional) · *2020*

---

## Why this works

- **The LLM work leads every section.** The summary, first experience bullet and first project are LLM work, even though most of his career is classic ML.
- **Classic ML becomes the advantage.** A/B testing, NDCG, inter-annotator agreement and distillation are things many AI engineers without an ML background can't show. He frames them as how he does LLM work well.
- **Online results as well as offline.** "+4.1% search-to-purchase in an A/B test" is stronger than any offline metric, and ML engineers have that habit.
- **The project fills a gap.** He has no agent or chatbot experience, so the project shows public, reproducible retrieval evaluation instead.
- **The title stays honest.** "Machine Learning Engineer II" stays. The bullets do the repositioning.

## What to change for each kind of employer

**Frontier lab.** This profile fits applied research and post-training data roles. Expand the fine-tuning and eval bullets with data sizes, training details and failure analysis. Add PyTorch depth (custom training loops, distributed training if any). Keep the statistics degree visible.

**Startup.** Show you can build the whole product around the model. If you wrote the API or UI around the query rewriter, say so. Add any agent or tool-calling work, even small. Startups hiring AI engineers often want someone who can ship a full feature alone.

**Enterprise.** Keep A/B testing, availability and drift checks high. Enterprises value someone who already runs models with monitoring and governance. Use the posting's terms (MLOps, model monitoring, responsible AI) where true.

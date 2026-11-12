# Example 05: Staff or lead AI engineer

> **Fictional person.** Grace Achterberg, her employers and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** staff, 12 years. **Target roles:** staff AI engineer, principal engineer (AI), head of AI engineering at a growth-stage company. **Background:** distributed systems and ML platform engineer who has led LLM platform work for 3 years.

Two pages are fine here, but page two must hold real work. Staff resumes are judged on scope and judgment: which problems you picked, which you said no to, and what changed across the company because of you.

---

## The resume

**Grace Achterberg**
San Francisco, CA · grace.achterberg@example.com · (555) 010-3364
github.com/gachterberg-example · Writing: graceachterberg.example.com (6 posts on LLM platform design)

**Summary**
Staff engineer, 12 years in distributed systems and ML platforms. Lead for the LLM platform at a public fintech: serving, evals, safety and cost for 31 AI features used by 9M customers. I pick the problems that block many teams and make them boring.

**Experience**

**Staff Engineer, LLM Platform Lead**, Ledgerline (fictional) · San Francisco, CA · *Feb 2023 to present*
*Public fintech, 4,000 employees, consumer banking and small-business accounts*
- Proposed and led the LLM platform (gateway, routing, prompt registry, eval service, tracing) now behind all 31 AI features; teams go from idea to production in a median of 3 weeks, down from 4 months for the first two features.
- Set the company's model strategy: a routing layer across 2 hosted providers and 1 self-hosted model, chosen per request by task and risk tier; cut LLM spend by 58% ($6.2M a year) while every feature held its eval baseline.
- Wrote the AI release standard (golden set, red-team set, human review rate by risk tier) adopted by the risk and compliance org as policy; it passed 2 regulator exams with no findings on AI controls.
- Led the incident review and fix after a support assistant gave wrong fee information to 1,400 customers; the fix (grounding checks against the fee table and an output verifier) has held at zero repeats across 18M answers since.
- Grew the platform team from 3 to 14 engineers; hired 9 of them and set the interview loop for AI engineers company-wide.
- Said no to a company-wide fine-tuning program in 2024 after a 6-week study showed routing and retrieval fixes beat fine-tuning on 7 of 9 target tasks; the study memo is still the reference for build-vs-buy calls.

**Senior Engineer, then Staff Engineer, ML Platform**, Ledgerline (fictional) · San Francisco, CA · *Apr 2019 to Feb 2023*
- Built the feature store and online model serving used by fraud, credit and marketing models; 140 models in production, p99 serving latency 18ms.
- Led the migration of model training from ad hoc notebooks to a pipeline with lineage and reproducible builds, a prerequisite for the 2022 model risk audit.

**Senior Software Engineer**, Mosaic Freight (fictional) · Oakland, CA · *2015 to 2019*
- Designed the real-time pricing service for freight quotes (Go, Kafka), 3K requests a second at peak.
- Tech lead for a 6-person team that rebuilt shipment tracking; on-time event delivery rose from 92% to 99.7%.

**Software Engineer**, Mosaic Freight (fictional) · *2013 to 2015*

**Skills**

LLM platform: gateways, model routing, prompt and eval registries, tracing, guardrails, self-hosted serving (vLLM), caching
ML platform: feature stores, online serving, training pipelines, model risk management
Languages and infra: Python, Go, Java, Kubernetes, Kafka, Postgres, AWS, GCP, Terraform

**Education**

**BS, Electrical Engineering and Computer Science**, Lakeshore State University (fictional) · *2013*

---

## Why this works

- **Scope is in the summary and the first bullet.** 31 features, 9M customers, idea-to-production time. The reader knows what level this is in ten seconds.
- **Judgment is visible.** The bullet about saying no to fine-tuning shows the most staff-level behavior there is: a well-argued decision not to build something.
- **Incidents are owned.** The wrong-fee incident bullet admits a failure and shows the fix holding at 18M answers. Senior readers trust this more than a page of wins.
- **Influence crosses org lines.** The release standard became compliance policy and passed regulator exams.
- **Hiring is quantified.** 3 to 14 engineers, 9 hired personally, and the interview loop.
- **Older roles shrink.** 2013 to 2015 is one line with no bullets.

## What to change for each kind of employer

**Frontier lab.** Labs hire staff engineers to build infrastructure at a scale few others have. Lead with serving, routing and eval infrastructure numbers (requests per second, GPU utilization, latency). Shrink the compliance material. Add any work close to the model (custom serving optimizations, eval methodology you published).

**Startup (head of AI engineering).** Lead with the 3-week idea-to-production number and the team you built. Add a line on how fast you can personally ship. Founders want a builder who can also hire. Cut the ML platform section to 1 bullet.

**Enterprise.** Keep the release standard, the regulator exams and the incident review high. These are exactly what enterprise AI leaders are hired to own. Add vendor management if you did it (contract and security review of model providers).

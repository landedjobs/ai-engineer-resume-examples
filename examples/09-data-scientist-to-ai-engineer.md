# Example 09: Data scientist moving into AI engineering

> **Fictional person.** Daniela Ortiz-Reyes, her employers, projects and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** mid, 4 years. **Target roles:** AI engineer, applied AI engineer, LLM engineer. **Background:** data scientist at an insurer (pricing models, claims analytics) who owned the deployment of two models and built one LLM system at work.

The risk with this resume is that it reads as "analyst who ran notebooks." The fix is to show the bridge from analysis to software: who packaged the model, who served it, who got paged when it broke. Every bullet says which of those she owned.

---

## The resume

**Daniela Ortiz-Reyes**
Chicago, IL (open to remote) · daniela.or@example.com · (555) 010-4417
github.com/dortizreyes-example · Eval report: danielaor.example.com/claims-extraction-eval

**Summary**
Data scientist, 4 years in insurance pricing and claims. For the last 18 months I've built and run production ML and LLM services myself: APIs, batch pipelines, tests and monitoring, not only the models. Looking for AI engineering roles where evaluation and data quality decide whether the system works.

**Experience**

**Senior Data Scientist**, Larchmont Mutual (fictional) · Chicago, IL · *Feb 2024 to present*
*Regional insurer, 1.4M policies, 30-person data team*
- Built and deployed the claims document extraction service: an LLM pulls 22 fields from adjuster notes and repair estimates into a typed schema; it handles 9K claims a day, and adjusters accept 94% of fields without edits.
- Wrote the extraction eval myself: 1,200 claims hand-labeled by 4 adjusters, per-field precision and recall, and a weekly sample of 100 live claims re-labeled to catch drift; the release gate fails any field below 0.90 F1.
- Owned the service end to end: FastAPI on Kubernetes, Pydantic schema validation, retries and a fallback queue for human review; 99.9% of claims processed within 5 minutes over 6 months.
- Moved the fraud-score model from a monthly notebook run to a daily batch job (Airflow, dbt, Docker) with data contracts on 14 input tables; failed loads dropped from about 3 a month to 0 in the last 2 quarters.
- Cut the extraction cost per claim from $0.042 to $0.011 by routing short, standard documents to a smaller model, keeping the large model for the 18% that failed schema checks.

**Data Scientist**, Larchmont Mutual (fictional) · Chicago, IL · *Jun 2022 to Feb 2024*
- Built the auto-renewal pricing model (gradient-boosted trees) used for 380K policies a year; analyzed its A/B rollout and reported a 1.6-point loss-ratio improvement. The pricing engineering team implemented the deployment.
- Wrote the team's shared Python package for feature definitions, with unit tests and CI; 6 data scientists now import it instead of copying SQL.

**Projects**

**Open claims-extraction benchmark** · *2025*
- Built a 500-document synthetic benchmark of insurance forms with field-level labels; compared 4 open and 2 hosted models on accuracy, latency and cost per document. Code, data card and eval report public. 140 GitHub stars.

**Skills**

AI engineering: structured extraction, schema validation, model routing, RAG, LLM-as-judge with human calibration, prompt and eval versioning
Data and ML: Python, SQL, pandas, scikit-learn, LightGBM, A/B testing, causal inference, data contracts
Engineering: FastAPI, Docker, Kubernetes, Airflow, dbt, Snowflake, GitHub Actions, pytest, Grafana

**Education**

**MS, Applied Statistics**, Northgate University (fictional) · *2022*
**BS, Economics**, Northgate University (fictional) · *2020*

---

## Why this works

- **Ownership is explicit.** "Owned the service end to end" and "The pricing engineering team implemented the deployment" sit on the same page. The honest line about the older model makes the stronger claims believable.
- **The bridge is in the bullets.** Each modeling result comes with the engineering around it: the API, the schema checks, the batch job, the data contracts, the on-call numbers. That is the gap a hiring manager worries about with a data scientist, and she closes it with evidence.
- **Her data habits become the advantage.** Hand-labeled eval sets, per-field metrics, drift checks and a release gate are things many AI engineers can't show. She frames them as how she builds AI systems.
- **The summary earns its place.** It names the move she is making in one line, then says what she brings. For a career change, that saves the reader a guess.
- **The title stays honest.** "Senior Data Scientist" stays. The bullets do the repositioning, and the project fills the gap of public, inspectable work.

## What to change for each kind of employer

**Frontier lab.** Labs hiring for applied AI or evals will care most about the eval design. Expand it: how the labels were collected, adjuster agreement, how the judge was checked against humans, and one failure you found. Keep the statistics degree visible. Cut the shared-package bullet if space is short.

**Startup.** Lead with the extraction service and the cost bullet. Show you can ship a feature alone: if you built the review UI or the API contract with another team, say so. Move the benchmark project up; startups often read the GitHub link first.

**Enterprise.** Keep the data contracts, the release gate and the human review fallback high. Regulated-industry experience counts here, so name what you handled (PII redaction, audit logs, model risk review) where true. Use the posting's terms, such as "document AI" or "intelligent document processing".

*Last checked: 17 Nov 2026*

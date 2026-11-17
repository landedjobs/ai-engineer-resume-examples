# Bullet bank: data pipelines

25 bullets for ingestion, parsing, labeling and data infrastructure behind AI systems. Replace every `[placeholder]` with your own numbers and nouns.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values.

1. Built the ingestion pipeline that parses, chunks and embeds [N]K documents a day with retries and dedup, cutting index staleness from [A] to [B].
2. Wrote parsers for [PDFs / scanned forms / HTML / slides] with table and layout extraction, raising usable text from [A]% to [B]% of pages.
3. Built connectors for [N] sources ([SharePoint, Google Drive, Confluence, Salesforce]) with incremental sync and permission mirroring.
4. Moved embedding generation from a nightly batch to a streaming job on [Kafka / Kinesis / Pub/Sub], processing [N] events a second.
5. Built PII detection and redaction on [N]M records before they reach any model, passing [audit / DPIA] with no findings.
6. Built the labeling pipeline ([tool]) with guidelines, QA sampling and agreement tracking; [N] annotators produced [N]K labels at [X%] accuracy.
7. Deduplicated a [N]M-document corpus with [MinHash / embeddings], removing [X%] near-duplicates and improving retrieval precision by [Y%].
8. Built data quality checks (schema, freshness, volume) that alert on upstream breakage, catching [N] incidents before they reached users.
9. Built the logging pipeline that captures every prompt, retrieval and response with user consent flags, the source for evals and fine-tuning data.
10. Orchestrated [N] pipelines in [Airflow / Dagster / Prefect], with [X%] on-time runs over [period].
11. Cut pipeline cost by [X%] by moving [step] from [service] to [service] and batching embedding calls.
12. Built a document versioning scheme so answers cite the version in force at the time, fixing [N]% of compliance escalations.
13. Built a feedback pipeline from thumbs up/down and edits to labeled examples, adding [N] examples a week to the eval and training sets.
14. Backfilled [N]M historical records into the new index in [N] hours with idempotent jobs and checkpointing.
15. Built access-control sync so the retrieval layer respects source permissions for [N]K users, verified with [N] automated tests.
16. Built the data warehouse tables (dbt) for AI usage, cost and quality metrics used by [N] teams.
17. Built OCR plus layout processing for [N]K scanned documents a month, raising field extraction accuracy from [A]% to [B]%.
18. Reduced pipeline failure rate from [A]% to [B]% with dead-letter queues, retries with backoff and per-source health checks.
19. Built data retention and deletion jobs that remove user data from indexes and logs within [N] days of a request.
20. Documented every data source used by AI features (owner, freshness, permissions), the input for the company's AI inventory.

## More bullets (Nov 2026)

These add the conditions that make a number checkable: the size of the test set, the baseline, the load and the date. Every number is still a placeholder; keep a condition only if it is true for your work. See [evaluation vocabulary to get right](README.md#evaluation-vocabulary-to-get-right) for the terms.

Last checked: 17 Nov 2026

21. Built a versioned ingestion pipeline for [N]M records a day, cutting processing time from [A] to [B] hours with partitioned runs and checkpointed retries, measured over [period].
22. Raised training-label agreement from [A] to [B] by rewriting guidelines and adjudicating [N] disputed examples, and linked each label version to the model and eval runs that used it.
23. Removed [X%] duplicate and near-duplicate training content with [MinHash / embeddings], then measured the effect on held-out [metric] and on a [N]-prompt memorization test.
24. Built PII filtering and access controls for [dataset], catching [X%] of labeled sensitive items on a [N]-item audit set, with the remaining misses written up and tracked.
25. Added data-quality checks, lineage and backfills to [pipeline], cutting training runs that failed on bad data from [A] to [B] per [month / quarter].

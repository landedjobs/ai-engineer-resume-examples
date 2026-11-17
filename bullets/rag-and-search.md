# Bullet bank: RAG and search

24 bullets for retrieval-augmented generation, search and knowledge assistants. Replace every `[placeholder]` with your own numbers and nouns. If you can't fill a placeholder honestly, pick a different bullet.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values, `[metric]` the measure you used.

1. Built a RAG assistant over [N] [internal docs / help articles / contracts] using [vector store] and [reranker], used by [N] [employees / customers] a week.
2. Raised answer accuracy on a [N]-question golden set from [A]% to [B]% by adding hybrid search (BM25 + embeddings) and a cross-encoder reranker.
3. Lifted retrieval recall@[k] from [A] to [B] on [N] labeled queries by switching from fixed-size chunks to [structure-aware / semantic] chunking.
4. Cut wrong-citation answers from [A]% to [B]% by requiring quoted source spans and rejecting answers whose quotes don't match retrieved text.
5. Added query rewriting for [vague / multi-part / conversational] questions, raising [metric] by [X%] on the hardest [N] queries in the eval set.
6. Built per-tenant index isolation for [N] customer workspaces, with access checks on every retrieved chunk, passing [security review / pen test] with no findings.
7. Migrated [N]M embeddings from [old store] to [new store], keeping recall@[k] at [B] and cutting storage cost by [$N / X%] a month.
8. Reduced index staleness from [A hours] to [B minutes] by moving embedding into the ingestion pipeline with change detection.
9. Replaced keyword search with hybrid retrieval and reranking for [N]M [products / listings / records], raising [click-through / search-to-cart] by [X%] in an A/B test.
10. Brought p95 retrieval latency from [A]ms to [B]ms with [HNSW tuning / caching / parallel shard queries] at [N] queries per second.
11. Added a "no good answer" path that declines when retrieval confidence is low, cutting unsupported answers by [X%] with a [Y%] drop in answer rate.
12. Built metadata filtering (date, product, region) into retrieval, fixing [N]% of golden-set failures caused by outdated documents.
13. Parsed [N]K [PDFs / scanned forms / slide decks] including tables and images into retrievable chunks, lifting accuracy on table questions from [A]% to [B]%.
14. Evaluated [N] embedding models on a domain-specific retrieval set and chose [model], improving recall@[k] by [X%] at [Y%] lower cost.
15. Fine-tuned an embedding model on [N]K [query, document] pairs from search logs, raising NDCG@10 by [X%] over the base model.
16. Designed the retrieval eval set ([N] queries, labeled by [who]) now used to gate every index or chunking change.
17. Built a citation UI that links each answer sentence to its source passage; [X%] of users clicked a citation, and support escalations about wrong answers fell by [Y%].
18. Added conversational memory to the assistant (query condensation over the last [N] turns), lifting follow-up question accuracy from [A]% to [B]%.
19. Diagnosed a [X%] accuracy drop to [stale index / chunking bug / embedding model change] within [N] hours using retrieval traces, and added an alert for it.
20. Wrote the internal RAG playbook used by [N] teams, covering chunking, hybrid search, reranking and evaluation.

## More bullets (Nov 2026)

These add the conditions that make a number checkable: the size of the test set, the baseline, the load and the date. Every number is still a placeholder; keep a condition only if it is true for your work. See [evaluation vocabulary to get right](README.md#evaluation-vocabulary-to-get-right) for the terms.

Last checked: 17 Nov 2026

21. Raised retrieval recall@5 from [A]% to [B]% on [N] held-out support queries by combining keyword and vector search with a reranker, and lifted the share of answers users accepted with a citation from [A]% to [B]% over [period].
22. Cut p95 retrieval latency from [A]ms to [B]ms at [N] queries per second by tuning metadata filters and index settings, keeping recall@[k] within [N] points of the baseline on the same [N]-query set.
23. Built incremental ingestion for [N]K documents with versioned chunks, idempotent updates and deletion propagation, cutting freshness lag from [A] hours to [B] minutes, measured on [date].
24. Built permission-aware retrieval for [N] teams that blocked unauthorized results in all [N] access-control test cases, while answer success on authorized queries stayed at [X%] against a [B]% baseline.

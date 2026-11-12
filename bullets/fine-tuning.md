# Bullet bank: fine-tuning and post-training

20 bullets for fine-tuning, distillation and preference training. Replace every `[placeholder]` with your own numbers and nouns. Only claim the method you used: interviewers ask about it.

Placeholders: `[N]` a count, `[X%]` a percentage, `[A]`/`[B]` before and after values.

1. Fine-tuned [model size] open model with LoRA on [N]K labeled [examples], matching [frontier model] on our eval at [1/N] the cost per request.
2. Built the training data pipeline (collection, dedup, filtering, labeling) that produced [N]K examples for [task] from production logs.
3. Ran a fine-tuning vs prompting vs retrieval comparison on [N] tasks; fine-tuning won on [N] and we shipped it only there.
4. Trained a classifier head on [model] for [intent / toxicity / routing], reaching [X%] F1 on [N] held-out examples at [N]ms latency.
5. Applied DPO on [N]K preference pairs from user feedback, raising win rate against the base model from [A]% to [B]% in blind review.
6. Fine-tuned an embedding model on [N]K domain pairs, raising retrieval recall@[k] by [X%].
7. Distilled [large model] outputs into a [small model] for [task], keeping [X%] of quality at [Y%] lower latency.
8. Set up training runs on [N] GPUs with [FSDP / DeepSpeed], cutting training time for [model] from [A] to [B] hours.
9. Built the eval suite for fine-tuned models, including checks for regressions on general ability and safety, run on every checkpoint.
10. Found and removed [X%] of training examples that leaked eval data, then re-measured; reported the honest score to stakeholders.
11. Fine-tuned a model to follow [company] output format and style, cutting post-processing failures from [A]% to [B]%.
12. Built a synthetic data generator for [task] with [method], validated by [N] human reviews; the model trained on it beat the baseline by [X%].
13. Ran hyperparameter sweeps on [N] configurations and documented the settings that mattered for [task].
14. Merged and served [N] LoRA adapters on one base model, supporting [N] customers' custom models with no extra GPU cost.
15. Trained a reward model on [N]K human ratings to score [outputs], reaching [X%] agreement with held-out human judgments.
16. Fine-tuned a vision-language model on [N]K [documents / images] for [task], raising accuracy from [A]% to [B]%.
17. Built a continual training loop that retrains [model] [weekly / monthly] on new labeled data, keeping accuracy within [N] points as inputs drifted.
18. Wrote the data card and model card for [model], covering data sources, known failure cases and evaluation results.
19. Reduced labeling cost by [X%] with model-assisted labeling and active learning, while keeping label accuracy above [Y%].
20. Decided against fine-tuning for [task] after a [N]-week study showed retrieval fixes gave [X%] more lift; documented it as the team's reference.

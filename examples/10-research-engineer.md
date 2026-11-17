# Example 10: Research engineer (LLM evals and post-training)

> **Fictional person.** Tomasz Lindqvist, his employers, papers and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** mid, 3 years after a master's. **Target roles:** research engineer, member of technical staff (research), evals engineer. **Background:** research engineer at an AI startup's research team, with two workshop papers and one open-source eval harness.

A publication title alone doesn't tell the reader what you did. Did you build the training pipeline, design the eval, or run the analysis? This resume answers that for every piece of research: the question, what he built, the comparison, the result and his share of the work.

---

## The resume

**Tomasz Lindqvist**
London, UK (open to relocation) · tomasz.l@example.com · (555) 010-3390
github.com/tlindqvist-example · Full CV and papers: tomaszl.example.com

**Research interests**
Evaluating agents on long, multi-step tasks; reward signals for code generation; making eval results reproducible.

**Experience**

**Research Engineer**, Meridian Labs (fictional) · London, UK · *Sep 2023 to present*
*AI startup, 80 people, 12-person research team training code models*
- Asked whether unit-test pass rate was a good enough reward for code RL; built the comparison myself (pass rate vs. pass rate plus a learned style critic) on 3 model sizes; the critic cut reward-hacked solutions from 11% to 3% at equal pass@1. Led the experiments; a colleague trained the critic.
- Built the team's agent eval harness: 640 repository-level tasks in sandboxed containers, deterministic replays and per-task traces; it runs nightly on every checkpoint, and 9 researchers use it to make go/no-go calls.
- Found that 7% of a public benchmark's tasks had broken or leaked tests; wrote the filter, re-scored 5 public models and showed the ranking changed for 2 of them. Results written up as a workshop paper (first author).
- Cut eval cost per checkpoint from 41 to 12 GPU-hours with caching of environment builds and early stopping on clearly failed trajectories, with no change in scores on a 200-task check set.
- Ran ablations on a SFT data mix (6 variants, 3 seeds each); found that removing synthetic docstrings raised pass@1 by 2.4 points and changed the team's data pipeline.

**Research Intern**, Bramblewood AI Lab (fictional) · Cambridge, UK · *Jun 2022 to Sep 2022*
- Implemented a LoRA fine-tuning baseline for a retrieval-augmented QA project; matched the full fine-tune within 1 point of exact match at 8% of the GPU memory.

**Selected research**

**Leaky tests in code benchmarks** · *Workshop paper, 2025, first author*
- Question: do public code benchmarks reward wrong solutions? Built the test-audit pipeline, labeled 400 tasks with a co-author (agreement 0.86 kappa), released the cleaned split and code.

**Critic rewards for code RL** · *Workshop paper, 2024, second author*
- Ran all reward-hacking analysis and wrote the eval section. Code and checkpoints public.

**Open source**

**taskbench** (author, 610 GitHub stars) · sandboxed, reproducible agent eval harness; 14 outside contributors.

**Education**

**MSc, Machine Learning**, Kingsbridge College (fictional) · *2023* · Thesis on reward model calibration
**BSc, Mathematics and Computer Science**, Kingsbridge College (fictional) · *2021*

**Skills**

Research: experiment design, ablations, multi-seed evaluation, statistical testing, reward modeling, RL for code, SFT, LoRA
Engineering: Python, PyTorch, JAX (reading level), Ray, Docker sandboxes, Slurm, Kubernetes, Weights & Biases

---

## Why this works

- **Every research bullet has a question, a comparison and a result.** "Asked whether pass rate was a good enough reward" turns a vague topic into an experiment with a decision at the end. That is the habit research teams screen for.
- **His share of the work is stated.** "Led the experiments; a colleague trained the critic" and "second author, ran all reward-hacking analysis" tell the reader exactly what to ask him about.
- **Papers link to artifacts.** Each paper has code, a dataset or checkpoints behind it, and the harness is public with stars and outside contributors. A reader can check the work.
- **Engineering shows up next to research.** Sandboxed containers, deterministic replays and a 70% cut in GPU-hours per checkpoint show he can build the infrastructure research depends on.
- **It stays one page.** The full publication list, talks and reviewing go in the longer CV on his site. The resume carries only the research that matches the role.

## What to change for each kind of employer

**Frontier lab.** Keep this order. Add model sizes, compute and the decision each experiment changed. If you have a stronger paper (main conference), move it to the top of Selected research. Link the longer CV, since many lab research teams read it.

**Startup.** Lead with the eval harness and the cost cut, then the research. Startups hiring research engineers want someone who ships tools other people use. Say how many people relied on it and what calls it informed.

**Enterprise.** Reframe the eval work as model evaluation and quality assurance for production, and the benchmark audit as risk detection. Move Skills above Selected research. Use the posting's terms (model validation, responsible AI, evaluation frameworks) where true.

*Last checked: 17 Nov 2026*

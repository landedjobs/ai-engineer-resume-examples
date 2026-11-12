# Example 01: New grad or career switcher AI engineer

> **Fictional person.** Maya Okafor, her schools, employers, projects and numbers are invented for this example. Any resemblance to a real person is a coincidence.

**Level:** entry. **Target roles:** AI engineer, applied AI engineer, junior LLM engineer. **Background:** BS in computer science, one software internship, two serious LLM projects.

The hardest resume to write. You have no production LLM job to point to, so the projects carry the page. They go above experience.

---

## The resume

**Maya Okafor**
Austin, TX · maya.okafor@example.com · (555) 010-4471
github.com/maya-okafor-example · mayaokafor.example.com · Eval report: mayaokafor.example.com/evals

**Projects**

**CourseMate**, RAG study assistant for a 900-student intro CS course · Python, FastAPI, Postgres + pgvector, React · *Jan 2026 to present*
- Built a retrieval assistant over 1,400 pages of lecture notes, slides and past forum answers; 312 students used it in the spring term, asking 6,800 questions.
- Wrote a 250-question golden set with two TAs and measured answer correctness; moved it from 64% to 86% by adding hybrid search (BM25 + embeddings) and a cross-encoder reranker.
- Cut wrong-citation answers from 11% to 2% by forcing quoted source spans in the output schema and rejecting answers whose quotes don't appear in the retrieved chunks.
- Kept cost under $40 a month for the whole term by caching repeated questions and routing short factual questions to a smaller model.

**ReceiptAgent**, tool-using agent for shared-expense tracking · Python, OpenAI-compatible tool calling, SQLite, Telegram bot API · *Sep to Dec 2025*
- Built an agent with 5 tools (OCR, currency lookup, split calculator, ledger write, reminder) that turns a photo of a receipt into a settled split; 41 people in 9 group chats used it for 3 months.
- Logged every agent run as a trace and built a 120-case test suite from real failures; task success went from 58% to 91% after fixing tool descriptions and adding a confirm step before ledger writes.
- Wrote a public write-up on the 6 failure types I saw (wrong tool, looping, hallucinated totals) and how each was fixed; 4,200 reads.

**Experience**

**Software Engineering Intern**, Tidewater Logistics (fictional) · Dallas, TX · *May to Aug 2025*
- Built an internal FastAPI service that classifies inbound shipping emails into 7 queues with an LLM and a rules fallback; it handled 3,000 emails a day by the end of the internship.
- Added an evaluation script over 500 hand-labeled emails that the team now runs before every prompt change; it caught 2 regressions before release.
- Wrote integration tests that raised coverage of the email service from 34% to 78%.

**Teaching Assistant, Intro to Programming**, Lakeshore State University (fictional) · *Aug 2024 to May 2025*
- Ran weekly labs for 60 students and wrote 14 autograded assignments in Python.

**Education**

**BS, Computer Science**, Lakeshore State University (fictional) · *May 2026* · GPA 3.8
Relevant courses: Machine Learning, Natural Language Processing, Distributed Systems, Databases

**Skills**

Languages: Python, TypeScript, SQL
LLM and retrieval: RAG, hybrid search, reranking, embeddings, tool calling, structured output
Evals: golden sets, LLM-as-judge, trace review
Tools: FastAPI, Postgres + pgvector, Docker, GitHub Actions, AWS (Lambda, S3)

---

## Why this works

- **Projects go first** because they are the strongest evidence. A hiring manager sees real users (312 students, 41 people) in the first five lines.
- **Each project has an eval.** The 250-question golden set and the 120-case test suite are what separate this from a tutorial project. Most entry-level resumes have no measurement at all.
- **Failures are on the page.** "Wrong-citation answers from 11% to 2%" and the write-up on 6 failure types show she has debugged a system, which is most of the job.
- **Cost appears once.** "$40 a month for the whole term" is small, and that's the point: it shows she thought about cost before anyone asked.
- **The internship bullets are AI work.** The title says software engineering intern, the bullets show the LLM classifier and the eval script. The title stays honest.
- **Links are visible text**, including a direct link to the eval report.

## If you're a career switcher

Use the same shape. Add a two-line summary at the top that names your old field and the bridge:

> Former high-school physics teacher, now building LLM applications. Shipped a RAG study assistant used by 312 students, with a public eval report.

Then keep projects first, put your previous career under Experience with 2 bullets that show measurable work (you ran a 120-student program, you built the school's grading spreadsheet that 30 teachers use), and move Education to the bottom. Don't hide the old career. Domain knowledge is an asset when you apply to AI companies in that domain (edtech, health, legal).

## What to change for each kind of employer

**Frontier lab (applied or product engineering roles).** Labs hire few new grads, and the bar is coding depth plus fundamentals. Add one bullet that shows you understand what's under the API: an implementation of attention from scratch, a small fine-tuning run with a measured result, or a tokenizer you wrote. Keep the eval detail. Move GPA and the ML/NLP coursework higher.

**Startup.** Lead with users and speed. Add how fast you shipped ("first version live in 9 days"). Put the live demo link first in the header. Startups care less about GPA; you can drop it if space is tight.

**Enterprise (bank, insurer, retailer, consulting).** Stress reliability and process: tests, the eval script that gates changes, the rules fallback in the internship classifier, cost control. Add a line on data handling if true ("no student data stored; questions logged without user IDs"). Use the posting's exact terms, since enterprise ATS filters lean harder on keyword match.

# Tailor your resume to a posting without keyword stuffing

Tailoring is choosing which of your true facts go first for this job, and using the posting's words where they describe what you did. It is not adding skills you don't have, renaming your job, or pasting the posting into your skills line.

This page gives a step-by-step method, then works through one real AI engineer posting with a fictional candidate. A second real posting with the same title shows how the same person's resume should change again.

*Last checked: 17 Nov 2026.*

## Contents

- [Why tailor at all](#why-tailor-at-all)
- [Keywords: what is known and what isn't](#keywords-what-is-known-and-what-isnt)
- [The method, step by step](#the-method-step-by-step)
- [Worked example: Baseten, AI Engineer](#worked-example-baseten-ai-engineer)
- [Same title, different proof: Elicit, AI Engineer](#same-title-different-proof-elicit-ai-engineer)
- [What you never change](#what-you-never-change)
- [Check the result](#check-the-result)

## Why tailor at all

The first people to read your resume are usually a recruiter or sourcer, then the hiring manager. They are looking for experience that resembles the job they are filling.

Recruiters say this openly. In an [OpenAI Forum session on 5 Feb 2026](https://forum.openai.com/public/videos/event-replay-get-hired-using-chatgpt-tips-from-openais-head-of-recruiter-programs-2026-02-05), Selena Ma, OpenAI's head of recruiting programs, advised tailoring your resume when you apply to different kinds of jobs or industries. She suggested reading the job description for the skills it wants, then picking the bullets from your career that match. She was just as clear about the limit: "You can't lie about your resume or inflate."

[Anthropic's guidance on candidates' AI use](https://www.anthropic.com/candidate-ai-guidance) (read 17 Nov 2026) asks you to write the first draft yourself and then use Claude to refine it. Its example prompt asks Claude to compare your resume with the job description and say which experiences align most. That is the same idea: select real experience, don't invent it.

## Keywords: what is known and what isn't

Keywords matter some. They don't matter the way "ATS score" tools suggest.

- **Recruiters search.** Greenhouse lets recruiters run [Boolean searches across candidates](https://support.greenhouse.io/hc/en-us/articles/202360199-Search-candidates-using-Boolean-queries), including resume text (article last updated 2 Mar 2026). If a recruiter searches "RAG" OR "retrieval-augmented generation" and neither appears on your resume, you don't come up.
- **Some screening is per employer and per criterion.** Ashby's [AI-assisted application review](https://docs.ashbyhq.com/ai-assisted-application-review) checks resumes against criteria the employer writes for that job. It can show recruiters the percentage of criteria each candidate met (read 17 Nov 2026). That is a list of requirements a person wrote, not a keyword count.
- **There is no known universal score, keyword count or density target.** No public ATS documentation we found describes one. Treat any "match %" tool as an editing aid.

So the practical rules, which are our advice:

1. Use the posting's term where it is true for you. If it says "evals" and you wrote "quality testing", say "evals".
2. Write the full term and the acronym once each when both are common: "retrieval-augmented generation (RAG)".
3. Put important terms inside bullets that show you used them, not only in the skills line.
4. Never add a hidden or white-text keyword block. Parsers read it as plain text, so a recruiter can see it.
5. Never list a tool you haven't used because the posting names it. The interview will find it.

## The method, step by step

These steps are our recommendation. No tool can predict a hiring decision, and neither can this list.

1. **Find the outputs.** Read the responsibilities and ask: what will this person build, run, measure or fix in the first six months? Write that down in one sentence.
2. **Split must-haves from nice-to-haves.** Most postings label them. Ignore the company boilerplate and the benefits.
3. **Map each must-have to your evidence.** Make a two-column list: requirement, and your strongest true bullet for it. A blank row is a gap. Don't fill it with words.
4. **Pick your top three.** The three bullets that answer the most important must-haves go first under your most recent role.
5. **Rewrite the summary** (if you use one) so its two lines answer the step 1 sentence.
6. **Adjust the skills line.** Reorder it so the posting's must-have terms that are true for you come first. Remove items that are irrelevant to this job and crowd the line.
7. **Use the posting's words only where accurate.** Swap a synonym for their term. Don't copy their phrases.
8. **Check every fact against your master version.** Numbers, titles and dates must be identical across every version you send.
9. **Run a check, then read it yourself.** Use a checker or an AI model to find gaps and vague bullets. Then verify every change by hand.

Keep a master resume with every bullet you have ever written, with the real numbers. Tailoring is choosing from it, not writing new claims.

## Worked example: Baseten, AI Engineer

**The posting.** [Baseten, AI Engineer](https://jobs.ashbyhq.com/baseten/b13ec426-d09d-4122-8112-cf25adbd7d60), San Francisco, published 20 Aug 2026 and open when we checked on 17 Nov 2026. Postings close; if the link is dead, the method still applies to the next one.

**What it asks for, in our words.**

- The job: build agent features for customers who train and post-train models on Baseten. Also, turn manual internal work into agent workflows for other teams.
- You design the harnesses, execution flows and guardrails that make agents reliable.
- You define evals so you know whether a change helped.
- You work across the API layer, backend, agent orchestration and some frontend.
- Must-haves: 5+ years shipping software; AI or agent products that real users depend on; strong engineering fundamentals beyond prompting; Python plus one other language; working with little structure; moving between customer product work and internal tooling.
- Nice-to-haves: founding or early startup experience; evals and agent observability; agent frameworks and MCP; fine-tuning or RL; frontend.

**One-sentence output (step 1).** This person ships production agents with the harness and evals that make them dependable, and builds internal AI tools other teams use.

**The candidate.** Sam Okafor is fictional, as are their employer and numbers. Senior software engineer at Tallyfield (fictional), a 400-person B2B SaaS company. 6 years in Python and Go backends, the last 2 on LLM features. Assume every detail below is true and is in Sam's master resume. Tailoring only moves true facts to the front; it never adds new ones.

**The map (step 3).**

| Posting must-have | Sam's evidence | Placement |
|---|---|---|
| Agent products real users depend on | Support agent resolving 38% of tickets end to end | First bullet |
| Harnesses and guardrails | Step limit, confirmation before refunds, human hand-off (in master notes, not yet on the page) | Inside the first bullet |
| Evals | 450-ticket eval suite, LLM judge at 91% agreement with human labels, runs in CI | Second bullet |
| Internal tooling for other teams | Slack bot that drafts incident summaries for 4 on-call teams | Third bullet (was fifth) |
| Python plus another language | Python and Go | Skills line, first |
| Fine-tuning or RL (nice to have) | None | Leave it out |

### Summary

| Before (Sam's general version) | After (for Baseten) |
|---|---|
| Backend engineer with 6 years in Python and Go services, the last 2 on LLM features. Shipped a support agent, an internal search tool and the eval suite behind both. | Backend engineer, 6 years in Python and Go, the last 2 building agents that customers rely on. Shipped a support agent that resolves 38% of tickets end to end, plus the eval and tracing harness that gates every change to it. |

What changed: the summary now answers the one-sentence output. The search tool drops out of the summary because this job doesn't ask for search. The 38% comes up from the bullets.

### Skills line

| Before | After |
|---|---|
| Languages: Python, Go, SQL | Languages: Python, Go, SQL |
| AI: RAG, prompt engineering, OpenAI API, LangChain | Agents and evals: tool calling, agent harnesses and guardrails, evals (golden sets, LLM-as-judge), tracing, LangChain |
| Infra: AWS, Postgres + pgvector, Redis, Docker, Kubernetes | Infra: AWS, Postgres, Redis, Docker, Kubernetes |

What changed: the AI line now leads with what the posting asks for, using its words ("harnesses", "guardrails", "evals"). Sam already did all of it. LangChain stays because Sam used it and the posting lists agent frameworks. Nothing new was added. "Claude Code", "Codex" and "MCP" are in the posting, but Sam hasn't used them, so they stay off.

### The three lead bullets

| | Before (top three in the general version) | After (top three for Baseten) |
|---|---|---|
| 1 | Built an internal search tool over 120K Confluence and Google Drive pages with pgvector and a reranker; 600 employees use it weekly. | Shipped a tool-using support agent (5 tools, a 12-step limit, confirmation before refunds, hand-off to a human) that resolves 38% of customer tickets end to end. |
| 2 | Shipped a tool-using support agent (5 tools plus a human hand-off) that resolves 38% of tickets end to end. | Built the agent's eval suite (450 real tickets, LLM judge at 91% agreement with human labels) and ran it in CI on every prompt and model change. |
| 3 | Built an eval suite of 450 real tickets with an LLM judge at 91% agreement with human labels, run on every prompt change. | Built a Slack bot that drafts weekly incident summaries from PagerDuty and Jira for 4 on-call teams, turning a manual write-up into a review step. |

What changed:

- **Order.** The agent moves to the top because "agents real users depend on" is the main must-have. The search tool moves to fourth place; it is still on the page.
- **Detail surfaced, not invented.** The step limit and the refund confirmation were already true. The general version left them out. Here they answer "harnesses and guardrails".
- **Same numbers.** 38%, 450 and 91% are identical in both versions.
- **Internal tooling moves up.** The posting wants someone who automates other teams' work. The Slack bot was Sam's fifth bullet; for this job it is third.

## Same title, different proof: Elicit, AI Engineer

Now Sam applies to [Elicit's AI Engineer role](https://elicit.com/careers/d27d51d7-b318-4cb0-9b88-c37de18905f3) (Oakland or remote in US time zones; listed on [Elicit's careers page](https://elicit.com/careers) on 17 Nov 2026, with no publish date shown). Same title, different job.

The posting pitches the role to backend engineers who like the hard parts: concurrency, fault tolerance and distributed systems. The work sits between the product's backend-for-frontend endpoints and the models. It asks for a "defensive, fault-first mindset". Its self-check questions cover Python async libraries, JavaScript's `await`, Kubernetes pods, and managing state in an LLM conversation.

Elicit has also published what its interviews touch on. In a [June 2024 post on hiring AI engineers](https://elicit.com/blog/how-to-hire-ai-engineers), Elicit's James Brady lists example topics from a coding exercise. These include converting a synchronous REST API to an asynchronous streaming endpoint and cancelling async work when a user closes the tab. That post is from 2024, so treat it as a sign of what the team values, not as the current interview.

So Sam leads with different true bullets:

| | For Baseten | For Elicit |
|---|---|---|
| Bullet 1 | Support agent with harness and guardrails, 38% resolved | Moved the agent's answer endpoint from blocking responses to streamed server-sent events, cancelling model calls when the user closes the tab; p95 time to first token fell from 6.2s to 0.9s. |
| Bullet 2 | Eval suite in CI | Support agent, now with the state detail: conversation state kept server-side so a dropped connection resumes mid-task, 38% resolved end to end. |
| Bullet 3 | Slack bot for on-call teams | Eval suite in CI (unchanged). |
| Skills line leads with | Agents, harnesses, evals | Python (asyncio), Go, Kubernetes, Postgres, then the AI line |
| Drops to the bottom | Search tool | Slack bot and search tool |

The streaming bullet was in Sam's master resume all along. For Baseten it didn't make the top three. For Elicit it is the best evidence on the page. The facts are identical across both versions; only the choice and the order changed.

For more on how the proof differs by role (ML engineer, LLM engineer, research engineer, FDE), see [roles.md](roles.md).

## What you never change

- **Job titles.** Sam's title stays "Senior Software Engineer" even though both postings say "AI Engineer". Reference checks compare titles.
- **Dates and employers.**
- **Numbers.** If 38% is true, it is 38% in every version. Don't round up for one company.
- **Methods.** Baseten lists fine-tuning and RL as nice to have. Sam hasn't done them, so they appear nowhere. Don't relabel prompt work as fine-tuning, or fine-tuning as RL.
- **Tools.** Only ones you have used. A posting naming MCP is not a reason to list MCP.
- **The posting's own sentences.** Use their terms, not their phrasing. A bullet that echoes the job ad word for word reads as copied.
- **Links.** The same GitHub, demo and eval report in every version. Check each one works on the day you apply.

## Check the result

Before you send a tailored version:

1. Read it next to your master resume and confirm every number, title and date matches.
2. Read only the top third. Does it answer your one-sentence output for this job?
3. Paste it and the posting into the free [landed ATS resume checker](https://www.landed.jobs/tools/ats-resume-checker?utm_source=github&utm_medium=referral&utm_campaign=github-ai-engineer-resume-examples&utm_content=ats-checker). It checks your format and your keyword overlap with the posting. A missing term you have real experience with is worth adding to a bullet. A missing term you don't have stays missing.
4. Read the questions on the application form and check that your answers match the resume. Greenhouse, for example, lets employers [auto-reject applicants based on their answers](https://support.greenhouse.io/hc/en-us/articles/360000653472-Auto-reject) to custom application questions (article last updated 30 Jan 2026). Answer them carefully and truthfully.

Back to the [main README](README.md).

---

<sub>No affiliation with the companies named. Sam Okafor, Tallyfield and every number in the worked example are fictional. Postings are summarized as they read on the dates given.</sub>

# Make your projects inspectable: GitHub, demos and eval reports

A resume line can only claim. A link can prove. This page covers what a project link should show that the resume can't, the four pieces of evidence we recommend for each project, where each link goes, and some open-source tools worth building with.

*Last checked: 17 Nov 2026*

## Contents

- [What a project link must answer](#what-a-project-link-must-answer)
- [The evidence package](#the-evidence-package)
- [Where each link goes](#where-each-link-goes)
- [Confidential work](#confidential-work)
- [Recommended repositories and their licences](#recommended-repositories-and-their-licences)
- [Templates and build guides](#templates-and-build-guides)

## What a project link must answer

A resume bullet has room for one result. The reader who clicks your link wants answers to the questions the bullet raised:

1. **What exactly did you build, and which part was yours?** A repo that wraps someone else's framework should say what you added.
2. **How do you know it works?** A held-out test set, a metric, a baseline, and the number that moved.
3. **What does it cost, and how fast is it?** Latency and cost per request, measured under stated conditions.
4. **Where does it fail?** At least one failure case and what you did about it, or what you would do next.
5. **What did you decide, and why?** The alternatives you tried or rejected.

The fifth point matters more now that coding agents write much of the code. In a 30 Mar 2026 post, Elicit described a strong interview candidate who [flagged a gap in the spec before writing any code](https://elicit.com/blog/engineering-interviews-in-the-era-of-agents), wrote down the assumption, and did not finish every requirement but could explain each choice. In its 22 Jun 2024 hiring guide, Elicit asked for [one or more serious projects on a unique domain](https://elicit.com/blog/how-to-hire-ai-engineers) and a "defensive, fault-first mindset" about latency, variance and errors.

Our reading: a project page should keep the evidence of judgment (options considered, assumptions, checks, the decision that followed), not only the finished code.

## The evidence package

For each project you put on the resume, we recommend four pieces. Each answers different questions.

| Piece | What it should contain | What to avoid |
|---|---|---|
| **Repository** | Code that runs from a clean clone, tests, a licence, a clear commit history | A dump of notebooks with no entry point |
| **README** | One-line purpose, results table at the top, architecture, setup in under 5 commands, design decisions, limitations, your contribution, licence | A generated introduction with no runnable instructions |
| **Demo or video** | One real workflow end to end, plus at least one failure or "I don't know" path. A 60 to 90 second video works when a live demo would cost you money | Only a hand-picked happy path |
| **Eval report** | Task, data source and rights, held-out split, metric definitions, graders and how they were checked against humans, baseline, quality vs. latency vs. cost, failure slices, how to reproduce | One aggregate score with no explanation |

For the eval report, OpenAI's [evaluation best practices guide](https://platform.openai.com/docs/guides/evaluation-best-practices) is a good technical basis. It recommends mixing production data with cases created by domain experts, covering edge cases, and calibrating automated scoring against human feedback. Keep the held-out set separate from the examples you looked at while building.

If you contributed to someone else's open-source project, the evidence is the specific merged PR, issue, benchmark or doc you wrote. Link that, not the project's home page.

## Where each link goes

| Surface | Put here | Avoid |
|---|---|---|
| **Resume project entry** | Problem, what you owned, the strongest measured result, then short links to repo, demo and eval report | A feature list with no outcome |
| **Resume header** | One link to your best single piece of evidence (usually an eval report or write-up), plus GitHub | Five links of equal weight |
| **GitHub profile** | Pinned repos for the 2 to 4 projects on your resume, and a profile README that says what each one shows | Every tutorial fork and experiment |
| **LinkedIn** | A headline for the role you want, the same claims and dates as the resume, and Featured items for a case study, a demo and an eval report | Titles or ownership the resume doesn't support |

On GitHub, you can [pin up to six repositories and gists, combined](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/pinning-items-to-your-profile). A [profile README](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme) appears when you have a public repository named after your username with a non-empty README.md in its root. Use the pins for your strongest relevant work, not your most recent.

On LinkedIn, a secondary guide dated 25 Aug 2026 lists [four types of Featured item](https://cvmadebetter.com/linkedin-featured-section): your posts, articles or newsletters, external links, and uploaded media such as PDFs, slides and images. Our suggestion is three items: a project case study, a demo, and an eval report. This is a presentation choice, not a claim about how LinkedIn ranks profiles.

A simple rule we use: every link on the resume should open a specific piece of evidence (a result, a decision, a contribution, a reproducible artifact). A link to a bare GitHub profile with 40 repos makes the reader do the work.

## Confidential work

Most production AI work can't be published. In that case:

- Write a sanitized account of the architecture, your decisions and the numbers you are allowed to share, and get it approved if your employer requires that.
- Say plainly that code and exact figures are private. Don't invent public evidence to fill the gap.
- Link a public project that shows the same skill (for example, a small public eval harness if your work eval harness is private).

## Recommended repositories and their licences

These are good tools to build with or learn from. Using a well-known framework is not an achievement on its own; your resume should say what you built with it and what you measured.

| Repository | Use it for | Licence | Stars |
|---|---|---|---|
| [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) | Versioned prompt, RAG and agent evals, and red-team checks run in CI | MIT | 27.4K |
| [vibrantlabsai/ragas](https://github.com/vibrantlabsai/ragas) (formerly explodinggradients/ragas) | Evaluating LLM applications and generating test sets | Apache-2.0 | 16.4K |
| [vllm-project/vllm](https://github.com/vllm-project/vllm) | Serving experiments: throughput, latency and cost per request on your own hardware | Apache-2.0 | 97.1K |
| [GokuMohandas/Made-With-ML](https://github.com/GokuMohandas/Made-With-ML) | Learning to develop, deploy and iterate on production ML applications | MIT | 50.1K |

Licences and stars from the GitHub API on 17 Nov 2026. Models, datasets and hosted services you use with these tools have their own terms; check those separately before you publish results or redistribute data.

Put a licence on your own project repos too. GitHub's docs note that [without a licence, default copyright applies](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) and nobody may reproduce, distribute or build on your code. A reviewer can still read it, but a licence shows you know how open source works.

## Templates and build guides

Our sister repo, [AI engineer portfolio projects](https://github.com/landedjobs/ai-engineer-portfolio-projects), has templates for each piece of the evidence package:

- [Project README template](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/templates/project-readme.md): results first, then quick start, design decisions, evaluation, failures and limits.
- [Eval report template](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/templates/eval-report.md): what success means, test set, graders, held-out results, cost, failure review.
- [Presenting your project](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/templates/presenting-your-project.md): the resume line, the link, and how to talk about it in the interview.
- [Build guides](https://github.com/landedjobs/ai-engineer-portfolio-projects/blob/main/guides/README.md): 10 step-by-step guides, from production RAG and tool-using agents to LLM serving and fine-tuning, all using the same reporting rules.

For how to write the resume line itself, see [the bullet formula](README.md#the-bullet-formula) and the [example resumes](examples/).

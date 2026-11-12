# Templates

Two plain, single-column templates that parse well in applicant tracking systems. Both are original to this repo and MIT-licensed.

| Template | Best for | File |
|---|---|---|
| Markdown | Fast edits, version control, converting with Pandoc | [resume-template.md](resume-template.md) |
| LaTeX | Fine control over spacing and fonts | [resume-template.tex](resume-template.tex) |

Both use standard headings (Summary, Experience, Projects, Education, Skills), no columns, no icons, no tables for layout, and links as visible text.

## Exporting to PDF

**Markdown with Pandoc.** Install [Pandoc](https://pandoc.org/installing.html) and a LaTeX engine, then run:

```
pandoc resume-template.md -o resume.pdf -V geometry:margin=0.6in -V fontsize=11pt
```

If you don't want to install LaTeX, open the Markdown in any editor with a preview (VS Code, Obsidian, Typora), then print to PDF from the preview.

**LaTeX locally.** With a TeX distribution installed, run:

```
pdflatex resume-template.tex
```

**LaTeX in the browser.** Upload `resume-template.tex` to [Overleaf](https://www.overleaf.com) and compile there. The template uses only standard packages, so it compiles on the free plan.

## Check the PDF before you send it

1. Open the PDF, select all text, and paste it into a plain text editor. If the order is scrambled or words are missing, a parser will see the same mess.
2. Click every link.
3. Keep it to one page unless you're at staff level or above.
4. Name the file `firstname-lastname-resume.pdf`.

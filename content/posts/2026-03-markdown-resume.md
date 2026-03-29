---
title: "A Simpler Markdown Resume (with Pandoc + XeLaTeX)"
date: 2026-03-28
draft: false
---

Mantaining a resume can be a pain. I've tried a lot of setups over the years. A basic word processor is good enough in many respects, but I don't like the lack of full version control or the fussiness of the formatting. I've also tried LaTex, but it's a lot to learn and I would much rather work in clean Markdown. 

If you're set on Markdown, then the question is how to generate a presentable PDF. Pandoc is a great tool for this but getting a work flow set up and managing the formatting can get [rather complicated](https://github.com/mszep/pandoc_resume). I've been searching for a way to get a good result with as few moving parts as possible and here's what I've settled on for now.

1. Put a light YAML header at the top of `resume.md` to set margins, font, and size:
```yaml
---
geometry:
- top=1in
- bottom=1in
- left=1in
- right=1in
mainfont: "Liberation Serif"
fontsize: 11.5pt
pagestyle: empty
---
```

2. Write the resume in plain Markdown below that header, as in this template: https://gist.github.com/BrianZbr/2b85b3e723c515a7da2e3f3c1495d6cf

3. Generate the PDF with Pandoc using XeLaTeX:
```bash
pandoc resume_template.md -o resume.pdf --pdf-engine=xelatex
```

Requirements:
- Pandoc with XeLaTeX support (a TeX distribution that includes `xelatex`).
- Your chosen font installed (e.g., Liberation Serif is what I've been using for [my own resume](/resume.pdf)).

## Optional: automate it
- Keep `resume.md` in a Git repo.
- Use a simple CI job to build the PDF on push and attach it as an artifact.
- If you have a website, a second job can publish the latest PDF to your site's static files.
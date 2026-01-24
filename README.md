# Brian Zbriger's Personal Website

A modern personal website built with Hugo and hosted on GitHub Pages.

**Live Site**: [https://www.brianz.page](https://www.brianz.page)

## Tech Stack

- **[Hugo](https://gohugo.io/)** - Static site generator
- **GitHub Pages** - Hosting
- **GitHub Actions** - Automated deployment
- **[Custom my-sustain theme](themes/my-sustain/)** - Based on [hugo-sustain](https://github.com/natarajanmb/hugo-sustain)

## Quick Start

```bash
# Clone and run locally
git clone https://github.com/BrianZbr/brianzbr.github.io.git
cd brianzbr.github.io
hugo serve --bind 0.0.0.0 --port 1313
```

Visit `http://localhost:1313` to preview.

## Project Structure

```
├── content/          # Site content
├── static/           # Assets (images, resume, CSS)
├── themes/my-sustain/  # Custom theme
├── config.toml       # Hugo configuration
└── .github/workflows/ # CI/CD deployment
```

## Deployment

- **Main branch**: Automatic deployment to production
- **Pull requests**: Preview builds available
- **Custom domain**: Configured via CNAME

## Customization

- **Content**: Edit files in `content/`
- **Theme**: Modify `themes/my-sustain/`
- **Config**: Update `config.toml`
- **Resume**: Replace `static/resume.pdf`

---

**Contact**: mail@brianz.page | **GitHub**: [BrianZbr](https://github.com/BrianZbr/)

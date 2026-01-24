# Brian Zbriger's Personal Website

A modern, responsive personal website built with [Hugo](https://gohugo.io/) static site generator and hosted on GitHub Pages. This site showcases Brian Zbriger's professional profile, projects, and technical skills.

## 🌐 Live Site

- **URL**: [https://www.brianz.page](https://www.brianz.page)
- **Domain**: Custom domain configured via CNAME record

## 🚀 Technology Stack

- **Static Site Generator**: Hugo v0.121+ (latest)
- **Theme**: Customized version of [hugo-sustain](https://github.com/nurlansu/hugo-sustain)
- **Hosting**: GitHub Pages
- **CI/CD**: GitHub Actions for automated deployment
- **Deployment**: Automatic on push to main branch

## 📁 Project Structure

```
brianzbr.github.io/
├── .github/
│   └── workflows/
│       └── gh-pages.yml          # GitHub Actions deployment workflow
├── content/
│   └── _index.md                 # Homepage content
├── static/
│   ├── img/
│   │   ├── headshot.jpg          # Profile picture
│   │   └── headshot-full.jpg     # Full resolution headshot
│   ├── resume.pdf                # Latest resume
│   ├── resume-2021-11.pdf        # Resume version (Nov 2021)
│   ├── resume-2021-12.pdf        # Resume version (Dec 2021)
│   ├── resume-latest.pdf         # Latest resume copy
│   ├── org.css                   # Custom CSS styles
│   ├── music_redirect.html       # Music page redirect
│   └── CNAME                     # Custom domain configuration
├── themes/
│   ├── hugo-sustain/             # Git submodule (upstream theme)
│   └── my-sustain/               # Custom theme modifications
├── config.toml                   # Hugo configuration
├── .gitmodules                   # Git submodule configuration
├── .gitignore                    # Git ignore rules
└── .nojekyll                     # Disable Jekyll processing
```

## ⚙️ Configuration

### Hugo Configuration (`config.toml`)

- **Base URL**: `https://www.brianz.page`
- **Language**: English (US)
- **Title**: Brian Zbriger
- **Theme**: hugo-sustain
- **Author**: Brian Zbriger
- **Avatar**: `/img/headshot.jpg`

### Social Links

- **GitHub**: [BrianZbr](https://github.com/BrianZbr/)
- **Email**: mail@brianz.page
- **LinkedIn**: [brian-zbriger-70a31561](https://linkedin.com/in/brian-zbriger-70a31561)
- **LeetCode**: [BrianZbr](https://leetcode.com/BrianZbr/)

### Navigation Menu

The site includes links to:
- GitHub Profile
- LeetCode Profile
- LinkedIn Profile
- Resume (PDF)
- Email Contact

## 🎨 Theme Customization

This site uses a customized version of the hugo-sustain theme:

### Features
- **Responsive Design**: Mobile-friendly layout
- **Syntax Highlighting**: Code highlighting with highlight.js
- **Social Integration**: Links to professional profiles
- **Custom Styling**: Modified CSS for personal branding
- **Bootstrap Integration**: Responsive grid system

### Theme Structure
- **Upstream Theme**: `themes/hugo-sustain/` (Git submodule)
- **Custom Modifications**: `themes/my-sustain/` (local customizations)

## 🔄 Deployment Process

### GitHub Actions Workflow

The site is automatically deployed using GitHub Actions:

1. **Trigger**: Push to `main` branch or pull request
2. **Steps**:
   - Checkout repository with submodules
   - Setup Hugo (latest version)
   - Build site with minification
   - Deploy to GitHub Pages (main branch only)

### Deployment Configuration

- **Environment**: Ubuntu Latest
- **Hugo Version**: Latest
- **Publish Directory**: `./public`
- **Minification**: Enabled

## 📝 Content Management

### Homepage Content

The homepage (`content/_index.md`) includes:
- Personal introduction
- Featured projects:
  - **Backstage Payroll**: Flask + Postgres REST API with Docker Compose
  - **Geo Trivia**: Text-based quiz game with JSON dataset, live on Replit

### Static Assets

- **Images**: Profile pictures in multiple resolutions
- **Documents**: Resume versions in PDF format
- **Stylesheets**: Custom CSS for enhanced styling
- **Redirects**: HTML redirect for music page

## 🛠️ Local Development

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/installing/) (v0.121+)
- Git

### Setup

1. Clone the repository:
   ```bash
   git clone --recursive https://github.com/BrianZbr/brianzbr.github.io.git
   cd brianzbr.github.io
   ```

2. Start development server:
   ```bash
   hugo serve
   ```

3. Visit `http://localhost:1313` to preview changes

### Build for Production

```bash
hugo --minify
```

The generated site will be in the `public/` directory.

## 📊 Site Features

### Professional Profile
- Personal introduction and background
- IT professional with focus on Python, data, and DevOps
- Links to coding profiles and achievements

### Project Showcase
- Featured projects with descriptions
- Links to live demos and repositories
- Technology stack highlights

### Contact Information
- Multiple contact methods
- Professional social media integration
- Direct email access

## 🔧 Customization Guide

### Adding New Content

1. **Blog Posts**: Create markdown files in `content/blog/`
2. **Projects**: Update `content/_index.md` or create dedicated project pages
3. **Static Assets**: Add files to `static/` directory

### Modifying Theme

1. **Layout Changes**: Edit files in `themes/my-sustain/layouts/`
2. **Style Updates**: Modify `themes/my-sustain/assets/`
3. **Configuration**: Update `config.toml`

### Updating Resume

1. Replace `static/resume.pdf` with new version
2. Update version-specific files if needed
3. Test download links

## 📈 Performance Optimization

- **Minification**: Enabled for HTML, CSS, and JS
- **Image Optimization**: Compressed profile images
- **CDN Delivery**: GitHub Pages CDN
- **Caching**: Proper cache headers via GitHub Pages

## 🔒 Security Considerations

- **No Server-Side Processing**: Static site only
- **HTTPS Enforced**: Via GitHub Pages
- **No Third-Party Scripts**: Minimal external dependencies
- **Content Security**: No user input processing

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

This is a personal website. For issues or suggestions:
1. Check existing issues
2. Create detailed bug reports
3. Provide improvement suggestions

## 📞 Contact

- **Email**: mail@brianz.page
- **GitHub**: [BrianZbr](https://github.com/BrianZbr/)
- **LinkedIn**: [Brian Zbriger](https://linkedin.com/in/brian-zbriger-70a31561)

---

**Last Updated**: January 2026  
**Hugo Version**: Latest (via GitHub Actions)  
**Theme**: hugo-sustain (customized)

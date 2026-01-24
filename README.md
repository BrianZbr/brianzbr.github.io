# Brian Zbriger's Personal Website

A modern, responsive personal website built with [Hugo](https://gohugo.io/) static site generator and hosted on GitHub Pages. This site showcases Brian Zbriger's professional profile, projects, and technical skills.

## 🌐 Live Site

- **URL**: [https://www.brianz.page](https://www.brianz.page)
- **Domain**: Custom domain configured via CNAME record

## 🚀 Technology Stack

- **Static Site Generator**: Hugo v0.123+ (latest)
- **Theme**: Custom `my-sustain` theme (based on hugo-sustain)
- **Hosting**: GitHub Pages
- **CI/CD**: GitHub Actions for automated deployment
- **Analytics**: GoatCounter for privacy-friendly tracking
- **Deployment**: Automatic on push to main branch

## 📁 Project Structure

```
brianzbr.github.io/
├── .github/
│   └── workflows/
│       ├── gh-pages.yml          # Main deployment workflow
│       └── preview.yml           # Preview deployment for PRs
├── content/
│   └── _index.md                 # Homepage content
├── layouts/
│   └── partials/
│       └── custom-head.html      # Custom analytics partial
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
│   └── my-sustain/               # Custom theme (active)
├── config.toml                   # Hugo configuration
├── .gitignore                    # Git ignore rules
└── .nojekyll                     # Disable Jekyll processing
```

## ⚙️ Configuration

### Hugo Configuration (`config.toml`)

- **Base URL**: `https://www.brianz.page`
- **Language**: English (US)
- **Title**: Brian Zbriger
- **Theme**: my-sustain (custom theme)
- **Author**: Brian Zbriger
- **Avatar**: `/img/headshot.jpg`
- **Analytics**: GoatCounter configuration-based

### Social Links

- **GitHub**: [BrianZbr](https://github.com/BrianZbr/)
- **Email**: mail@brianz.page
- **LinkedIn**: [brian-zbriger-70a31561](https://linkedin.com/in/brian-zbriger-70a31561)

### Navigation Menu

The site includes links to:
- GitHub Profile
- LinkedIn Profile
- Resume (PDF)
- Email Contact

## 🎨 Theme Customization

This site uses a custom `my-sustain` theme based on hugo-sustain:

### Features
- **Responsive Design**: Mobile-friendly layout
- **Syntax Highlighting**: Code highlighting with highlight.js
- **Social Integration**: Links to professional profiles
- **Custom Styling**: Modified CSS for personal branding
- **Bootstrap Integration**: Responsive grid system

### Theme Structure
- **Active Theme**: `themes/my-sustain/` (standalone custom theme)
- **Custom Partials**: `layouts/partials/custom-head.html` for analytics
- **Configuration-Based**: Analytics managed via `config.toml`
- **No Submodules**: Simplified setup without Git complexity

## 🔄 Deployment Process

### GitHub Actions Workflows

#### Main Deployment (`gh-pages.yml`)
- **Trigger**: Push to `main` branch
- **Build**: Hugo builds site with minification
- **Deploy**: Automatic deployment to GitHub Pages

#### Preview Deployment (`preview.yml`)
- **Trigger**: Pull requests to `main`
- **Build**: Tests build process
- **Deploy**: Optional preview deployment

### Deployment Configuration

- **Environment**: Ubuntu Latest
- **Hugo Version**: Latest
- **Publish Directory**: `./public`
- **Minification**: Enabled
- **Submodules**: Not used (simplified setup)

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
- **Analytics**: GoatCounter configuration-based tracking

## 🛠️ Local Development

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/installing/) (v0.123+)
- Git

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/BrianZbr/brianzbr.github.io.git
   cd brianzbr.github.io
   ```

2. Start development server:
   ```bash
   hugo serve --bind 0.0.0.0 --port 1313
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

### Analytics & Tracking
- GoatCounter integration for privacy-friendly analytics
- Configuration-based tracking setup
- No cookies, GDPR compliant

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
4. **Custom Partials**: Add/modify files in `layouts/partials/`

### Analytics Configuration

1. **Update GoatCounter**: Modify `config.toml`:
   ```toml
   [params.analytics]
     goatcounter = "your-subdomain.goatcounter.com"
   ```
2. **Add New Analytics**: Extend `layouts/partials/custom-head.html`
3. **Disable Tracking**: Set analytics value to empty string

### Updating Resume

1. Replace `static/resume.pdf` with new version
2. Update version-specific files if needed
3. Test download links

## 📈 Performance Optimization

- **Minification**: Enabled for HTML, CSS, and JS
- **Image Optimization**: Compressed profile images
- **CDN Delivery**: GitHub Pages CDN
- **Caching**: Proper cache headers via GitHub Pages
- **Lightweight Analytics**: GoatCounter minimal script

## 🔒 Security Considerations

- **No Server-Side Processing**: Static site only
- **HTTPS Enforced**: Via GitHub Pages
- **Privacy-Friendly Analytics**: GoatCounter (no cookies)
- **Minimal Dependencies**: Limited external scripts
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
**Theme**: my-sustain (custom Hugo theme)  
**Analytics**: GoatCounter (privacy-friendly)  
**Deployment**: GitHub Pages with CI/CD

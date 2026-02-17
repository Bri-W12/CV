# Brianna L. Watts - Academic Website

This repository contains the source code for my academic website, built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

## Website

🌐 Visit the live site: [https://bri-w12.github.io/CV](https://bri-w12.github.io/CV)

## Contents

- **CV**: Complete curriculum vitae with education, research experience, publications, and honors
- **Blog**: Updates about research, conferences, and graduate school experiences

## Technology Stack

- **Framework**: Quarto (scientific and technical publishing system)
- **Hosting**: GitHub Pages
- **Deployment**: Automated via GitHub Actions
- **Theme**: Cosmo

## Local Development

### Prerequisites

Install [Quarto](https://quarto.org/docs/get-started/) for your operating system.

### Preview Locally

```bash
quarto preview
```

This will start a local server and open the site in your browser. Changes will auto-refresh.

### Build Site

```bash
quarto render
```

The rendered site will be in the `_site/` directory.

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch via GitHub Actions.

### Required GitHub Settings

1. **Actions Permissions**: Settings → Actions → General → "Read and write permissions"
2. **Pages Source**: Settings → Pages → Deploy from branch: `gh-pages` / `root`

## Adding Blog Posts

Create a new post by adding a folder in `posts/` with the format `YYYY-MM-DD-post-title/`:

```bash
mkdir posts/2026-02-17-my-new-post
```

Then create `index.qmd` inside with frontmatter:

```yaml
---
title: "My Post Title"
author: "Brianna L. Watts"
date: "2026-02-17"
categories: [research, category2]
description: "A brief description"
---

Your content here...
```

## Project Structure

```
.
├── _quarto.yml                 # Site configuration
├── index.qmd                   # CV homepage
├── blog.qmd                    # Blog listing page
├── posts/                      # Blog posts
│   ├── _metadata.yml
│   └── YYYY-MM-DD-title/
│       └── index.qmd
├── .github/workflows/
│   └── publish.yml             # Deployment workflow
├── styles.css                  # Custom CSS
└── Meredith_lab_logo.png       # Lab logo
```

## License

© 2026 Brianna L. Watts. All rights reserved.

## Contact

- Email: blw5699@psu.edu
- GitHub: [@Bri-W12](https://github.com/Bri-W12)

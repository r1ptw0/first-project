# My First MkDocs Site

A sample MkDocs documentation site with Material theme, demonstrating best practices for documentation and automated deployment to GitHub Pages.

## Overview

This project is a "Hello World" for MkDocs and GitHub Pages, showcasing:

- Modern documentation site with Material for MkDocs theme
- Automated deployment via GitHub Actions
- Multi-level navigation structure
- Code highlighting and syntax support
- Light/dark theme toggle
- Built-in search functionality
- Responsive design

## Prerequisites

- Python 3.7 or higher
- pip (Python package installer)
- Git

## Local Development

### 1. Clone the Repository

```bash
git clone https://github.com/r1ptw0/first-project.git
cd first-project
```

### 2. Install Dependencies

```bash
pip install mkdocs mkdocs-material
```

Or use a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install mkdocs mkdocs-material
```

### 3. Serve Locally

```bash
mkdocs serve
```

Open your browser to [http://127.0.0.1:8000](http://127.0.0.1:8000)

The site will automatically reload when you make changes.

### 4. Build the Site

```bash
mkdocs build
```

This generates static HTML files in the `site/` directory.

## Deployment to GitHub Pages

### Automatic Deployment

This repository is configured with GitHub Actions for automatic deployment:

1. Push changes to the `main` branch
2. GitHub Actions will automatically build and deploy to GitHub Pages
3. Your site will be available at `https://r1ptw0.github.io/first-project`

### First-Time Setup

1. Go to your repository settings on GitHub
2. Navigate to **Pages** (under "Code and automation")
3. Under "Source", select **Deploy from a branch**
4. Select the `gh-pages` branch and `/ (root)` folder
5. Click **Save**

The GitHub Actions workflow will create the `gh-pages` branch automatically on the first push.

### Manual Deployment

You can also deploy manually:

```bash
mkdocs gh-deploy
```

## Project Structure

```
first-project/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow
├── docs/
│   ├── index.md               # Home page
│   ├── getting-started.md     # Getting started guide
│   ├── user-guide/
│   │   ├── installation.md    # Installation instructions
│   │   └── configuration.md   # Configuration guide
│   └── about.md               # About page
├── mkdocs.yml                 # MkDocs configuration
├── .gitignore                 # Git ignore file
└── README.md                  # This file
```

## Customization

### Update Site Information

Edit `mkdocs.yml` to customize:

- Site name and description
- Repository links (replace `r1ptw0/first-project`)
- Theme colors
- Navigation structure

### Add New Pages

1. Create a new Markdown file in the `docs/` directory
2. Add it to the navigation in `mkdocs.yml`

### Change Theme

The Material theme offers extensive customization options. See the [Material for MkDocs documentation](https://squidfunk.github.io/mkdocs-material/) for details.

## Resources

- [MkDocs Documentation](https://www.mkdocs.org/)
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## License

This is a sample project provided as-is for learning and template purposes.

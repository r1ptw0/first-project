# Getting Started

Welcome! This guide will help you get started with this MkDocs site.

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7 or higher
- pip (Python package installer)

## Installation

1. Clone this repository:

```bash
git clone https://github.com/yourusername/first-project.git
cd first-project
```

2. Install MkDocs and the Material theme:

```bash
pip install mkdocs mkdocs-material
```

## Building the Site

To build the documentation site locally:

```bash
mkdocs build
```

This creates a `site` directory with the static HTML files.

## Local Development

To preview your documentation as you write:

```bash
mkdocs serve
```

Then open your browser to [http://127.0.0.1:8000](http://127.0.0.1:8000)

The site will automatically reload when you save changes to your Markdown files.

## Deploying to GitHub Pages

This project is configured with GitHub Actions to automatically deploy to GitHub Pages whenever you push to the `main` branch.

!!! tip "Manual Deployment"
    You can also deploy manually using: `mkdocs gh-deploy`

## Project Structure

```
first-project/
├── docs/
│   ├── index.md
│   ├── getting-started.md
│   ├── user-guide/
│   │   ├── installation.md
│   │   └── configuration.md
│   └── about.md
├── mkdocs.yml
└── README.md
```

## Next Steps

Now that you're set up, explore the [User Guide](user-guide/installation.md) to learn more!

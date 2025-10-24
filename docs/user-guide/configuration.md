# Configuration

Learn how to customize your MkDocs site.

## The mkdocs.yml File

The `mkdocs.yml` file is the heart of your MkDocs site. It controls:

- Site metadata
- Theme settings
- Navigation structure
- Markdown extensions
- And more!

## Basic Configuration

### Site Information

```yaml
site_name: My Documentation
site_description: A brief description
site_author: Your Name
site_url: https://example.com
```

### Repository Links

Link your documentation to its GitHub repository:

```yaml
repo_name: username/repository
repo_url: https://github.com/username/repository
```

## Theme Customization

This site uses the Material for MkDocs theme with several customizations.

### Color Palette

The theme supports both light and dark modes:

```yaml
theme:
  palette:
    - scheme: default
      primary: indigo
      accent: indigo
    - scheme: slate
      primary: indigo
      accent: indigo
```

Available colors include: `red`, `pink`, `purple`, `indigo`, `blue`, `cyan`, `teal`, `green`, `lime`, `yellow`, `amber`, `orange`, and `deep orange`.

### Features

Enable additional features:

```yaml
theme:
  features:
    - navigation.tabs        # Top-level tabs
    - navigation.sections    # Expandable sections
    - navigation.top        # Back-to-top button
    - search.suggest        # Search suggestions
    - search.highlight      # Highlight search terms
    - content.code.copy     # Copy button for code blocks
```

## Markdown Extensions

This site uses several Markdown extensions for enhanced functionality:

- **Code Highlighting**: `pymdownx.highlight`
- **Admonitions**: Call-out boxes for notes, warnings, etc.
- **Tabbed Content**: `pymdownx.tabbed`
- **Details/Summary**: Collapsible sections

Example admonition:

!!! warning "Important"
    Always backup your configuration before making changes!

## Navigation Structure

Define your site's navigation in `mkdocs.yml`:

```yaml
nav:
  - Home: index.md
  - Getting Started: getting-started.md
  - User Guide:
      - Installation: user-guide/installation.md
      - Configuration: user-guide/configuration.md
  - About: about.md
```

## Further Reading

- [MkDocs Configuration Reference](https://www.mkdocs.org/user-guide/configuration/)
- [Material for MkDocs Setup](https://squidfunk.github.io/mkdocs-material/setup/)
- [Markdown Extensions Guide](https://squidfunk.github.io/mkdocs-material/reference/)

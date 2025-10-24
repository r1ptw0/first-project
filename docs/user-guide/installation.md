# Installation

This page provides detailed installation instructions.

## System Requirements

- **Operating System**: Windows, macOS, or Linux
- **Python**: Version 3.7 or higher
- **pip**: Latest version recommended

## Step-by-Step Installation

### 1. Install Python

=== "Windows"

    Download Python from [python.org](https://www.python.org/downloads/) and run the installer.

    Make sure to check "Add Python to PATH" during installation.

=== "macOS"

    Using Homebrew:
    ```bash
    brew install python
    ```

=== "Linux"

    ```bash
    sudo apt-get update
    sudo apt-get install python3 python3-pip
    ```

### 2. Verify Installation

Check your Python installation:

```bash
python --version
pip --version
```

### 3. Install MkDocs

Install MkDocs and the Material theme:

```bash
pip install mkdocs mkdocs-material
```

### 4. Verify MkDocs Installation

```bash
mkdocs --version
```

You should see output indicating the version of MkDocs installed.

!!! success "Installation Complete"
    You're all set! Head over to the [Configuration](configuration.md) guide to customize your site.

## Troubleshooting

### Permission Errors

If you encounter permission errors on Linux/macOS, try:

```bash
pip install --user mkdocs mkdocs-material
```

### Command Not Found

If `mkdocs` command is not found, add Python's user bin directory to your PATH.

For more help, visit the [MkDocs documentation](https://www.mkdocs.org/).

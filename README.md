<p align="center">
  <img src="./icon.png" alt="Metupy Logo" width="128" height="128">
</p>

<h1 align="center">Metupy IntelliSense</h1>

<p align="center">
  <strong>Official IntelliSense & Syntax Highlighting for Metupy (.pym) file format</strong><br>
  <em>Project by PalembangPy Community</em>
</p>

<p align="center">
  <img src="https://img.shields.io/pypi/v/metupy-core?style=for-the-badge&logo=python&logoColor=white" alt="PyPI Version">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License">
</p>

---

## Description

Metupy IntelliSense is a Visual Studio Code extension that provides full syntax highlighting, code snippets, and language support for .pym files — the native content format of Metupy Static Site Generator.

## Features

- Syntax Highlighting for .pym file format
- Frontmatter key-value highlighting
- Template variables `{{ }}` and logic tags {% %}
- Comment support `{# #}`
- Embedded Markdown and Python syntax
- Auto-closing pairs and smart indentation
- Custom file icon for `.pym` files

## Installation

### Install from VS Code Marketplace
Open Command Palette (Ctrl+Shift+P) and run:

```text
ext install PalembangPyCommunity.metupy-intellisense
```

### Manual Installation
1. Download the .vsix file from Releases page
2. Open VS Code → Extensions → Install from VSIX...
3. Select the downloaded file
4. Restart VS Code

## Install Metupy from PyPI

### Install Metupy
Run this command in your terminal:

```bash
pip install metupy
```

### Verify Installation

```bash
metupy --version
```

## Quick Start

### Create a New Project

```bash
metupy init my-site && cd my-site
```

### Create Content File
Create a file named `index.pym` inside content folder:

```markdown
title: Welcome to Metupy
author: Your Name
date: 2026-08-28
---

# Welcome to Metupy

This is my first Metupy site!
```

### Start Development Server

```bash
metupy dev
```

### Build for Production

```bash
metupy build
```

## File Format

`.pym` file uses simple structure:

```markdown
key: value
another_key: another value
---

Your content here with {{ variables }} and {% logic %}
```

## Syntax Reference

- Variables: `{{ variable_name }}`
- Logic: `{% for item in list %} ... {% endfor %}`
- Condition: `{% if condition %} ... {% endif %}`
- Comment: `{# This is a comment #}`
- Frontmatter: `key: value` above `---` separator

## About Metupy

Metupy is a fast, modern static site generator built with Python. It supports .pym, .md, .rst, and .py file formats. No Node.js required.

## License

MIT License — PalembangPy Community

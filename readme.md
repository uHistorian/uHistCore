<div align="center">

# Welcome to uHistorian Core 

**Industrial IoT data acquisition, visualization and event management**

[![Docs build](https://github.com/uHistorian/uHistCore/actions/workflows/docs.yml/badge.svg)](https://github.com/uHistorian/uHistCore/actions/workflows/docs.yml)
[![Documentation](https://img.shields.io/badge/docs-uhistorian.github.io-blue)](https://uhistorian.github.io/uHistCore/)
[![Languages](https://img.shields.io/badge/docs-English%20%7C%20Fran%C3%A7ais-informational)](https://uhistorian.github.io/uHistCore/en/)

[📖 **Read the documentation**](https://uhistorian.github.io/uHistCore/en/) ·
[📖 Lire la documentation](https://uhistorian.github.io/uHistCore/) ·
[✉️ Contact](mailto:info@uhistorian.com)

</div>

---

## About

**uHistorian** is an IIoT platform that collects data from sensors, modules and industrial interfaces,
archives it, and makes it available through web and mobile views, notifications and standard protocols.

This repository hosts the **public documentation** of uHistorian: installation and user manuals, written in
English and French.

## Documentation

The site is bilingual. Use the language switcher in the header to change between English and French.

| Section | What you will find |
|---------|--------------------|
| **Configuration** | Modules, tags, tag groups, messages, notifications and event management, general settings, security |
| **Interfaces** | OPC-UA client and server, LiDAR (RS-485) |
| **Visualization** | Dataview (web and iPhone), EventView |
| **Maintenance** | Changing passwords and routine administration |

👉 Start here: **<https://uhistorian.github.io/uHistCore/en/>**

## Repository layout

```text
.
├── docs/                   Markdown pages and screenshots
│   ├── index.md            Home page (French)
│   ├── index.en.md         Home page (English)
│   ├── assets/             Screenshots used by the French pages
│   └── assets-en/          Screenshots used by the English pages
├── mkdocs.yml              Site configuration and navigation
└── .github/workflows/      Build and publishing (GitHub Actions)
```

Naming convention: `page.md` is the French page and `page.en.md` is its English translation.

## Build the documentation locally

Requirements: Python 3.9 or later (Python 3.7 works with the older versions shown below) and Git.

```bash
git clone https://github.com/uHistorian/uHistCore.git
cd uHistCore

python -m venv .venv
# Windows:      .venv\Scripts\activate
# Linux/macOS:  source .venv/bin/activate

pip install "mkdocs<2" "mkdocs-material==9.7.6" "mkdocs-static-i18n==1.3.1"
mkdocs serve
```

Open <http://127.0.0.1:8000>. The site reloads each time you save a file.

> **Python 3.7:** use `mkdocs-material==9.2.7` and `mkdocs-static-i18n==1.2.0`.

To check for broken links and missing images, as the CI does:

```bash
mkdocs build --strict
```

## Contributing

Corrections and suggestions are welcome.

1. Fork the repository and create a branch.
2. Edit or add pages under `docs/`. Keep the French and English versions in sync, and put screenshots in the matching
   `assets/` or `assets-en/` folder.
3. Run `mkdocs build --strict`.
4. Open a pull request.

You can also report a problem by opening an **issue**, or write to <info@uhistorian.com>.

> **Please never commit** passwords, license keys, tokens, public IP addresses or personal data, including in
> screenshots.

## Contact

**uHistorian** · <info@uhistorian.com> · <https://uhistorian.github.io/uHistCore/en/>

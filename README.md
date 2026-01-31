# Slow Erasure

![Slow Erasure](docs/images/cover.jpg)

**Slow Erasure: Identity, Agency & Episteme in Settler-Colonial Genocide by Attrition**

A PhD dissertation by [Bram J. De Smet](https://orcid.org/0000-0002-4364-6827), Tampere University, Finland.

## About

This repository contains the source files for the online version of the dissertation, built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Read Online

The book is available at: https://slowerasure.phd

## PDF Version

The official PDF is available via Tampere University: [https://urn.fi/URN:ISBN:978-952-03-4306-4](https://urn.fi/URN:ISBN:978-952-03-4306-4)

## Citation

De Smet, Bram J. 2025. *Slow Erasure: Identity, Agency & Episteme in Settler Colonial-Genocide by Attrition*. TAPRI Studies in Peace and Conflict Research 113. Tampere: Tampere Peace Research Institute.

## Setup

### Prerequisites

- Python 3.12+
- Pandoc (`sudo pacman -S pandoc` on Arch, `sudo apt install pandoc` on Debian/Ubuntu)

### Install dependencies

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Local development

```bash
mkdocs serve
```

Visit http://127.0.0.1:8000

### Build for production

```bash
mkdocs build --strict
```

Output is generated in the `site/` directory.

## Deployment

Deployment happens automatically via GitHub Actions when pushing to the `main` branch. The workflow builds the site with MkDocs and deploys via rsync to a remote server.

## Project structure

```
docs/               Markdown content (chapters, front matter, bibliography)
docs/images/        Images referenced in the text
docs/stylesheets/   Custom CSS
overrides/          MkDocs Material theme overrides (Matomo analytics)
mkdocs.yml          MkDocs configuration and navigation
references.bib      BibTeX bibliography (365 entries)
chicago-author-date.csl   Citation style
requirements.txt    Python dependencies
```

## License

- **Text and original images:** © 2025 Bram J. De Smet — licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Third-party images and materials:** Subject to their own license terms; credited individually where used

## Contact

For inquiries: [bram@academic.coffee](mailto:bram@academic.coffee)

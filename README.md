# 🛠️ AI Compute Broker Docs – Setup Guide

This guide outlines how to install, run, lint, and export the documentation site using [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

---

## ✅ Installation

Clone the repository:

```bash
git clone https://github.com/your-org/ai-compute-broker-docs.git
cd ai-compute-broker-docs
```

Optional: Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

Install required dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Docs

To build the static site:

```bash
mkdocs build
```

To launch a local dev server with hot reload:

```bash
mkdocs serve
```

Then open [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.

---

## 🖨 Exporting to PDF

Each page includes a print icon in the top-right corner.  
Click it to export that page as a PDF via your browser's print dialog.

---

## 🧼 Markdown Linting (Optional)

Linting rules are defined in `pymarkdown.json`.

Rules defined in `pymarkdown.json`

To scan a specific file:

```bash
pymarkdown --config pymarkdown.json scan docs/<filename>.md
```

> Note: `pymarkdown` does not auto-fix files — it only reports issues.

Fix them:
```bash
pymarkdown --config pymarkdown.json fix docs/<filename>.md
```

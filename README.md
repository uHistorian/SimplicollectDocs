# Simplicollect – Manuals (legacy product)

Installation and user manuals for **Simplicollect**, a legacy product. Bilingual (French / English) MkDocs Material site.
The English screenshots (`docs/assets-en/`) were retouched automatically and are draft quality.

## View the site locally

```bash
pip install "mkdocs<2" "mkdocs-material==9.7.6" "mkdocs-static-i18n==1.3.1"
mkdocs serve
```

Open <http://127.0.0.1:8000>. Pages: `page.md` = French, `page.en.md` = English.
`mkdocs build --strict` runs on every push (`.github/workflows/docs-check.yml`).
To publish with GitHub Pages, see `docs-publish.yml.example`.

## Rules

This repository is public: never commit passwords, license keys, public IP addresses, host names or personal data
(check screenshots too).

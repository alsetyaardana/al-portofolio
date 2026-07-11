# Alindra Setya Ardana - Personal Professional Website

Static personal website for Alindra Setya Ardana, a Presales Engineer and Technology Builder.

The website presents:
- professional identity;
- Presales experience;
- technology domains;
- selected work and experiments;
- personal notes;
- connection to Alink Tech.

## Purpose

This repository powers the personal professional website at `https://www.alindra.my.id/`. The site is designed to introduce Alindra's Presales Engineering work, document selected projects and experiments, and provide clear paths for professional contact.

Alink Tech is referenced as a separate independent commercial initiative, not as the primary identity of this website.

## Architecture

The website is intentionally lightweight and static:
- semantic HTML in `index.html`;
- local CSS in `assets/css/styles.css`;
- minimal vanilla JavaScript in `assets/js/main.js`;
- static images in `assets/images/`;
- GitHub Pages-compatible paths.

No framework, build system, backend, database, or runtime dependency is required.

## Directory Structure

```text
/
+-- index.html
+-- CNAME
+-- robots.txt
+-- sitemap.xml
+-- README.md
+-- favicon.svg
+-- assets/
    +-- css/
    |   +-- styles.css
    +-- js/
    |   +-- main.js
    +-- images/
        +-- alindra-semi-formal.png
        +-- og-cover.png
        +-- work-automation-finance.png
        +-- work-laut-jaya.png
        +-- work-network-hospital.png
        +-- work-paralife-ai.png
        +-- work-rfid-linen-visibility.png
        +-- work-rfid-warehouse.png
```

## Local Preview

Run a simple static server from the repository root:

```bash
python -m http.server 8000
```

Open:

```text
http://127.0.0.1:8000/
```

## Deployment

The site is suitable for GitHub Pages. The canonical domain is configured through `CNAME`:

```text
www.alindra.my.id
```

Do not remove or overwrite `CNAME` unless the production hostname changes.

## SEO Files

The repository includes:
- `robots.txt` with the canonical sitemap location;
- `sitemap.xml` containing the canonical homepage URL;
- Open Graph and Twitter metadata in `index.html`;
- JSON-LD structured data using `ProfilePage` and `Person`.

## Editing Guidelines

- Keep the site static and GitHub Pages-compatible.
- Use Indonesian as the primary language.
- Keep the primary positioning as `Presales Engineer & Technology Builder`.
- Use first-person writing.
- Do not add unsupported claims, fake metrics, client names, certifications, or private employer details.
- Keep Alink Tech concise as a separate independent initiative.
- Keep external links descriptive and use `rel="noopener noreferrer"` when opening a new tab.

## Privacy

A detailed CV is not publicly hosted from the current website. CV sharing should happen directly by request.

Removing a file from the current branch does not remove it from previous Git commits. Git history cleanup requires a separate owner-approved destructive operation.

## Verification Commands

```bash
git status --short
git diff --check
git diff --stat
grep -RniE "<removed-public-cv-and-outdated-marketing-terms>" . --exclude-dir=.git
python -m http.server 8000
```

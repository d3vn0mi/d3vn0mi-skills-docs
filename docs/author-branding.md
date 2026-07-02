# author-branding
> Every project Claude scaffolds comes out branded as you — one modern README, your name across the repo, consistently. GitHub-first.

## Description
A branding standard for the projects you build with an AI assistant. Set your author identity once and this skill applies it everywhere: a **modern, rich README** (badges, a centered hero, a table of contents, collapsible sections, an Author/Credits block), your author info across the repo's manifests (`LICENSE` copyright, `package.json`, `pyproject.toml`, `Cargo.toml`, `composer.json`, `CITATION.cff`, `FUNDING.yml`), a consistent GitHub file set (`.gitignore`, `.github/` templates, `CONTRIBUTING`), and AI-assistant attribution stripped from your own files. The author is a parameter — d3vn0mi is the built-in default, swap in your own. It brands **your** work; it never touches third-party attribution.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your author identity and produces a modern README, author-applied project files, and a consistent GitHub repo scaffold. **Brands YOUR own output as your authorship and strips AI-assistant attribution from your files — it never removes third-party copyright, OSS `LICENSE`/`NOTICE`, or upstream credits, and it is not legal advice on licensing.**

## Keywords
author branding, README template, modern README, project scaffolding, GitHub repo template, authorship, package.json author, pyproject authors, LICENSE copyright, badges, shields.io, CITATION.cff, FUNDING.yml, repo consistency, personal brand, developer branding, README generator

## Sample input
> "I'm shipping a CLI tool called `swiftpack` to GitHub, author d3vn0mi, MIT. Give me a modern README and put my name on everything."

## Sample output
*(Illustrative shape.)*
- **Modern README** — a centered hero (`<div align="center">` + tagline), a live badge row (`![License](https://img.shields.io/github/license/d3vn0mi/swiftpack)` + version/stars/build), a table of contents, Features / Install / Usage / Examples (in `<details>`), Roadmap, Contributing, License, and an **Author / Credits** block: `Built by [d3vn0mi](https://github.com/d3vn0mi)`.
- **Author across manifests** — `LICENSE`: `Copyright (c) 2026 d3vn0mi`; `package.json`: `"author": "d3vn0mi"`; `pyproject.toml`: `[project] authors = [{ name = "d3vn0mi" }]`; `CITATION.cff` + `FUNDING.yml` filled.
- **Clean attribution** — "🤖 Generated with Claude" and any `Co-Authored-By` AI trailers removed from *your* files.
- **Consistent repo** — `.gitignore`, `.github/` issue + PR templates, `CONTRIBUTING.md`, and a reusable identity profile so your *next* project looks the same.

## Known limitations
- **Brands your work only** — it will not remove or alter third-party copyright headers, upstream author names, or OSS `LICENSE`/`NOTICE`/`AUTHORS` files (those are legally required and stay), and it won't rebrand someone else's project as yours.
- **You are the author of record** — the identity you set is the real author; it won't impersonate a different real person, and you're accountable for the code.
- **Not legal advice** — for licensing/copyleft obligations it points you to choosealicense.com / tldrlegal.com; verify for your project.
- **Advisory only** — it produces the files; you commit them. GitHub-first (other package registries can follow). Not a git/GitHub API tool, not a license chooser, not visual brand identity.

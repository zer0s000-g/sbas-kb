# SBAS Knowledge Base

Institutional-grade SBAS knowledge base published with [Quartz v4](https://quartz.jzhao.xyz/) and GitHub Pages.

Live site:

https://zer0s000-g.github.io/sbas-kb/

Repository:

https://github.com/zer0s000-g/sbas-kb

## What this repository contains

This repository is a Quartz project whose publishable Obsidian vault lives in `content/`.

Key directories:

- `content/` — the Obsidian/Quartz knowledge base Markdown files.
- `content/Concepts/` — atomic SBAS concept notes.
- `content/Sources/` — source notes, provenance notes, and source backlogs.
- `content/Standards-Regulation/` — standards, claim-routing, and validation matrices.
- `content/MOCs/` — Maps of Content used as navigation hubs.
- `content/Syntheses/` — bounded comparison and synthesis notes.
- `content/Logs/` — dated research and maintenance logs.
- `.github/workflows/deploy.yml` — GitHub Pages deployment workflow.
- `quartz.config.ts` — Quartz site configuration.

## Knowledge-base rules

This vault is maintained as a source-routed aviation knowledge base, not as a casual notes folder.

Core rules:

1. Do not duplicate knowledge across notes.
   - Each concept must have one clear owner.
   - Related notes should link to the owner rather than copy its explanation.

2. Do not publish unsupported operational claims.
   - Service-provider evidence does not automatically prove procedure availability, aircraft eligibility, operator authorization, or regulator approval.
   - Operational claims must route through `content/Standards-Regulation/SBAS Operational Validation Dashboard.md`.

3. Keep source provenance visible.
   - Source notes belong in `content/Sources/`.
   - Use original/authoritative public sources where possible.
   - If a claim is only a routing scaffold or source-context signal, label it that way.

4. Keep local/private data out of published content.
   - Do not publish local filesystem paths, backup paths, credentials, API keys, tokens, or private workspace names.
   - Use neutral wording such as “private source collection” or “local backup” if needed.

5. Keep Markdown Quartz-safe.
   - Use valid YAML frontmatter fences: `---`.
   - Keep tables structurally valid.
   - Avoid placeholder wikilinks unless the target note exists.

## Requirements

- Node.js 22 or newer.
- npm 10.9.2 or newer.
- Git.
- GitHub Pages configured to use GitHub Actions.

Check local versions:

```bash
node --version
npm --version
git --version
```

Install dependencies:

```bash
npm ci
```

## How publishing works

The site is published by GitHub Actions.

On every push to `main`:

1. GitHub checks out the repository.
2. Node.js 22 is installed.
3. Dependencies are installed with `npm ci`.
4. Quartz builds the static site with `npx quartz build`.
5. The generated `public/` artifact is deployed to GitHub Pages.

Workflow file:

```text
.github/workflows/deploy.yml
```

Quartz config:

```text
quartz.config.ts
```

Current production base URL is configured as:

```ts
baseUrl: "zer0s000-g.github.io/sbas-kb"
```

## Local preview

From the repository root:

```bash
npm ci
npx quartz build --serve
```

Then open:

```text
http://localhost:8080
```

If you only want to build without serving:

```bash
npx quartz build
```

## How to update the knowledge base

Use this workflow for normal content changes.

### 1. Start from a clean main branch

```bash
git checkout main
git pull origin main
git status --short --branch
```

Do not start a new edit cycle if the working tree is dirty unless you understand the existing changes.

### 2. Edit Markdown under `content/`

Examples:

```text
content/Concepts/...
content/Sources/...
content/Standards-Regulation/...
content/MOCs/...
content/Syntheses/...
content/Logs/...
```

Recommended note pattern:

```markdown
---
title: Clear Note Title
description: One-sentence scope statement.
tags:
  - sbas
  - source-routing
status: draft
verification_status: source-scaffold-linked
---

# Clear Note Title

## Purpose

State what this note owns.

## Non-overlap boundary

State what this note does not own and link to the correct owner notes.

## Source anchors

- [[Source - Example]]

## See also

- [[Related Concept]]
```

### 3. Enforce non-overlap before adding claims

Before writing a new explanation, search for the existing owner note.

Examples:

```bash
rg "correction|integrity|protection level|alert limit" content/Concepts content/Standards-Regulation
rg "LPV|LNAV|service volume|coverage" content/
```

If an owner note already exists, link to it instead of duplicating the explanation.

Important routing notes:

- `content/Standards-Regulation/SBAS Core Claim Routing.md`
- `content/Standards-Regulation/SBAS Standards Source Matrix.md`
- `content/Standards-Regulation/SBAS Operational Validation Dashboard.md`
- `content/Standards-Regulation/SBAS Standards to Operations Evidence Ladder.md`

### 4. Add or update source notes first

For new factual claims, create or update the source note before changing downstream concept pages.

Source-note location:

```text
content/Sources/Source - [Name].md
```

A source note should state:

- source identity
- source type
- what the source can support
- what the source must not be used to support
- downstream notes affected
- open provenance questions

### 5. Add a research log for significant changes

For substantial changes, add a dated log:

```text
content/Logs/ResearchLog-YYYY-MM-DD-Short-Topic.md
```

The log should include:

- scope of work
- files created
- files updated
- source-boundary decisions
- claims deliberately not made
- QA/publish status

### 6. Format changed files

For a small content update, run Prettier on changed Markdown files:

```bash
npx prettier --write "content/path/to/changed-file.md"
```

For a broad vault-wide formatting task only, run:

```bash
npm run format
```

Avoid mass-formatting unrelated files during a focused source-hardening change unless that is the task.

### 7. Run quality checks

Minimum local checks before committing:

```bash
npm run check
npx quartz build
python3 ~/.hermes/skills/note-taking/obsidian-knowledge-management/scripts/obsidian_wikilink_audit.py content
python3 ~/.hermes/skills/productivity/obsidian-quartz-publish/scripts/quartz_publication_audit.py .
python3 ~/.hermes/skills/productivity/obsidian-quartz-publish/scripts/markdown_table_audit.py content
git diff --check
```

If those helper scripts are not available, at minimum run:

```bash
npm run check
npx quartz build
git diff --check
rg "/Users/|/home/|file://|quartz-backups|api[_-]?key|token|secret" content public
```

The privacy scan should return no real secrets or local paths. If it returns a false positive, inspect it manually before publishing.

### 8. Review the diff

```bash
git status --short
git diff --stat
git diff -- README.md content/ quartz.config.ts .github/workflows/deploy.yml
```

Confirm the diff contains only intentional changes.

### 9. Commit and push

```bash
git add -A
git commit -m "docs: describe the change"
git push origin main
```

Pushing to `main` triggers the Quartz deploy workflow.

### 10. Verify deployment

Check the pushed SHA:

```bash
git rev-parse HEAD
git ls-remote origin refs/heads/main
```

Check GitHub Actions:

https://github.com/zer0s000-g/sbas-kb/actions

If `gh` is unavailable, use the GitHub API:

```bash
python3 - <<'PY'
import json, urllib.request
repo = "zer0s000-g/sbas-kb"
url = f"https://api.github.com/repos/{repo}/actions/runs?per_page=10"
req = urllib.request.Request(url, headers={"Accept": "application/vnd.github+json", "User-Agent": "sbas-kb"})
with urllib.request.urlopen(req, timeout=30) as r:
    data = json.load(r)
for run in data.get("workflow_runs", [])[:10]:
    print(run["id"], run["head_branch"], run["head_sha"][:7], run["status"], run.get("conclusion"), run["html_url"])
PY
```

Then verify the live site and search index:

```bash
python3 - <<'PY'
import urllib.request
urls = [
    "https://zer0s000-g.github.io/sbas-kb/",
    "https://zer0s000-g.github.io/sbas-kb/static/contentIndex.json",
]
for url in urls:
    req = urllib.request.Request(url, headers={"User-Agent": "sbas-kb", "Cache-Control": "no-cache"})
    with urllib.request.urlopen(req, timeout=30) as r:
        body = r.read(5000).decode(errors="replace")
    print(url, "OK", len(body))
PY
```

For newly added pages, verify the exact live route as well. Quartz usually converts spaces to hyphens. For example:

```text
content/Concepts/SBAS Service Performance Concepts.md
```

becomes:

```text
https://zer0s000-g.github.io/sbas-kb/Concepts/SBAS-Service-Performance-Concepts
```

## Publishing a different Obsidian vault with Quartz

If you want to reuse this repository pattern for another vault:

1. Create or clone a Quartz project.
2. Put the vault Markdown files under `content/`.
3. Ensure there is a root `content/index.md`.
4. Set `pageTitle` and `baseUrl` in `quartz.config.ts`.
5. Keep `.github/workflows/deploy.yml` configured for `main`.
6. Push to GitHub.
7. In GitHub repository settings, set Pages source to GitHub Actions.
8. Verify the deployed site and `static/contentIndex.json`.

Important CI/CD rule:

- A local symlinked `content/` directory can work for local preview.
- For GitHub Actions deployment, `content/` must be real files committed into the repository, not a symlink to a local vault path.

## Common problems

### GitHub Actions succeeds but the page looks stale

Wait a short time and re-check the exact page plus `static/contentIndex.json`. GitHub Pages propagation can lag.

### A new page returns 404

Check the emitted route in `public/` after local build, or verify the slug pattern. Quartz normalizes spaces to hyphens and may normalize punctuation.

### Raw table pipes render on the live site

Run the Markdown table audit and fix inconsistent pipe-table cell counts:

```bash
python3 ~/.hermes/skills/productivity/obsidian-quartz-publish/scripts/markdown_table_audit.py content
```

### Frontmatter appears as visible page text

Check that the file starts and ends frontmatter with exactly three dashes:

```markdown
---
title: Example
---
```

### Local paths or credentials appear in content

Treat this as a publication blocker. Redact the source Markdown, rebuild, rerun privacy audit, commit, push, and verify the live page plus `static/contentIndex.json`.

## Useful links

- Live site: https://zer0s000-g.github.io/sbas-kb/
- Repository: https://github.com/zer0s000-g/sbas-kb
- GitHub Actions: https://github.com/zer0s000-g/sbas-kb/actions
- Quartz documentation: https://quartz.jzhao.xyz/

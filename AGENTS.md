# AGENTS.md

## Cursor Cloud specific instructions

This is a Jekyll 4.4 static portfolio site (Ruby 3.2+). There is no database, no Docker, no Node.js, and no backend services.

### Running locally

```bash
bundle exec jekyll serve --host 0.0.0.0
```

The dev server starts on `http://127.0.0.1:4000`. It supports live-reload and auto-regeneration when files change.

### Build

```bash
bundle exec jekyll build
```

Output goes to `_site/`.

### Key caveats

- Bundler is configured with `path: vendor/bundle` (local install). This avoids permission issues in the cloud VM.
- The Gemfile.lock targets `x86_64-linux-gnu` so gems install without compilation issues on the cloud VM.
- There is no linter configured in this project (no Rubocop, no HTMLProofer). The CI workflow (`.github/workflows/pages.yml`) only builds and deploys via GitHub Pages.
- The site content is in Dutch. Pages: Home (`/`), Over mij (`/over-mij/`), Aan de slag (`/aan-de-slag/`), Projecten (`/projecten/`).

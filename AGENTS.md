# Repository Guidelines

## Project Structure & Modules
This HugoBlox Academic CV site keeps global settings under `config/_default/`: adjust branding in `hugo.yaml`, SEO and appearance in `params.yaml`, navigation in `menus.yaml`, languages in `languages.yaml`, and module mounts in `module.yaml`. Hugo modules pull in `blox-tailwind` and `blox-plugin-netlify`; run module maintenance commands from the repo root. Content bundles live in `content/` (`authors/admin`, `projects`, `blog`, `publications`, `experience.md`), while layouts and shortcodes belong in `layouts/`. Media for each page stays inside its bundle or in `assets/`, and deploy artifacts in `public/` should never be committed.

## Build, Test, and Maintenance Commands
```bash
pnpm install         # install Tailwind and HugoBlox dependencies
npm run dev          # hugo server with live reload
npm run build        # production build to public/
hugo --gc --minify   # clean cache + minify for release builds
hugo mod tidy        # remove unused module refs
hugo mod get -u      # update module versions
hugo mod vendor      # vendor modules for offline work
```
Verify that `npm run build` succeeds before opening a PR and keep the working tree clean of generated files.

## Coding Style & Naming Conventions
Use two spaces in YAML/TOML and align nested front matter logically. Keep Markdown bundle folders lowercase with dash-separated slugs (for example, `content/projects/roi-audit/`). Reference media via relative paths into the same bundle or `assets/images/`, and let Tailwind’s generated CSS dictate utility order—never edit `public/` CSS by hand. Russian remains the default locale; mirror existing capitalization and punctuation in localized copy.

## Testing & Verification
Treat `npm run build` as the regression gate. Spot-check key pages through `npm run dev`, then confirm responsive behavior and Lighthouse guidance described in `MOBILE_OPTIMIZATION.md`. For structural changes, inspect the generated `public/` output and run `hugo --gc` to surface stale resources.

## Deployment Workflow
GitHub Actions deploys `main` via `.github/workflows/deploy.yml` to GitHub Pages. Production runs expect Hugo 0.150.0, Node 22, Go 1.21.5, and use `HUGO_ENV=production`; enable `HUGO_ENABLEGITINFO=true` when you need git-sourced “last updated” dates. Update `baseURL` in `config/_default/hugo.yaml` if domains change.

## Commit & Pull Request Guidelines
Follow the existing short, imperative subject style (e.g., `adjust hero copy`). Group related edits, omit build artifacts, and mention configuration or module updates explicitly. Pull requests should describe the user-facing outcome, link issues when relevant, and add before/after screenshots for visual tweaks or navigation changes.

## Content Authoring Workflow
Duplicate an existing bundle under `content/` to add sections, updating front matter fields like `title`, `summary`, `weight`, and `draft`. Keep headshots and project imagery in `assets/images/` and reference them within the bundle. For bilingual copy, keep translated Markdown in the same bundle and gate it with `draft: true` until review is complete.

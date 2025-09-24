# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Hugo-based website using the Academic CV theme from HugoBlox, designed as a portfolio site for Алена Ирошникова (Alena Iroshnikova), a marketer. The site uses Hugo modules system with HugoBlox components and is deployed on GitHub Pages via GitHub Actions.

## Development Commands

### Local Development
- `npm run dev` or `hugo server --disableFastRender` - Start development server with live reload
- `npm run build` or `hugo --minify` - Build production site to `public/` directory
- `pnpm install` - Install dependencies (Tailwind CSS v4 and related packages)

### Hugo-Specific Commands
- `hugo mod tidy` - Clean up unused module dependencies
- `hugo mod get -u` - Update all Hugo modules
- `hugo mod vendor` - Vendor modules to local directory for offline development

## Site Architecture

### Configuration Structure
- `config/_default/` - Main configuration directory
  - `hugo.yaml` - Main Hugo configuration (title, baseURL, advanced settings)
  - `params.yaml` - Site parameters (appearance, SEO, features)
  - `module.yaml` - Hugo modules imports and mounts
  - `languages.yaml` - Multi-language configuration
  - `menus.yaml` - Navigation menu structure

### Theme & Modules
- Uses HugoBlox Academic CV theme via Hugo modules
- Two main modules:
  - `blox-plugin-netlify` - Netlify deployment optimizations
  - `blox-tailwind` - Tailwind CSS v4 integration
- Theme files mounted from `hugo-blox/blox/` directory

### Content Structure
- `content/authors/admin/_index.md` - Main profile page (needs customization for Alena Iroshnikova)
- `content/blog/` - Blog posts and articles
- `content/projects/` - Portfolio projects
- `content/publications/` - Academic publications
- `content/experience.md` - Work experience page
- `content/courses/` - Educational content

### Key Features
- Responsive design with dark/light mode toggle
- SEO optimized with structured data
- BibTeX citation support for publications
- Image processing and optimization
- Search functionality and image optimization
- Mobile-first responsive design
- SEO optimization with structured data

## Deployment

### GitHub Pages via GitHub Actions
- Workflow file: `.github/workflows/deploy.yml`
- Auto-deployment on push to `main` branch
- Hugo version: 0.150.0, Node version: 22, Go version: 1.21.5
- Production builds use minification and garbage collection

### Setup Instructions
1. Enable GitHub Pages in repository Settings → Pages → Source → **GitHub Actions**
2. Workflow will run automatically on push to `main`
3. Site available at: `https://username.github.io/repository-name/`
4. For custom domain: update `baseURL` in `config/_default/hugo.yaml`

### Environment Variables
- `HUGO_ENV=production` for production builds
- `HUGO_ENABLEGITINFO=true` for git-based last modified dates

## Content Customization

### Profile Setup for Alena Iroshnikova ✅ COMPLETED
- `content/authors/admin/_index.md` - Updated with Alena's information:
  - Personal info: Алена Ирошникова, B2B marketing expert
  - 18+ years experience with KNIPEX, Jungheinrich, Siemens
  - Education: ВШЭ (Masters), МГУ (Bachelor)
  - Social media: LinkedIn, Telegram, email
  - Skills focused on B2B marketing, brand strategy, product launch

### Site Configuration ✅ COMPLETED
- `config/_default/hugo.yaml` - Updated title for B2B marketer
- `config/_default/params.yaml` - SEO optimized for Russian market
- `config/_default/menus.yaml` - Russian navigation menu
- Localization set to Russian as primary language

### Content Organization ✅ COMPLETED
- `content/projects/` - 3 real marketing cases with ROI metrics
- `content/_index.md` - Hero section with marketing expertise
- `layouts/partials/hooks/head-end/` - Custom SEO and mobile optimizations
- Removed demo content (publications, events, courses)
- Blog posts kept for content marketing
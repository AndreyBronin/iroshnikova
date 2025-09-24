# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Hugo-based website using the Academic CV theme from HugoBlox, designed as a portfolio site for Алена Ирошникова (Alena Iroshnikova), a marketer. The site uses Hugo modules system with HugoBlox components and is deployed on Netlify.

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
- Search functionality (Pagefind integration on Netlify)

## Deployment

### Netlify Configuration
- Build command includes Hugo build + Pagefind indexing
- Hugo version: 0.150.0
- Node version: 22
- Go version: 1.21.5
- Production builds use minification and garbage collection

### Environment Variables
- `HUGO_ENV=production` for production builds
- `HUGO_ENABLEGITINFO=true` for git-based last modified dates

## Content Customization

### Profile Setup for Alena Iroshnikova
- Edit `content/authors/admin/_index.md` to update:
  - Personal information (name, role, bio)
  - Professional experience and education
  - Social media links and contact information
  - Skills and interests relevant to marketing
- Replace `content/authors/admin/avatar.png` with Alena's photo

### Site Configuration
- Update `config/_default/hugo.yaml` title and baseURL
- Modify `config/_default/params.yaml` for:
  - Site branding (`header.navbar.logo.text`)
  - SEO settings (`marketing.seo`)
  - Color scheme (`appearance.color`)

### Content Organization
- Blog posts use markdown with front matter
- Projects support featured images and detailed descriptions
- Publications support BibTeX citations and PDF attachments
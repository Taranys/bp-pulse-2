# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## First Task

When working with this Slidev project, always read https://sli.dev/llms.txt first to gather information about Slidev features, syntax, and best practices.

## Project Overview

This is a Slidev presentation repository for "AI Reality Check" - a presentation about AI wins, fails, and lessons learned at BOSS/Doctolib. The presentation is built using Slidev and deployed to GitHub Pages.

## Package Manager

This project uses **npm** (not pnpm despite what the README says). The lock file is `package-lock.json`.

## Common Commands

### Development
- `npm install` - Install dependencies
- `npm run dev` - Start development server (opens at http://localhost:3030)

### Building
- `npm run build` - Build presentation for production (outputs to `docs/` directory with base path `/bp-pulse-2/`)
- `npm run export` - Export slides (to PDF or other formats)

### Deployment
The presentation is automatically deployed to GitHub Pages via GitHub Actions when changes are pushed to the `docs/` directory on the `main` or `master` branch.

## Architecture

### File Structure
- **`slides.md`** - Main presentation content. This is the primary file to edit.
- **`docs/`** - Build output directory (used for GitHub Pages deployment, committed to git)
- **`components/`** - Custom Vue components for slides
- **`pages/`** - Additional slide pages that can be imported
- **`snippets/`** - Code snippets for use in slides
- **Static assets** - Place images and other assets in the root directory (e.g., `QrCode.png`)

### Slidev Configuration
The presentation uses:
- **Theme**: `@doctolib/slidev-theme` (Doctolib's custom theme)
- **CSS Engine**: UnoCSS (for styling)
- **MDC Syntax**: Enabled (for enhanced Markdown features)
- **Transitions**: slide-left (default)

### Slide Structure
Slides are written in Markdown with frontmatter configuration:
- Each slide is separated by `---`
- Frontmatter at the top configures presentation-wide settings
- Individual slides can have their own frontmatter (layout, class, background, transition, etc.)
- Supports Vue components, UnoCSS classes, and v-click animations

### Deployment Strategy
This project uses a static deployment approach:
1. Build output goes to `docs/` directory (not `dist/`)
2. The `docs/` directory is committed to git
3. GitHub Actions deploys from `docs/` to GitHub Pages
4. Base path is set to `/bp-pulse-2/` for GitHub Pages routing

### Static Assets
Images and assets should be:
- Placed in the root directory
- Referenced with leading slash (e.g., `/QrCode.png`)
- Will be copied to `docs/assets/` during build with hashed filenames

## Theme-Specific Features

The Doctolib theme supports:
- **Layouts**: `default`, `center`, `cover`, `section`, etc.
- **Background images**: Via `background:` property in frontmatter
- **Custom styling**: UnoCSS utility classes for positioning and styling
- **Vue components**: Can be used inline in slides

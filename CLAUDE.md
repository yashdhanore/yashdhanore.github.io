# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website for Yash Dhanore, hosted on GitHub Pages at `yashdhanore.github.io`. The site is built as a static website using the HTML5 UP "Forty" template with Jekyll integration for GitHub Pages hosting.

## Technology Stack

- **Static HTML/CSS/JavaScript** - No backend framework
- **Jekyll** - Minimal configuration for GitHub Pages compatibility
- **SCSS/Sass** - For CSS preprocessing
- **jQuery** - Core JavaScript functionality including scrolly and scrollex plugins
- **HTML5 UP "Forty" template** - Professional portfolio template base

## Common Development Commands

Since this is a static Jekyll site hosted on GitHub Pages, development is primarily done through direct file editing. GitHub Pages handles Jekyll compilation automatically.

**Local development (if Jekyll is installed):**
```bash
bundle exec jekyll serve
```

**SCSS compilation** happens automatically through Jekyll/GitHub Pages - no manual build process required.

## Architecture and File Structure

### Core Files
- `index.html` - Main portfolio page with project showcase
- `_config.yml` - Jekyll configuration (minimal setup with theme reference)
- `assets/sass/main.scss` - Main SCSS entry point with comprehensive import structure

### Asset Organization
- `assets/sass/` - SCSS source files organized in modular structure:
  - `libs/` - Framework utilities (vars, mixins, breakpoints, grid system)
  - `base/` - Foundation styles (reset, page, typography)
  - `components/` - Reusable UI components (buttons, forms, tiles, etc.)
  - `layout/` - Page structure (header, banner, main, footer, menu)
- `assets/css/` - Compiled CSS output
- `assets/js/` - JavaScript files and jQuery plugins
- `images/` - Portfolio images and project screenshots

### Responsive Design System
The template uses a comprehensive breakpoint system defined in `main.scss`:
- xxsmall: ≤360px
- xsmall: 361px-480px
- small: 481px-736px
- medium: 737px-980px
- large: 981px-1280px
- xlarge: 1281px-1680px

### Template Structure
Built on HTML5 UP "Forty" template featuring:
- Modular SCSS architecture with clear separation of concerns
- Responsive grid system
- jQuery-powered smooth scrolling and scroll-based animations
- Tile-based project showcase layout
- Professional typography using Source Sans Pro

## Key Development Notes

- **No build process required** - GitHub Pages handles Jekyll compilation
- **Direct file editing workflow** - Changes can be made directly to HTML/SCSS files
- **Template-based** - Core functionality comes from HTML5 UP template structure
- **Mobile-first responsive design** - Uses breakpoint mixins for responsive layouts
- **jQuery dependencies** - Site relies on jQuery and custom plugins (scrolly, scrollex)

## Content Management

Portfolio content is managed directly in `index.html`:
- Project tiles in the "tiles" section
- Personal information in the banner section
- Links to GitHub repositories for project showcases
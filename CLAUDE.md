# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview
This is a personal portfolio/academic website built with Quarto, a scientific publishing system. The website showcases research interests, publications, teaching experience, and professional background for Sitao Min, a Ph.D. candidate at Rutgers University.

## Tech Stack
- **Quarto**: Static site generator (version 1.7.32)
- **HTML/CSS**: Bootstrap theme (lumen) with custom styles
- **Output**: Static HTML files in `docs/` directory for GitHub Pages deployment

## Commands

### Development
```bash
quarto preview    # Live preview with hot reload
```

### Build
```bash
quarto render     # Build site to docs/ directory
```

### Deploy
```bash
quarto publish gh-pages    # Deploy to GitHub Pages
```

## Project Structure
- `*.qmd` files: Quarto markdown source files for each page
- `_quarto.yml`: Main configuration file defining site structure, theme, and build settings
- `docs/`: Generated output directory containing built HTML site
- `images/`: Image assets used throughout the site
- `papers/`: PDF research papers
- `styles.css`: Custom CSS overrides

## Key Configuration
The site is configured in `_quarto.yml`:
- Output directory: `docs/` (for GitHub Pages compatibility)
- Theme: lumen (Bootstrap)
- Navigation: About, Research, Experience, Teaching sections
- Search enabled
- Responsive design with max-width: 2500px

## Content Pages
- `index.qmd`: About/homepage with education and research interests
- `research.qmd`: Research projects and publications
- `experience.qmd`: Professional experience
- `teaching.qmd`: Teaching experience
- Additional pages follow same `.qmd` format

## Important Notes
- The site uses Quarto's visual editor mode
- TinyTeX is installed for LaTeX support if needed
- Python/Jupyter integration available but nbclient module may need installation for notebook rendering
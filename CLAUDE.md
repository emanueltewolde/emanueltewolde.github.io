# CLAUDE.md - Personal Website Overview

## Project Overview
This is Emanuel Tewolde's personal academic website (emanueltewolde.com) built using Jekyll and hosted on GitHub Pages. The site is based on the Academic Pages template, a fork of the Minimal Mistakes Jekyll theme.

## Website Owner
**Emanuel Tewolde** - 4th year PhD student in Computer Science at Carnegie Mellon University
- Research focus: Algorithmic game theory, reinforcement learning, AI safety, coordination, cooperation, and alignment
- Advisor: Vincent Conitzer
- Supported by: Cooperative AI PhD Fellowship

## Technical Stack
- **Framework**: Jekyll (Ruby-based static site generator)
- **Theme**: Academic Pages (forked from Minimal Mistakes)
- **Hosting**: GitHub Pages
- **Domain**: emanueltewolde.com (via CNAME file)
- **Ruby Dependencies**: Managed via Gemfile/Bundler
- **JavaScript**: Minimal - mainly for UI enhancements (jQuery, plugins)

## Repository Structure

### Configuration Files
- `_config.yml` - Main Jekyll configuration with site metadata, author info, collections, and build settings
- `_config.dev.yml` - Development configuration override
- `Gemfile` - Ruby dependencies (github-pages, jekyll plugins)
- `package.json` - npm build scripts for JavaScript minification

### Content Collections
The site uses Jekyll collections to organize different types of content:

#### Publications (`_publications/`)
- 8 academic papers (2021-2025)
- Format: Markdown files with YAML front matter
- Fields: title, authors, venue, status, dates, file links, arXiv URLs
- Example: `2025-04-01-LearnPhiEQs.md` (EC 2025 paper)

#### Working Papers (`_workingpapers/`)
- 3 working papers (2025)
- Similar format to publications but for unpublished work
- Example: `2025-05-01-Concordia.md` (Concordia LLM evaluation paper)

#### Teaching (`_teaching/`)
- 9 teaching experiences (2014-2025)
- Format: Course information with dates and descriptions
- Latest: "Cooperative AI" course (2025) as Head TA

#### Talks (`_talks/`)
- Academic presentations and tutorials
- Currently has 4 sample entries

#### Portfolio (`_portfolio/`)
- Project showcase (minimal content currently)

### Pages (`_pages/`)
Key pages include:
- `about.md` - Homepage with bio, research interests, and dynamic content sections
- `cv.md` - Curriculum vitae page
- `publications.md` - Publications listing
- `teaching.html` - Teaching experience
- Various archive and utility pages

### Layout & Design (`_layouts/`, `_includes/`, `_sass/`)
- **Layouts**: Templates for different page types (single, archive, talk)
- **Includes**: Reusable components (header, footer, author profile, navigation)
- **Sass**: Styling with variables, mixins, and component styles

### Assets
- `files/` - PDFs (CV, papers, posters)
- `images/` - Profile photos and icons
- `assets/` - CSS, JavaScript, fonts
- `_site/` - Generated static site (build output)

### Data (`_data/`)
- `navigation.yml` - Site navigation (currently commented out)
- `authors.yml` - Author information
- `ui-text.yml` - UI text strings

## Key Features

### Dynamic Content Generation
The homepage (`about.md`) dynamically displays:
- Working papers section (if any exist)
- Publications (reverse chronological)
- Teaching experience (reverse chronological)

### Build Process
- Jekyll processes Markdown + YAML front matter
- Sass compilation for CSS
- JavaScript minification via npm scripts
- Output to `_site/` directory

### SEO & Analytics
- Google Analytics integration
- Sitemap generation
- SEO optimization via jekyll-seo-tag

## Development Workflow

### Local Development
```bash
bundle install          # Install Ruby dependencies
bundle exec jekyll serve # Run local server
npm run build:js        # Build JavaScript assets
```

### Content Management
- Publications: Add new `.md` files to `_publications/`
- Teaching: Add new `.md` files to `_teaching/`
- Working papers: Add new `.md` files to `_workingpapers/`
- Files: Upload PDFs to `files/` directory

### Navigation
Currently, main navigation is commented out in `_data/navigation.yml`, making the site a single-page layout focused on the about page.

## Content Conventions
- Author ordering notation: "- αβ -" indicates alphabetical ordering
- Equal contribution: "==" superscripts
- File naming: YYYY-MM-DD-descriptive-name.md
- YAML front matter required for all content files

## Dependencies & Security
- Uses GitHub Pages compatible gems
- All dependencies managed through Gemfile
- No custom plugins that would break GitHub Pages compatibility
- Regular Jekyll and theme updates via gem updates

## Notes
- The site is currently a work in progress, particularly the working papers section
- Navigation is simplified to focus content on the main about page
- Academic focus with emphasis on publications and teaching
- Clean, professional design suitable for academic portfolio
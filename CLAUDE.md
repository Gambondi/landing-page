# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website built on HTML5 UP's "Landed" template - a dark, modern, responsive design with dynamic landing page functionality. The site serves as Matthew Moturi Ondeyo's student developer portfolio showcasing projects and providing contact information.

## Architecture

The site follows a traditional static HTML structure with:

- **Main Landing Page**: `index.html` - Contains hero section, project overview cards, and navigation
- **Project Detail Pages**: `project-1.html` through `project-6.html` - Individual project showcases with detailed descriptions
- **Asset Structure**:
  - `assets/css/` - Compiled CSS (main.css) and noscript fallback
  - `assets/sass/` - Source SCSS files with modular organization (main.scss imports from libs/)
  - `assets/js/` - jQuery-based JavaScript with plugins for scrolling, dropdowns, and responsive behavior
  - `images/` - Project images, screenshots, and profile photos

## CSS/SASS Architecture

The styling uses a sophisticated SASS setup:

- **Main Entry**: `assets/sass/main.scss` imports all partials
- **Core Libraries**: Located in `assets/sass/libs/` with modular concerns:
  - `_vars.scss` - Color palette, fonts, sizing variables
  - `_mixins.scss` - Reusable SASS mixins
  - `_breakpoints.scss` - Responsive breakpoint definitions
  - `_functions.scss` - SASS utility functions
- **Responsive Design**: Mobile-first with breakpoints (xsmall: 480px, small: 736px, medium: 980px, large: 1280px, xlarge: 1680px)
- **Key Components**: Spotlight sections, wrapper styles, navigation system, and form elements

## JavaScript Architecture

jQuery-based functionality with these key plugins:
- **jquery.scrolly.min.js** - Smooth scrolling for anchor links
- **jquery.dropotron.min.js** - Dropdown menu functionality
- **jquery.scrollex.min.js** - Scroll-based animations and effects
- **browser.min.js** and **breakpoints.min.js** - Responsive utilities
- **main.js** - Site initialization, mobile detection, and component bindings

## Navigation Structure

- Fixed header with logo and dropdown navigation
- Mobile responsive with slide-out navigation panel
- Project dropdown links to individual project pages
- External resume link (Adobe PDF)

## Content Management

Individual project pages follow consistent structure:
- Hero section with project title and description
- Technology stack details
- Key features and functionality lists
- Impact and benefits sections
- Consistent footer with social links

## Development Notes

- No build process required - direct SASS compilation to CSS
- Static site suitable for GitHub Pages or similar hosting
- Font Awesome icons integrated via CDN
- Images should be optimized and properly sized for responsive display
- Social media links in header/footer currently placeholder (`#` links)

## Common Tasks

When editing this site:
- Update project content by modifying individual `project-*.html` files
- Add new projects by creating new project pages following existing pattern
- Modify styling through SASS files in `assets/sass/`
- Images go in `images/` directory and should be referenced relatively
- Social links and contact information need updating from placeholder values
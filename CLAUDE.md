# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML presentation for Dragon Den pitches in Dungeons & Dragons campaigns. The presentation follows a fantasy-themed narrative centered around "HealthUp" - a revolutionary healing product for adventurers.

## Codebase Structure

The entire application is contained in a single HTML file (`index.html`) with three main sections:

1. **HTML Structure** - Contains 10 slide sections organized by chapters:
   - The Problem (slides 1-2)
   - The Solution (slides 3-4)
   - The Product (slide 5)
   - The Differentiator (slides 6-7)
   - The System (slide 8)
   - The Ask (slides 9-10)

2. **CSS Styling** - All styles are embedded in the `<style>` tag with organized sections:
   - Color variables in `:root`
   - Layout components (#app, #sidebar, #stage)
   - Slide transitions and positioning
   - Typography utilities (.eyebrow, .headline, .subline, etc.)
   - Component styles (.vial, .hup-unit, .pack-diagram, etc.)
   - Responsive design with clamp() for scalable typography

3. **JavaScript Functionality** - Handles presentation logic:
   - Slide navigation (keyboard arrows, buttons, touch swipe)
   - Chapter-based sidebar navigation
   - Progress tracking and UI updates
   - Animation timing controls

## Common Development Tasks

### Running the Project
- Simply open `index.html` in any modern web browser
- No build process or dependencies required

### Modifying Content
- Edit slide content directly within each `.slide` div
- Adjust styling in the CSS section of the same file
- Modify navigation behavior in the JavaScript section

### Adding New Slides
- Create a new `.slide` div with appropriate data attributes
- Follow existing patterns for consistency
- Update JavaScript if adding complex interactions

## Architecture Patterns

1. **Component-Based CSS** - Reusable utility classes for consistent styling
2. **Data-Driven Navigation** - Slides and chapters managed through dataset attributes
3. **Progressive Enhancement** - Core functionality works without JavaScript
4. **Self-Contained Design** - All code in one file for maximum portability

## Key Variables and Selectors

- `:root` color variables for consistent theming
- `.slide` elements with `data-chapter` and `data-index` attributes
- `.chapter-item` for sidebar navigation
- Animation timing controlled through `setTimeout` durations
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an ESG GenAI Compliance Platform presentation built as a static HTML website. It contains 12 presentation slides showcasing an AI-powered ESG reporting automation platform, presented in Korean language.

## Development Commands

### Local Development
```bash
# Start local development server (Python)
npm run dev
# or
python -m http.server 3000

# Alternative with Node.js
npx http-server -p 3000
```

### Build & Deploy
```bash
# No build step needed (static files)
npm run build

# Deploy to Vercel (configured for static hosting)
# Deployment handled via vercel.json configuration
```

## Project Structure

### Core Files
- `index.html` - Main navigation page with slide grid layout
- `assets/common.css` - Global styles and design system
- `package.json` - Project metadata and scripts
- `vercel.json` - Vercel deployment configuration

### Slides Directory
12 individual HTML slide files in `/slides/`:
1. `01-title.html` - Title slide
2. `02-executive-summary.html` - Executive summary with 5 key cards
3. `03-market-analysis.html` - Market analysis and pain points
4. `04-why-now.html` - Market timing and opportunities
5. `05-competitive-landscape.html` - ESG SaaS competitive analysis
6. `06-solution-overview.html` - 3-step process overview
7. `07-key-features.html` - As-Is vs To-Be comparison
8. `08-technology-architecture.html` - Technical stack
9. `09-project-milestones.html` - MVP achievements
10. `10-roadmap.html` - Future development roadmap
11. `11-resource-requests.html` - Team expansion and budget requests
12. `12-qa.html` - Q&A and contact information

## Architecture

### Design System
- **Primary Color**: #4CAF50 (Green - representing ESG/sustainability)
- **Font**: Inter font family from Google Fonts
- **Icons**: Font Awesome 6.4.0
- **Framework**: Tailwind CSS 2.2.19 for utility classes
- **Layout**: Card-based modern design with hover effects

### Styling Approach
- Global styles in `assets/common.css`
- Inline styles for slide-specific customizations
- CSS custom properties (variables) for consistent theming
- Responsive design with mobile-first approach

### Navigation System
- Main index page provides slide overview grid
- Each slide is standalone HTML file
- Navigation between slides via slide-nav component
- Keyboard navigation support (arrow keys)
- Touch/swipe support for mobile devices

## Content Structure

The presentation follows a logical business case flow:
1. **Problem identification** (market analysis, pain points)
2. **Solution positioning** (why now, competitive landscape)
3. **Product demonstration** (solution overview, key features)
4. **Technical credibility** (architecture, milestones)
5. **Future vision** (roadmap, resource requests)

## Development Guidelines

### File Organization
- Keep slide HTML files focused and semantic
- Use common.css for shared styles
- Maintain consistent naming conventions
- Preserve Korean language content accurately

### Styling Conventions
- Use existing CSS utility classes from common.css
- Follow the established color palette
- Maintain consistent spacing and typography
- Ensure responsive behavior across devices

### Content Updates
- Slides contain business-sensitive information (budget, team size, ROI)
- Maintain professional tone and formatting
- Keep slide transitions smooth and consistent
- Preserve accessibility features (keyboard navigation)

## Deployment

The project is configured for Vercel static hosting:
- No build process required
- Direct file serving from root directory
- Automatic deployments from git repository
- Custom domain configuration available via Vercel dashboard
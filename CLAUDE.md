# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML redirect page for Quick Spot customers after completing Stripe payment setup. The entire application is a single self-contained HTML file with embedded CSS and inline SVG graphics.

## Architecture

- **Single-file architecture**: All HTML, CSS, and animations are in `index.html`
- **Static deployment**: Designed for Vercel with no build process required
- **Vercel configuration**: `vercel.json` uses rewrites (not routes) to handle all requests and set cache headers

## Development Commands

```bash
# Local development server
npm run dev

# Deploy to production
npm run deploy

# Or deploy via Vercel CLI
vercel --prod
```

## Key Implementation Details

- **No external CSS/JS files**: All styling and animations are embedded in index.html
- **Animations**: Uses CSS keyframes for checkmark scale-in and SVG stroke draw animations
- **Brand colors**: Sky blue (#87ceeb) and coral (#ff6b35) gradient for checkmark
- **Typography**: Inter font family loaded from Google Fonts
- **Contact email**: quickspot.help@gmail.com

## Deployment Notes

- Vercel configuration uses `rewrites` (not `routes`) to avoid deprecation warnings
- Static site builder: `@vercel/static`
- Cache headers set to 1 year for optimal performance

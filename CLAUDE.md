# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio website for lvboda.cn — a single-page static site with no build system or dependencies.

## Architecture

The entire site is a single `index.html` file with inline CSS and JavaScript. There is no package.json, no bundler, and no framework. The site is bilingual (Chinese/English).

- `index.html` — Full page: markup, styles, and a toggle script for the "Personal Projects" section
- `favicon.ico` — Site icon (PNG format)

## Deployment

Hosted on **Cloudflare Workers/Pages**. The `cloudflare/workers-autoconfig` branch contains `wrangler.jsonc` configuration. Static assets are served directly from the repository root.

## Development

No build or install step. Open `index.html` in a browser to preview. For Cloudflare Workers local dev, use `npx wrangler dev` (requires the wrangler config from the cloudflare branch).

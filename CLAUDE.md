# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Static website for wpo-org-uk. Plain HTML, CSS, and minimal JavaScript — no build tools, no framework, no site generator.

## Purpose

This is the website for the Westminster Philharmonic Orchestra

The users include 
- members of the orchestra looking for rehearsal and concert details
- the public looking for details of a concert
- curious people looking for information about the orchestra, including its history and people involved


## Development

Open files directly in a browser, or serve locally to avoid CORS issues with any fetch calls:

```bash
python3 -m http.server 8000
```

## Structure

- `index.html` — site entry point
- `css/` — stylesheets
- `js/` — JavaScript files
- `assets/` — images and other static files

## Conventions

- Prefer semantic HTML
- Keep JavaScript minimal and dependency-free
- CSS should be plain — no preprocessors
- support desktop and mobile phone browsers

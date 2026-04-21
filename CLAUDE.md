# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

## Project

Static website for the Westminster Philharmonic Orchestra (WPO). Plain HTML, CSS, and minimal JavaScript — no build tools, no framework, no site generator.

## Audience

- Orchestra members — rehearsal schedules, concert details
- The public — upcoming concerts, how to attend or support
- Curious visitors — orchestra history, people, and how to get involved

## Development

Serve locally to avoid CORS issues with any fetch calls:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` in a browser. Files can also be opened directly, but fetch-based features may not work.

## Structure

- `index.html` — home page / site entry point
- `concerts.html` — upcoming concerts listing
- `concerts/` — individual concert detail pages (e.g. `spring-2026-05-09.html`)
- `rehearsals.html` — rehearsal schedule; `rehearsals.ics` — iCal feed
- `about.html`, `history.html`, `people.html` — orchestra information
- `members.html` — member resources
- `support.html`, `contact.html` — supporting and contacting the orchestra
- `css/style.css` — single stylesheet
- `js/main.js` — minimal site-wide JavaScript (nav toggle etc.)
- `assets/` — images, logos, icons
- `fonts/` — web fonts

## Conventions

- Semantic HTML throughout
- Accessibility: use ARIA attributes and skip-links as established in existing pages
- JavaScript: dependency-free, minimal, progressive enhancement only
- CSS: plain, no preprocessors; single `style.css`
- Support both desktop and mobile browsers
- New concert pages go in `concerts/` following the `season-YYYY-MM-DD.html` naming pattern

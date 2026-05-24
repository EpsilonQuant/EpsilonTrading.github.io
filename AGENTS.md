# AGENTS.md

Guidance for AI coding agents working in this repository.

## Overview

This repository hosts the GitHub Pages site for the `epsilon.trading` domain. It
is intentionally minimal: it serves a single page that redirects visitors to
`https://epsilonquant.com/`.

## Repository layout

- `index.html` — the page served at the domain root. It performs an immediate
  `meta refresh` redirect to `https://epsilonquant.com/` with a fallback link.
- `CNAME` — configures the custom domain (`epsilon.trading`) for GitHub Pages.
- `README.md` — short description of the repository.

## How it works

GitHub Pages serves `index.html` from the default branch at the domain defined
in `CNAME`. There is no build step, package manager, or framework — the site is
plain static HTML.

## Working in this repo

- Keep the site minimal. The sole purpose is the redirect; avoid adding
  dependencies, build tooling, or frameworks unless explicitly requested.
- If you change the redirect target, update it in `index.html` (both the
  `meta refresh` URL and the fallback `<a href>`).
- Do not modify `CNAME` unless the custom domain is intentionally changing.
- There are no tests or build commands. Validate changes by opening
  `index.html` in a browser and confirming the redirect behaves as expected.

## Conventions

- All Markdown files should begin with a single top-level (`#`) heading.
- Never attribute work to AI. Do not add AI co-authorship, "Generated with"
  notices, or any similar mention in commit messages, pull requests, code
  comments, or anywhere else.

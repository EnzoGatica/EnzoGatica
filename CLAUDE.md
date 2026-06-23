# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is the `EnzoGatica/EnzoGatica` special GitHub repository. GitHub automatically renders its `README.md` as the public profile page at [github.com/EnzoGatica](https://github.com/EnzoGatica). There is no build system, no dependencies, and no tests — the entire output is the rendered Markdown/HTML on that profile page.

## Repository Structure

- **`README.md`** — The profile page content. GitHub renders this directly; changes pushed to `main` are immediately live.
- **`svg/`** — Local SVG icon assets available for use in the README (currently unused; the README relies on shields.io badges and external image URLs instead).

## README Architecture

The README uses a mix of raw HTML `<div>` blocks and Markdown, in this section order:

1. **Header** — Animated typing SVG from `readme-typing-svg.demolab.com`
2. **Dino runner** — ASCII art block in a fenced code block
3. **About me** — Two-column Markdown table
4. **Languages & Tools** — Row of `shields.io` flat-square badge images
5. **Experience** — Four-column Markdown table (icon, role, company, period)
6. **GitHub Stats** — Two side-by-side stat cards from `github-readme-stats-sigma-five.vercel.app`
7. **Social links** — Centered `shields.io` for-the-badge images wrapped in `<a>` tags

## Key Conventions

- Badge style for the Languages & Tools section is `style=flat-square`; social link badges use `style=for-the-badge`.
- External stat card URLs reference username `EnzoGatica` (case-sensitive) and use `theme=dark&hide_border=true&bg_color=0d1117`.
- The `svg/` assets are not currently referenced in the README. If local assets are ever used, link them with a relative path (e.g., `./svg/python-5.svg`), but note that GitHub caches external images via camo — shields.io badges are generally preferred for consistency.
- Section separators use `---` (horizontal rule).
- All table content and badge alt-text should stay in English even though experience entries use Spanish (matching the existing style).

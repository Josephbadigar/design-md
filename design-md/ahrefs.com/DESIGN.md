---
version: alpha
name: Ahrefs
description: "Dark interface measured from ahrefs.com: Ahrefs type with Inter, vivid orange accents, flat surfaces and pill-shaped controls."
colors:
  background: "#3A57FC"
  surface: "#3A57FC"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#000000"
  on-surface-muted: "#C4CDFE"
  overlay: "#00000026"
  overlay-strong: "#FFFFFF33"
  outline: "#FFFFFF4D"
  outline-variant: "#00000033"
  primary: "#FF8D00"
  on-primary: "#FFFFFF"
  secondary: "#C9C47A"
  tertiary: "#6B6820"
typography:
  display-hero:
    fontFamily: Ahrefs
    fontSize: 64px
    fontWeight: 400
    lineHeight: 0.94
  headline-display:
    fontFamily: Ahrefs
    fontSize: 60px
    fontWeight: 400
    lineHeight: 0.95
  headline-lg:
    fontFamily: Ahrefs
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: Ahrefs
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.06
  headline-sm:
    fontFamily: Ahrefs
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.08
  body-md:
    fontFamily: Ahrefs
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
  body-sm:
    fontFamily: Ahrefs
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
  label-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.61
  headline-display-mobile:
    fontFamily: Ahrefs
    fontSize: 41px
    fontWeight: 400
    lineHeight: 0.95
  display-hero-mobile:
    fontFamily: Ahrefs
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
  headline-md-mobile:
    fontFamily: Ahrefs
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.08
rounded:
  sm: 4px
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 12px
  section: 96px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 5px
    padding: 17px 32px
    height: 72px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: 3px
    padding: 4px 12px
    height: 32px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 7px 16px
    height: 42px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 7px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Ahrefs Design System

## Overview

Ahrefs describes itself as: “We help marketers drive visibility across AI search, SEO, content, and social – with the largest AI and search databases online.” The interface is dark, built on **Vivid Indigo (#3A57FC)** with **White (#FFFFFF)** text, and **Vivid Orange (#FF8D00)** as the main accent.

Type is set in **Ahrefs** and **Inter**. Headlines run large; body text is 20px. The surface language is flat. Controls are pill-shaped.

Measured from [ahrefs.com](https://ahrefs.com/) on November 4, 2026 at 1440×900 and 390×844 from 346 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Vivid Indigo (#3A57FC):** Page background, seen 7 times. Token `background`, CSS `--color-link`.
- **White (#FFFFFF):** Primary text and headings, seen 49 times. Token `on-surface`.
- **Near Black (#000000):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Pale Indigo (#C4CDFE):** Muted text and metadata, seen 10 times. Token `on-surface-muted`.
- **Near Black 15% (#00000026):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 20% (#FFFFFF33):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **White 30% (#FFFFFF4D):** Borders and dividers, seen 7 times. Token `outline`.
- **Near Black 20% (#00000033):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Orange (#FF8D00):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--accentPrimary-1ygyxil`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Yellow (#C9C47A):** Secondary buttons, seen 3 times. Token `secondary`.
- **Dark Yellow (#6B6820):** Accent in text, fills and borders, seen 30 times. Token `tertiary`.

## Typography

**Ahrefs** and **Inter** share the interface. Fallback stack: `Ahrefs, sans-serif`.

- **display-hero:** Ahrefs 64px at weight 400, line height 0.94 (40px on mobile). Oversized hero statements.
- **headline-display:** Ahrefs 60px at weight 400, line height 0.95 (41px on mobile). Page title (h1).
- **headline-lg:** Ahrefs 48px at weight 400, line height 1. Section headings (h2).
- **headline-md:** Ahrefs 32px at weight 400, line height 1.06 (24px on mobile). Sub-section headings.
- **headline-sm:** Ahrefs 24px at weight 400, line height 1.08. Card and feature titles.
- **body-md:** Ahrefs 20px at weight 400, line height 1.2. Body text.
- **body-sm:** Ahrefs 16px at weight 400, line height 1.25. Secondary and small text.
- **label-md:** Inter 18px at weight 400, line height 1.61. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (71% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 24px, xl 40px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 720px, 767px, 768px, 769px, 1200px, 1279px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF4D borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (4px):** 56 elements.
- **full (9999px):** 48 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up for Ahrefs”):** #FF8D00 fill, #FFFFFF text, 18px/400, 5px radius, padding 17px 32px.
- **button-secondary (“Get Started”):** #C9C47A fill, #000000 text, 18px/400, 3px radius, padding 4px 12px.
- **button-outline (“Sign up”):** transparent fill, #FFFFFF text, 20px/400, 4px radius, padding 7px 16px, border 2px solid #FFFFFF4D.
- **button-ghost (“Sign up”):** transparent fill, #FFFFFF text, 20px/400, 4px radius, padding 7px 16px, border 2px solid #FFFFFF4D.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #3A57FC for the page.
- Do keep text in 3 levels: #FFFFFF, #000000, #C4CDFE.
- Do reserve #FF8D00 for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #000000 for body text; it reaches 3.95:1 on #3A57FC. Keep it for large text or metadata.
- Don't use #C4CDFE for body text; it reaches 3.42:1 on #3A57FC. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Ahrefs and Inter.
- Don't use #FF8D00 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ahrefs.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

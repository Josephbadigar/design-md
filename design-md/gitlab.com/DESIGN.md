---
version: alpha
name: GitLab
description: "Dark interface measured from about.gitlab.com: GitLab Sans type, red accents, flat surfaces and 4px corners."
colors:
  background: "#171321"
  surface: "#171321"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F7F7F5"
  on-surface-muted: "#A2A1A6"
  on-surface-subtle: "#74717A"
  overlay: "#FFFFFF26"
  overlay-strong: "#FFFFFF1A"
  outline: "#45424D"
  outline-variant: "#FFFFFF33"
  primary: "#E24329"
  on-primary: "#000000"
  secondary: "#FC6D26"
typography:
  headline-display:
    fontFamily: GitLab Sans
    fontSize: 96px
    fontWeight: 660
    lineHeight: 1.04
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: GitLab Sans
    fontSize: 64px
    fontWeight: 660
    lineHeight: 1.06
    letterSpacing: -0.03em
  headline-md:
    fontFamily: GitLab Sans
    fontSize: 32px
    fontWeight: 580
    lineHeight: 1.13
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: GitLab Sans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.02em
  body-md:
    fontFamily: GitLab Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  body-lg:
    fontFamily: GitLab Sans
    fontSize: 18px
    fontWeight: 660
    lineHeight: 1.56
  label-md:
    fontFamily: GitLab Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: GitLab Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  headline-display-mobile:
    fontFamily: GitLab Sans
    fontSize: 48px
    fontWeight: 660
    lineHeight: 1.04
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: GitLab Sans
    fontSize: 48px
    fontWeight: 660
    lineHeight: 1.06
    letterSpacing: -0.03em
rounded:
  sm: 4px
  md: 120px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 96px
  margin: 48px
components:
  button-primary:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 24px
    height: 72px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 11px 16px
    height: 47px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  card:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 24px
  link:
    textColor: "{colors.on-surface}"
---

# GitLab Design System

## Overview

GitLab describes itself as: “Teams and agents ship trusted software faster with GitLab, the intelligent orchestration platform with context and governance for the entire software lifecycle.” The interface is dark, built on **Cool Charcoal (#171321)** with **White (#FFFFFF)** text, and **Red (#E24329)** as the main accent.

Type is set in **GitLab Sans**, with **GitLab Mono** for code. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [about.gitlab.com](https://about.gitlab.com/) on October 29, 2026 at 1440×900 and 390×844 from 385 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #E53C97, #7759C2, #FC6D26.

- **Cool Charcoal (#171321):** Page background, seen 15 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 96 times. Token `on-surface`.
- **Snow (#F7F7F5):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Gray (#A2A1A6):** Muted text and metadata, seen 12 times. Token `on-surface-muted`.
- **Cool Slate (#74717A):** Subtle text and placeholders, seen 12 times. Token `on-surface-subtle`.
- **White 15% (#FFFFFF26):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Cool Graphite (#45424D):** Borders and dividers, seen 6 times. Token `outline`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Red (#E24329):** Brand color in the logo, seen 2 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#FC6D26):** Accent in the logo, seen 4 times. Token `secondary`.

## Typography

**GitLab Sans** and **GitLab Mono** (monospace) share the interface. Fallback stack: `GitLab Sans, sans-serif`.

- **headline-display:** GitLab Sans 96px at weight 660, line height 1.04, tracking -0.03em (48px on mobile). Page title (h1).
- **headline-lg:** GitLab Sans 64px at weight 660, line height 1.06, tracking -0.03em (48px on mobile). Section headings (h2).
- **headline-md:** GitLab Sans 32px at weight 580, line height 1.13, tracking -0.02em. Sub-section headings.
- **headline-sm:** GitLab Sans 24px at weight 400, line height 1.33, tracking -0.02em. Card and feature titles.
- **body-md:** GitLab Sans 14px at weight 400, line height 1.2. Body text.
- **body-lg:** GitLab Sans 18px at weight 660, line height 1.56. Lead paragraphs.
- **label-md:** GitLab Sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** GitLab Mono 14px at weight 400, line height 1.71. Code and technical values.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 375px, 500px, 576px, 768px, 769px, 1025px, 1200px, 1220px, 1300px, 1440px, 1550px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #45424D borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 60 elements.
- **md (120px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try for free”):** transparent fill, #FFFFFF text, 18px/580, padding 24px, border 1px solid #FFFFFF33.
- **button-secondary (“Get free trial”):** #FFFFFF fill, #171321 text, 18px/660, 4px radius, padding 11px 16px, border 1px solid #FFFFFF.
- **button-ghost (“Platform”):** transparent fill, #FFFFFF text, 16px/400, 4px radius, padding 0px.
- **card:** #FFFFFF1A fill, #171321 text, 16px/400, padding 24px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #171321 for the page.
- Do keep text in 4 levels: #FFFFFF, #F7F7F5, #A2A1A6, #74717A.
- Do use #E24329 as the brand accent: header, logo and key highlights.
- Do set headlines in GitLab Sans with tight tracking (-0.03em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 120px.
- Don't use #74717A for body text; it reaches 3.81:1 on #171321. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond GitLab Sans and GitLab Mono.
- Don't use #E24329 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.18s, 0.3s, 0.2s, 0.1s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.7, 0, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gitlab.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).

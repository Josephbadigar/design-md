---
version: alpha
name: GitHub
description: "Dark interface measured from github.com: Mona Sans type with Mona Sans VF, deep indigo accents, tonal surfaces and 6px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#A4AEA6"
  surface-container-low: "#090D0A"
  surface-container: "#0D1117"
  surface-container-high: "#0F1511"
  overlay: "#FFFFFF1F"
  overlay-strong: "#1F232866"
  outline: "#21262D"
  outline-variant: "#191F1B"
  primary: "#080A3D"
  on-primary: "#FFFFFF"
  secondary: "#5FED83"
  tertiary: "#A2DAFF"
  success: "#08872B"
typography:
  headline-display:
    fontFamily: Mona Sans
    fontSize: 64px
    fontWeight: 425
    lineHeight: 1.08
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Mona Sans
    fontSize: 40px
    fontWeight: 460
    lineHeight: 1.2
  headline-md:
    fontFamily: Mona Sans VF
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.5
  headline-sm:
    fontFamily: Mona Sans
    fontSize: 22px
    fontWeight: 480
    lineHeight: 1.4
  body-md:
    fontFamily: Mona Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Mona Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Mona Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.015em
  label-sm:
    fontFamily: Mona Sans VF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: Mona Sans Mono
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Mona Sans
    fontSize: 40px
    fontWeight: 440
    lineHeight: 1.15
  headline-sm-mobile:
    fontFamily: Mona Sans
    fontSize: 20px
    fontWeight: 480
    lineHeight: 1.4
rounded:
  sm: 6px
  md: 8px
  lg: 48px
  xl: 60px
spacing:
  xs: 2.1px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 12px
  section: 72px
components:
  button-primary:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 6px 20px
    height: 48px
  button-primary-hover:
    backgroundColor: "#077124"
  button-outline:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.tertiary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 6px 20px
    height: 56px
  button-outline-hover:
    backgroundColor: "#4D566166"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 1px 12px
    height: 32px
  input-field:
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 18px 12px 0px 18px
  link:
    textColor: "{colors.on-surface}"
---

# GitHub Design System

## Overview

GitHub describes itself as: “Join the world's most widely adopted, AI-powered developer platform where millions of developers, businesses, and the largest open source community build software that advances humanity.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Deep Indigo (#080A3D)** as the main accent.

Type is set in **Mona Sans** and **Mona Sans VF**, with **Mona Sans Mono** for code. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 6px.

Measured from [github.com](https://github.com/) on October 21, 2026 at 1440×900 and 390×844 from 422 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #000240.

- **Near Black (#000000):** Page background. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 46 times. Token `on-surface`, CSS `--brand-Tabs-item-underline-rest`.
- **Gray (#A4AEA6):** Secondary text, seen 29 times. Token `on-surface-variant`, CSS `--brand-color-text-muted`.
- **Near Black (#090D0A):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Charcoal (#0D1117):** Cards and panels, seen 3 times. Token `surface-container`.
- **Charcoal (#0F1511):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White 12% (#FFFFFF1F):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Cool Charcoal 40% (#1F232866):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Graphite (#21262D):** Borders and dividers, seen 10 times. Token `outline`.
- **Charcoal (#191F1B):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Deep Indigo (#080A3D):** Brand color in logos and imagery. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Green (#5FED83):** Brand accent (CSS variable), seen 20 times. Token `secondary`, CSS `--brand-Label-color-green-blue-start`.
- **Light Blue (#A2DAFF):** Most used accent color, seen 15 times. Token `tertiary`.
- **Dark Green (#08872B):** Success and positive states, seen 2 times. Token `success`.

## Typography

**Mona Sans**, **Mona Sans VF** and **Mona Sans Mono** (monospace) share the interface. Fallback stack: `Mona Sans, MonaSansFallback, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Mona Sans 64px at weight 425, line height 1.08, tracking -0.035em (40px on mobile). Page title (h1).
- **headline-lg:** Mona Sans 40px at weight 460, line height 1.2. Section headings (h2).
- **headline-md:** Mona Sans VF 24px at weight 600, line height 1.5. Sub-section headings.
- **headline-sm:** Mona Sans 22px at weight 480, line height 1.4 (20px on mobile). Card and feature titles.
- **body-md:** Mona Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Mona Sans 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Mona Sans 16px at weight 500, line height 1.5, tracking 0.015em. Buttons, navigation and labels.
- **label-sm:** Mona Sans VF 14px at weight 400, line height 1.5. Small labels and badges.
- **code:** Mona Sans Mono 12px at weight 500, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (74% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.1px, sm 8px, md 12px, lg 20px, xl 48px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#090D0A → #0D1117 → #0F1511) and #21262D borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 32 elements.
- **xl (60px):** 32 elements.
- **md (8px):** 4 elements.
- **lg (48px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up for GitHub”):** #08872B fill, #FFFFFF text, 14px/400, 6px radius, padding 6px 20px.
- **button-primary-hover:** background #077124, text #FFFFFF on hover.
- **button-outline (“Download GitHub Copilot app”):** #1F232866 fill, #A2DAFF text, 14px/400, 6px radius, padding 6px 20px, border 1px solid #FFFFFF.
- **button-outline-hover:** background #4D566166, text #A2DAFF on hover.
- **button-ghost (“Search /”):** transparent fill, #FFFFFF text, 16px/400, 6px radius, padding 1px 12px, border 1px solid #262C28.
- **input-field (“you@domain.com”):** transparent fill, #000000 text, 16px/400, 8px radius, padding 18px 12px 0px 18px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #090D0A, #0D1117, #0F1511.
- Do keep text in 2 levels: #FFFFFF, #A4AEA6.
- Do use #080A3D as the brand accent: header, logo and key highlights.
- Do set headlines in Mona Sans with tight tracking (-0.035em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 6px corners on most elements; larger surfaces also use 60px, 8px and 48px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Mona Sans, Mona Sans VF and Mona Sans Mono.
- Don't use #080A3D for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/github.com/), the free DESIGN.md generator.

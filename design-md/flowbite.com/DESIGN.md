---
version: alpha
name: Flowbite
description: "Light interface measured from flowbite.com: Inter type, blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#111827"
  on-background: "#111827"
  on-surface-variant: "#6B7280"
  on-surface-muted: "#9CA3AF"
  surface-container-low: "#F9FAFB"
  surface-container: "#F3F4F6"
  surface-container-high: "#E1EFFE"
  outline: "#F3F4F6"
  outline-variant: "#E5E7EB"
  primary: "#1A56DB"
  on-primary: "#FFFFFF"
  secondary: "#5468FF"
  tertiary: "#CC0000"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 60px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.11
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  sm: 6px
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  gutter: 8px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 10px 20px
    height: 40px
  button-primary-hover:
    backgroundColor: "#1E429F"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 8px 8px 16px
    height: 40px
  button-outline-hover:
    backgroundColor: "{colors.surface-container}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 24px
    height: 46px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 12px
    padding: 16px 12px 16px 44px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 20px
  link:
    textColor: "#4B5563"
---

# Flowbite Design System

## Overview

Flowbite describes itself as: “Get started with an open-source library of over 600+ UI components, sections, and pages built with the utility classes from Tailwind CSS and designed in Figma.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#111827)** text, and **Blue (#1A56DB)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [flowbite.com](https://flowbite.com/) on November 4, 2026 at 1440×900 and 390×844 from 436 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 87 times. Token `background`, CSS `--docsearch-footer-background`.
- **Deep Blue (#111827):** Primary text and headings, seen 107 times. Token `on-surface`.
- **Cool Slate (#6B7280):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Blue (#9CA3AF):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Snow (#F9FAFB):** Raised areas one step from the page, seen 12 times. Token `surface-container-low`.
- **Snow (#F3F4F6):** Cards and panels, seen 1 time. Token `surface-container`.
- **Pale Blue (#E1EFFE):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Snow (#F3F4F6):** Borders and dividers, seen 60 times. Token `outline`.
- **Cool Mist (#E5E7EB):** Secondary dividers, seen 31 times. Token `outline-variant`.
- **Blue (#1A56DB):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#5468FF):** Accent (CSS variable). Token `secondary`.
- **Red (#CC0000):** Accent, seen 6 times. Token `tertiary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, ui-sans-serif, system-ui, -apple-system`.

- **headline-display:** Inter 60px at weight 800, line height 1, tracking -0.025em (36px on mobile). Page title (h1).
- **headline-lg:** Inter 36px at weight 800, line height 1.11 (16px on mobile). Section headings (h2).
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 20px at weight 600, line height 1.4. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Inter 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 1024px, 1280px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 336 elements.
- **sm (6px):** 12 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign in”):** #1A56DB fill, #FFFFFF text, 14px/500, 8px radius, padding 10px 20px.
- **button-primary-hover:** background #1E429F, text #FFFFFF on hover.
- **button-outline (“Search K”):** #F9FAFB fill, #6B7280 text, 16px/500, 8px radius, padding 8px 8px 8px 16px, border 1px solid #D1D5DB, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-outline-hover:** background #F3F4F6, text #6B7280 on hover.
- **button-ghost (“Explore components”):** transparent fill, #111827 text, 16px/500, 8px radius, padding 10px 24px, border 1px solid #E5E7EB.
- **input-field (“Enter your email”):** #FFFFFF fill, #111827 text, 16px/400, 12px 0px 0px 12px radius, padding 16px 12px 16px 44px, border 1px solid #E5E7EB.
- **card:** #F9FAFB fill, #000000 text, 16px/400, 6px 6px 0px 0px radius, padding 10px 20px.
- **link:** transparent fill, #4B5563 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9FAFB, #F3F4F6, #E1EFFE.
- Do keep text in 3 levels: #111827, #6B7280, #9CA3AF.
- Do reserve #1A56DB for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 6px.
- Don't use #9CA3AF for body text; it reaches 2.54:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter.
- Don't use #1A56DB for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/flowbite.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

---
version: alpha
name: Netlify
description: "Dark interface measured from netlify.com: Figtree type with Instrument Sans, cyan accents, tonal surfaces and 4px corners."
colors:
  background: "#12181F"
  surface: "#12181F"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#DEFFFE"
  on-surface-muted: "#E4F0FB"
  on-surface-subtle: "#545A61"
  surface-container-low: "#181A1C"
  overlay: "#E9EBED1A"
  overlay-strong: "#FFFFFF19"
  outline: "#FFFFFF33"
  primary: "#32E6E2"
  on-primary: "#181A1C"
  secondary: "#014847"
  tertiary: "#89DDFF"
typography:
  headline-display:
    fontFamily: Figtree
    fontSize: 64px
    fontWeight: 800
    lineHeight: 1.1
  headline-lg:
    fontFamily: Figtree
    fontSize: 32px
    fontWeight: 800
    lineHeight: 1.1
  headline-md:
    fontFamily: Figtree
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
  body-md:
    fontFamily: Instrument Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Figtree
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.1
  label-md:
    fontFamily: Instrument Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Instrument Sans
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.5
  code:
    fontFamily: Martian Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Figtree
    fontSize: 41px
    fontWeight: 800
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Figtree
    fontSize: 24px
    fontWeight: 800
    lineHeight: 1.1
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 360px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 12px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 10px 17px
    height: 40px
  button-primary-hover:
    backgroundColor: "#8EFBF7"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 10px 17px
    height: 40px
  button-secondary-hover:
    backgroundColor: "#8EFBF7"
  button-ghost:
    textColor: "#353A3E"
    typography: "{typography.label-md}"
    padding: 4px
  input-field:
    backgroundColor: "{colors.on-surface}"
    textColor: "#353A3E"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "#353A3E"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 24px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# Netlify Design System

## Overview

Netlify describes itself as: “Create with AI or code, deploy instantly on production infrastructure. One platform to build and ship.” The interface is dark, built on **Cool Charcoal (#12181F)** with **White (#FFFFFF)** text, and **Cyan (#32E6E2)** as the main accent.

Type is set in **Figtree** and **Instrument Sans**, with **Martian Mono** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [netlify.com](https://www.netlify.com/) on October 29, 2026 at 1440×900 and 390×844 from 390 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Cool Charcoal (#12181F):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 18 times. Token `on-surface`, CSS `--table-bg`.
- **Pale Cyan (#DEFFFE):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Pale Blue (#E4F0FB):** Muted text and metadata, seen 14 times. Token `on-surface-muted`.
- **Cool Slate (#545A61):** Subtle text and placeholders, seen 36 times. Token `on-surface-subtle`.
- **Charcoal (#181A1C):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--ntl-button-primary-text-color`.
- **Mist 10% (#E9EBED1A):** Translucent fill for cards and controls, seen 10 times. Token `overlay`.
- **White 10% (#FFFFFF19):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 10 times. Token `outline`.
- **Cyan (#32E6E2):** Primary buttons and calls to action, seen 19 times. Token `primary`, CSS `--ntl-button-primary-bg-color`.
- **Charcoal (#181A1C):** Text and icons on primary. Token `on-primary`.
- **Deep Cyan (#014847):** Accent in the logo, seen 8 times. Token `secondary`.
- **Light Cyan (#89DDFF):** Accent in text, fills and borders, seen 29 times. Token `tertiary`.

## Typography

**Figtree**, **Instrument Sans** and **Martian Mono** (monospace) share the interface. Fallback stack: `Figtree, system-ui, Helvetica, sans-serif`.

- **headline-display:** Figtree 64px at weight 800, line height 1.1 (41px on mobile). Page title (h1).
- **headline-lg:** Figtree 32px at weight 800, line height 1.1 (24px on mobile). Section headings (h2).
- **headline-md:** Figtree 24px at weight 700, line height 1.1. Sub-section headings.
- **body-md:** Instrument Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Figtree 18px at weight 600, line height 1.1. Lead paragraphs.
- **label-md:** Instrument Sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Instrument Sans 13px at weight 700, line height 1.5. Small labels and badges.
- **code:** Martian Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.25) 0px 4px 12px 0px`
- `rgba(51, 55, 59, 0.08) 0px 2px 4px 0px, rgba(51, 55, 59, 0.06) 0px 1px 10px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 94 elements.
- **xl (360px):** 28 elements.
- **lg (6px):** 16 elements.
- **full (9999px):** 16 elements.
- **sm (2px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #32E6E2 fill, #181A1C text, 16px/700, 360px radius, padding 10px 17px, border 2px solid #32E6E2.
- **button-primary-hover:** background #8EFBF7, text #181A1C on hover.
- **button-secondary (“Start building”):** #32E6E2 fill, #12181F text, 16px/700, 360px radius, padding 10px 17px, border 2px solid #32E6E2.
- **button-secondary-hover:** background #8EFBF7, text #12181F on hover.
- **button-ghost (“Toggle platform submenu”):** transparent fill, #353A3E text, 16px/400, 50% radius, padding 4px.
- **input-field:** #FFFFFF fill, #353A3E text, 16px/400, 4px radius, padding 8px, border 1px solid #778089.
- **card:** #FFFFFF fill, #353A3E text, 16px/400, 6px radius, padding 24px, border 1px solid #E9EBED.
- **link:** transparent fill, #545A61 text, padding 0px.

## Do's and Don'ts

- Do use #12181F for the page and lift surfaces in small steps: #181A1C.
- Do keep text in 4 levels: #FFFFFF, #DEFFFE, #E4F0FB, #545A61.
- Do reserve #32E6E2 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 360px, 6px and 2px.
- Don't use #545A61 for body text; it reaches 2.56:1 on #12181F. Keep it for large text or metadata.
- Don't introduce new font families beyond Figtree, Instrument Sans and Martian Mono.
- Don't use #32E6E2 for large backgrounds or body text.
- Don't make interface transitions slower than 0.45s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.45s, 0.15s.

- **Easing:** `cubic-bezier(0.33, 1, 0.68, 1)`, `cubic-bezier(0.22, 1, 0.36, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/netlify.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).

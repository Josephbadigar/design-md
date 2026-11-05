---
version: alpha
name: Sunsama
description: "Light interface measured from sunsama.com: DM Sans type, vivid orange accents, tonal surfaces and 10px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#202228"
  on-background: "#202228"
  on-surface-variant: "#4C4F56"
  on-surface-muted: "#797A7E"
  surface-container-low: "#FAFAFA"
  surface-container: "#F6F5F1"
  outline: "#EBEFF7"
  outline-variant: "#F2F2F2"
  primary: "#FF891C"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: DM Sans
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.16
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: DM Sans
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: DM Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: DM Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.16
    letterSpacing: -0.01em
  body-md:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: DM Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.48
    letterSpacing: -0.01em
  body-sm:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.48
    letterSpacing: -0.01em
  label-md:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.24
    letterSpacing: -0.01em
  label-sm:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.48
    letterSpacing: -0.01em
rounded:
  xs: 10px
  sm: 16px
  md: 24px
  lg: 30px
  xl: 50px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 20px
  xl: 44px
  gutter: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 10px 22px
    height: 44px
  button-primary-hover:
    backgroundColor: "#DB7414"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 11px
    padding: 0px
    height: 45px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-lg}"
    rounded: 20px
    padding: 6px 12px
    height: 30px
  input-field:
    textColor: "#333333"
    typography: "{typography.body-sm}"
    rounded: 20px
    padding: 8px 12px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xs}"
    padding: 32px 20px 0px 20px
  link:
    textColor: "{colors.primary}"
---

# Sunsama Design System

## Overview

Sunsama describes itself as: “The digital daily planner that helps you feel calm and stay focused.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#202228)** text, and **Vivid Orange (#FF891C)** as the main accent.

Type is set in **DM Sans**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 10px.

Measured from [sunsama.com](https://www.sunsama.com/) on November 4, 2026 at 1440×900 and 390×844 from 176 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #F06351, #F59549, #FF891C, #378FE9.

- **White (#FFFFFF):** Page background, seen 32 times. Token `background`.
- **Cool Graphite (#202228):** Primary text and headings, seen 45 times. Token `on-surface`, CSS `--black-2`.
- **Cool Slate (#4C4F56):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Slate (#797A7E):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 20 times. Token `surface-container-low`, CSS `--bg-light-grey-new`.
- **Mist (#F6F5F1):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--bg-secondary-new`.
- **Cool Mist (#EBEFF7):** Borders and dividers, seen 27 times. Token `outline`.
- **Mist (#F2F2F2):** Secondary dividers, seen 9 times. Token `outline-variant`, CSS `--border-new`.
- **Vivid Orange (#FF891C):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--ss-orange`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**DM Sans** carries the whole interface. Fallback stack: `DM Sans, sans-serif`.

- **headline-display:** DM Sans 48px at weight 600, line height 1.16, tracking -0.01em. Page title (h1).
- **headline-lg:** DM Sans 40px at weight 600, line height 1.1, tracking -0.01em. Section headings (h2).
- **headline-md:** DM Sans 24px at weight 500, line height 1.1, tracking -0.01em. Sub-section headings.
- **headline-sm:** DM Sans 20px at weight 600, line height 1.16, tracking -0.01em. Card and feature titles.
- **body-md:** DM Sans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** DM Sans 18px at weight 400, line height 1.48, tracking -0.01em. Lead paragraphs.
- **body-sm:** DM Sans 14px at weight 400, line height 1.48, tracking -0.01em. Secondary and small text.
- **label-md:** DM Sans 16px at weight 500, line height 1.24, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** DM Sans 14px at weight 500, line height 1.48, tracking -0.01em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 20px, xl 44px.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 576px, 767px, 768px, 991px, 1280px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(61, 71, 83, 0.05) 0px 0px 0px 0px, rgba(61, 71, 83, 0.05) 0px 1px 0px 0px, rgba(61, 71, 83, 0.08) 0px 2px 4px 0px`

## Shapes

Most elements use 10px corners. Measured radii, most used first:

- **xs (10px):** 120 elements.
- **lg (30px):** 32 elements.
- **xl (50px):** 28 elements.
- **md (24px):** 24 elements.
- **sm (16px):** 20 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for Free”):** #FF891C fill, #FFFFFF text, 16px/400, 30px radius, padding 10px 22px.
- **button-primary-hover:** background #DB7414, text #FFFFFF on hover.
- **button-outline (“Named Best Scheduling Tool by”):** #F6F5F1 fill, #202228 text, 16px/400, 11px radius, padding 0px.
- **button-ghost (“next slide”):** #F6F5F1 fill, #FFFFFF text, 40px/400, 20px radius, padding 6px 12px, border 1px solid #E5E4E0.
- **input-field (“Enter email”):** transparent fill, #333333 text, 14px/400, 20px radius, padding 8px 12px.
- **card:** #FAFAFA fill, #202228 text, 16px/400, 10px radius, padding 32px 20px 0px 20px, border 1px solid #F2F2F2.
- **link:** transparent fill, #FF891C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F6F5F1.
- Do keep text in 3 levels: #202228, #4C4F56, #797A7E.
- Do reserve #FF891C for primary actions and key highlights.
- Do set headlines in DM Sans with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do use 10px corners on most elements; larger surfaces also use 30px, 50px and 24px.
- Don't use #797A7E for body text; it reaches 4.29:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond DM Sans.
- Don't use #FF891C for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sunsama.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

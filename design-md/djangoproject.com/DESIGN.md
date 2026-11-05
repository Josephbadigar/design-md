---
version: alpha
name: Django
description: "Light interface measured from djangoproject.com: Roboto type, deep teal accents, tonal surfaces and 5px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0C3C26"
  on-background: "#0C3C26"
  on-surface-variant: "#859D94"
  surface-container-low: "#F1FFF7"
  surface-container: "#F8F8F8"
  outline: "#CFE3DC"
  outline-variant: "#44B78B"
  primary: "#0C4B33"
  on-primary: "#FFFFFF"
  secondary: "#2B8C67"
  success: "#20AA76"
typography:
  display-hero:
    fontFamily: Roboto
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.6
  headline-display:
    fontFamily: Roboto
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.031em
  headline-lg:
    fontFamily: Roboto
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.6
  body-md:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  body-lg:
    fontFamily: Roboto
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
  body-sm:
    fontFamily: Roboto
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.6
  label-lg:
    fontFamily: Roboto
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.2
  label-sm:
    fontFamily: Roboto
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.23
rounded:
  md: 5px
spacing:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 20px
  xl: 35px
  section: 50px
components:
  button-primary:
    backgroundColor: "{colors.outline-variant}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 18px 50px 19.8px 50px
    height: 61px
  button-primary-hover:
    backgroundColor: "#51BE95"
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 18px 27px
    height: 67px
  button-outline-hover:
    textColor: "{colors.success}"
  button-ghost:
    textColor: "{colors.outline-variant}"
    typography: "{typography.label-md}"
    rounded: 4px
    padding: 0px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 4px
    padding: 6px 39.41px 8px 10px
  link:
    textColor: "{colors.surface-container-low}"
---

# Django Design System

## Overview

The interface is light, built on **White (#FFFFFF)** with **Deep Teal (#0C3C26)** text, and **Deep Teal (#0C4B33)** as the main accent.

Type is set in **Roboto**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 5px.

Measured from [djangoproject.com](https://www.djangoproject.com/) on November 4, 2026 at 1440×900 and 390×844 from 177 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--white-color`.
- **Deep Teal (#0C3C26):** Primary text and headings, seen 21 times. Token `on-surface`, CSS `--table-color`.
- **Teal (#859D94):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--dark-hairline-color`.
- **Snow (#F1FFF7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--body-bg`.
- **Snow (#F8F8F8):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--sidebar-bg`.
- **Light Teal (#CFE3DC):** Borders and dividers, seen 13 times. Token `outline`, CSS `--hairline-color`.
- **Teal (#44B78B):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--primary`.
- **Deep Teal (#0C4B33):** Brand color in the header, seen 7 times. Token `primary`, CSS `--community-img-fg`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#2B8C67):** Accent (CSS variable), seen 7 times. Token `secondary`, CSS `--primary-accent`.
- **Teal (#20AA76):** Success and positive states, seen 36 times. Token `success`, CSS `--search-link`.

## Typography

**Roboto** carries the whole interface. Fallback stack: `Roboto, Corbel, Avenir, Lucida Grande`. Other loaded fonts: FontAwesome.

- **display-hero:** Roboto 40px at weight 700, line height 1.6. Oversized hero statements.
- **headline-display:** Roboto 32px at weight 400, line height 1.1, tracking -0.031em. Page title (h1).
- **headline-lg:** Roboto 24px at weight 400, line height 1.6. Section headings (h2).
- **body-md:** Roboto 14px at weight 400, line height 1.6. Body text.
- **body-lg:** Roboto 20px at weight 400, line height 1.2. Lead paragraphs.
- **body-sm:** Roboto 12px at weight 400, line height 1.6. Secondary and small text.
- **label-lg:** Roboto 18px at weight 400, line height 1.6. Large buttons and tabs.
- **label-md:** Roboto 16px at weight 700, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Roboto 13px at weight 700, line height 1.23. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 21% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 10px, lg 20px, xl 35px.
- **Sections:** 50px vertical padding between major sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(255, 255, 255) 0px 0px 0px 0px, rgb(255, 255, 255) 0px 0px 0px 0px, rgb(255, 255, 255) -460px 0px 0px 0px, rgb(255, 255, 255) -1000px 0px 0px 0px, rgb(255, 255, 255) 0px 600px 0px 0px, rgb(255, 255, 255) -460px 600px 0px 0px`

## Shapes

Most elements use 5px corners. Measured radii, most used first:

- **md (5px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started with Django”):** #44B78B fill, #FFFFFF text, 18px/700, 5px radius, padding 18px 50px 19.8px 50px.
- **button-primary-hover:** background #51BE95, text #FFFFFF on hover.
- **button-outline (“Learn more about Django”):** transparent fill, #859D94 text, 18px/400, 5px radius, padding 18px 27px, border 1px solid #CFE3DC.
- **button-outline-hover:** background #00000000, text #20AA76 on hover.
- **button-ghost (“Search”):** transparent fill, #44B78B text, 16px/400, 4px radius, padding 0px.
- **input-field (“Search (Ctrl+K)”):** #FFFFFF fill, #0C3C26 text, 16px/400, 4px radius, padding 6px 39.41px 8px 10px, border 1px solid #CFE3DC.
- **link:** transparent fill, #F1FFF7 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F1FFF7, #F8F8F8.
- Do keep text in 2 levels: #0C3C26, #859D94.
- Do use #0C4B33 as the brand accent: header, logo and key highlights.
- Do set headlines in Roboto with tight tracking (-0.031em).
- Do reuse the measured spacing steps (6px, 10px, 20px).
- Do use 5px corners on most elements.
- Don't use #859D94 for body text; it reaches 2.90:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Roboto.
- Don't use #0C4B33 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.5s, 0.3s.

- **Easing:** `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/djangoproject.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

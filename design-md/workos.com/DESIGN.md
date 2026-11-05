---
version: alpha
name: WorkOS
description: "Light interface measured from workos.com: Untitled Sans type, indigo accents, tonal surfaces and 100px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#29363D"
  on-background: "#29363D"
  on-surface-variant: "#656B8A"
  on-surface-muted: "#717AA8"
  surface-container-low: "#F9F9FB"
  outline: "#E8EAED"
  outline-variant: "#FFFFFF33"
  primary: "#6363F1"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#23F0C3"
  tertiary: "#D272FF"
typography:
  headline-display:
    fontFamily: Untitled Sans
    fontSize: 80px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.07em
  headline-lg:
    fontFamily: Untitled Sans
    fontSize: 52px
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: -0.05em
  headline-md:
    fontFamily: Untitled Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: Untitled Sans
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.05em
  title-lg:
    fontFamily: Untitled Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: Untitled Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
  body-lg:
    fontFamily: Untitled Sans
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.01em
  body-sm:
    fontFamily: Untitled Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Untitled Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
  label-sm:
    fontFamily: Untitled Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.2
  code:
    fontFamily: IBM Plex Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Untitled Sans
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.07em
  headline-sm-mobile:
    fontFamily: Untitled Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: Untitled Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.05em
rounded:
  sm: 4px
  md: 8px
  lg: 100px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 22px
  xl: 64px
  gutter: 12px
  section: 120px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 12px 24px
    height: 43px
  button-primary-hover:
    backgroundColor: "#7777F3"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 20px 8px 8px
    height: 66px
  button-outline-hover:
    backgroundColor: "#F3F4F7"
  button-ghost:
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 9.5px 20px
    height: 35px
  card:
    backgroundColor: "#181B39"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 18px
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# WorkOS Design System

## Overview

WorkOS describes itself as: “Developer APIs/SDKs for Enterprise Ready features like Single Sign-On, Directory Sync, Audit Logging, and more. Get started for free.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#29363D)** text, and **Indigo (#6363F1)** as the main accent.

Type is set in **Untitled Sans**, with **IBM Plex Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 100px.

Measured from [workos.com](https://workos.com/) on November 4, 2026 at 1440×900 and 390×844 from 433 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #25DFF9, #21FF94, #A683FF, #7772E5.

- **White (#FFFFFF):** Page background, seen 12 times. Token `background`, CSS `--um-input-bg-active`.
- **Deep Blue (#29363D):** Primary text and headings, seen 46 times. Token `on-surface`, CSS `--light-1`.
- **Indigo (#656B8A):** Secondary text, seen 38 times. Token `on-surface-variant`, CSS `--foreground-light-2`.
- **Indigo (#717AA8):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Snow (#F9F9FB):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`, CSS `--um-input-bg`.
- **Mist (#E8EAED):** Borders and dividers, seen 35 times. Token `outline`, CSS `--border-color`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Indigo (#6363F1):** Primary buttons and calls to action, seen 16 times. Token `primary`, CSS `--brand-purple`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Vivid Teal (#23F0C3):** Accent (CSS variable), seen 12 times. Token `secondary`, CSS `--dark-accent`.
- **Light Violet (#D272FF):** Accent in text, fills and borders, seen 18 times. Token `tertiary`.

## Typography

**Untitled Sans** and **IBM Plex Mono** (monospace) share the interface. Fallback stack: `Untitled Sans, Untitled Fallback, Arial, sans-serif`.

- **headline-display:** Untitled Sans 80px at weight 500, line height 1.05, tracking -0.07em (42px on mobile). Page title (h1).
- **headline-lg:** Untitled Sans 52px at weight 500, line height 1.07, tracking -0.05em (32px on mobile). Section headings (h2).
- **headline-md:** Untitled Sans 32px at weight 500, line height 1.2, tracking -0.04em. Sub-section headings.
- **headline-sm:** Untitled Sans 28px at weight 500, line height 1.2, tracking -0.05em (20px on mobile). Card and feature titles.
- **title-lg:** Untitled Sans 20px at weight 500, line height 1.2, tracking -0.01em. Small titles.
- **body-md:** Untitled Sans 16px at weight 400, line height 1.2. Body text.
- **body-lg:** Untitled Sans 19px at weight 400, line height 1.6, tracking -0.01em. Lead paragraphs.
- **body-sm:** Untitled Sans 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Untitled Sans 16px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Untitled Sans 14px at weight 500, line height 1.2. Small labels and badges.
- **code:** IBM Plex Mono 14px at weight 400, line height 1.2. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (71% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 12px, lg 22px, xl 64px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 480px, 767px, 768px, 991px, 992px, 1090px, 1100px, 1140px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(17, 7, 53, 0.05) 0px 51px 78px 0px, rgba(17, 7, 53, 0.035) 0px 21.3066px 35.4944px 0px, rgba(17, 7, 53, 0.03) 0px 11.3915px 18.9418px 0px, rgba(17, 7, 53, 0.024) 0px 6.38599px 9.8801px 0px, rgba(17, 7, 53, 0.02) 0px 3.39155px 4.58665px 0px, rgba(17, 7, 53, 0.016) 0px 1.4113px 1.55262px 0px, rgba(41, 56, 78, 0.05) 0px 1px 0px 0px inset`
- `rgba(23, 6, 100, 0.035) 0px 24px 22px 0px, rgba(23, 6, 100, 0.055) 0px 8.5846px 8.03036px 0px, rgba(23, 6, 100, 0.067) 0px 4.77692px 3.89859px 0px, rgba(23, 6, 100, 0.082) 0px 2.63479px 1.91116px 0px, rgba(23, 6, 100, 0.12) 0px 1.15891px 0.755676px 0px`
- `rgba(3, 3, 6, 0.07) 0px 100px 80px 0px, rgba(3, 3, 6, 0.05) 0px 41.7776px 33.4221px 0px, rgba(3, 3, 6, 0.043) 0px 22.3363px 17.869px 0px, rgba(3, 3, 6, 0.035) 0px 12.5216px 10.0172px 0px, rgba(3, 3, 6, 0.027) 0px 6.6501px 5.32008px 0px, rgba(3, 3, 6, 0.02) 0px 2.76726px 2.21381px 0px`

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 160 elements.
- **md (8px):** 56 elements.
- **full (9999px):** 40 elements.
- **sm (4px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #6363F1 fill, #FFFFFF text, 16px/500, 100px radius, padding 12px 24px, shadow `rgba(23, 6, 100, 0.035) 0px 24px 22px 0px, rgba(23, 6, 100, 0.055) 0px 8.5846px 8.03036px 0px, rgba(23, 6, 100, 0.067) 0px 4.77692px 3.89859px 0px, rgba(23, 6, 100, 0.082) 0px 2.63479px 1.91116px 0px, rgba(23, 6, 100, 0.12) 0px 1.15891px 0.755676px 0px`.
- **button-primary-hover:** background #7777F3, text #FFFFFF on hover.
- **button-outline (“Passport”):** #F9F9FB fill, #29363D text, 16px/500, 8px radius, padding 8px 20px 8px 8px, border 1px solid #E7E8EC.
- **button-outline-hover:** background #F3F4F7, text #29363D on hover.
- **button-ghost (“Sign in”):** transparent fill, #6363F1 text, 14px/400, 100px radius, padding 9.5px 20px, border 1px solid #E8EAED.
- **card:** #181B39 fill, #FFFFFF text, 16px/400, 18px radius, padding 0px, shadow `rgba(3, 3, 6, 0.07) 0px 100px 80px 0px, rgba(3, 3, 6, 0.05) 0px 41.7776px 33.4221px 0px, rgba(3, 3, 6, 0.043) 0px 22.3363px 17.869px 0px, rgba(3, 3, 6, 0.035) 0px 12.5216px 10.0172px 0px, rgba(3, 3, 6, 0.027) 0px 6.6501px 5.32008px 0px, rgba(3, 3, 6, 0.02) 0px 2.76726px 2.21381px 0px`.
- **link:** transparent fill, #6363F1 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9F9FB.
- Do keep text in 3 levels: #29363D, #656B8A, #717AA8.
- Do reserve #6363F1 for primary actions and key highlights.
- Do set headlines in Untitled Sans with tight tracking (-0.07em).
- Do reuse the measured spacing steps (8px, 12px, 22px).
- Do use 100px corners on most elements; larger surfaces also use 8px and 4px.
- Don't use #717AA8 for body text; it reaches 4.16:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Untitled Sans and IBM Plex Mono.
- Don't use #6363F1 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/workos.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

---
version: alpha
name: Auth0
description: "Dark monochrome interface measured from auth0.com: Aeonik type, tonal surfaces and 4px corners."
colors:
  background: "#20003A"
  surface: "#20003A"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E5E5E5"
  on-surface-muted: "#EBD3FF"
  on-surface-subtle: "#C5C5C5"
  surface-container-low: "#120021"
  overlay: "#FFFFFF40"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#BCBAFF"
typography:
  headline-display:
    fontFamily: Aeonik
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.016em
  headline-lg:
    fontFamily: Aeonik
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.17
    letterSpacing: -0.021em
  headline-md:
    fontFamily: Aeonik
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.38
  headline-sm:
    fontFamily: Aeonik
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
  title-lg:
    fontFamily: Aeonik
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: Aeonik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0.013em
  body-lg:
    fontFamily: Aeonik
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.56
    letterSpacing: 0.007em
  label-md:
    fontFamily: Aeonik
    fontSize: 16px
    fontWeight: 500
    lineHeight: 2
    letterSpacing: 0.013em
  label-sm:
    fontFamily: Aeonik
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
  code:
    fontFamily: Aeonik Mono
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0.107em
  headline-display-mobile:
    fontFamily: Aeonik
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.27
  headline-lg-mobile:
    fontFamily: Aeonik
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.38
  title-lg-mobile:
    fontFamily: Aeonik
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 96px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 8px
  section: 106px
  margin: 96px
  container: 1728px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xs}"
    padding: 7px 24px
    height: 40px
  button-secondary:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xs}"
    padding: 7px 24px
    height: 40px
  button-outline:
    textColor: "#FFFEFA"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xs}"
    padding: 8px 12px 8px 16px
    height: 38px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 24px 0px
  input-field:
    textColor: "#FFFEFA"
    typography: "{typography.code}"
    rounded: 0px
    padding: 0px 16px 0px 20px
  card:
    textColor: "#FFFEFA"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 64px
  link:
    textColor: "{colors.primary}"
---

# Auth0 Design System

## Overview

Auth0 describes itself as: “Secure users, AI agents, and more with Auth0, an easy-to-implement, scalable, and adaptable authentication and authorization platform.” The interface is dark, built on **Deep Violet (#20003A)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Aeonik**, with **Aeonik Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [auth0.com](https://auth0.com/) on October 21, 2026 at 1440×900 and 390×844 from 377 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #490186, #9921FE, #FF6217.

- **Deep Violet (#20003A):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 101 times. Token `on-surface`.
- **Mist (#E5E5E5):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Pale Violet (#EBD3FF):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Silver (#C5C5C5):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **Deep Violet (#120021):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **White 25% (#FFFFFF40):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 123 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Pale Indigo (#BCBAFF):** Accent, seen 2 times. Token `secondary`.

## Typography

**Aeonik** and **Aeonik Mono** (monospace) share the interface. Fallback stack: `Aeonik, sans-serif`.

- **headline-display:** Aeonik 64px at weight 400, line height 1.13, tracking -0.016em (44px on mobile). Page title (h1).
- **headline-lg:** Aeonik 48px at weight 400, line height 1.17, tracking -0.021em (32px on mobile). Section headings (h2).
- **headline-md:** Aeonik 32px at weight 400, line height 1.38. Sub-section headings.
- **headline-sm:** Aeonik 24px at weight 400, line height 1.5. Card and feature titles.
- **title-lg:** Aeonik 20px at weight 400, line height 1.4 (24px on mobile). Small titles.
- **body-md:** Aeonik 16px at weight 400, line height 1.38, tracking 0.013em. Body text.
- **body-lg:** Aeonik 18px at weight 500, line height 1.56, tracking 0.007em. Lead paragraphs.
- **label-md:** Aeonik 16px at weight 500, line height 2, tracking 0.013em. Buttons, navigation and labels.
- **label-sm:** Aeonik 14px at weight 400, line height 2. Small labels and badges.
- **code:** Aeonik Mono 14px at weight 500, line height 1.43, tracking 0.107em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 64px.
- **Sections:** 106px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1728px.
- **Page margin:** 96px on each side of full-width sections.
- **Breakpoints:** 390px, 400px, 425px, 426px, 550px, 600px, 767px, 768px, 896px, 900px, 1023px, 1024px, 1180px, 1200px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#120021).

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 112 elements.
- **md (12px):** 32 elements.
- **sm (8px):** 16 elements.
- **lg (24px):** 8 elements.
- **xl (96px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FFFFFF fill, #000000 text, 16px/500, 4px radius, padding 7px 24px.
- **button-secondary (“Let's connect”):** transparent fill, #FFFFFF text, 16px/500, 4px radius, padding 7px 24px, border 1px solid #FFFFFFF2.
- **button-outline (“Auth0 platform announcements”):** transparent fill, #FFFEFA text, 14px/400, 4px radius, padding 8px 12px 8px 16px, border 1px solid #FFFFFF54.
- **button-ghost (“AI Agents”):** transparent fill, #FFFFFF text, 18px/500, padding 24px 0px.
- **input-field (“Language selector”):** transparent fill, #FFFEFA text, 14px/500, padding 0px 16px 0px 20px.
- **card:** transparent fill, #FFFEFA text, 14px/400, 12px radius, padding 64px, border 1px solid #FFFFFF54.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #20003A for the page and lift surfaces in small steps: #120021.
- Do keep text in 4 levels: #FFFFFF, #E5E5E5, #EBD3FF, #C5C5C5.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #20003A.
- Do set headlines in Aeonik with tight tracking (-0.016em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 12px, 8px and 24px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Aeonik and Aeonik Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.6s, 0.25s. Longer ambient animations run 1.1s.

- **Easing:** `ease-in-out`, `ease`, `cubic-bezier(0.4, 0, 0.1, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/auth0.com/), the free DESIGN.md generator.

---
version: alpha
name: Jenkins
description: "Light interface measured from jenkins.io: georgia type with system-ui, vivid blue accents, flat surfaces and 10.56px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000C1A"
  on-background: "#000C1A"
  overlay: "#FFFFFF1A"
  overlay-strong: "#006CF61A"
  primary: "#006CF6"
  on-primary: "#FFFFFF"
  secondary: "#9EC5FE"
  tertiary: "#052C65"
typography:
  headline-display:
    fontFamily: georgia
    fontSize: 64px
    fontWeight: 700
  headline-lg:
    fontFamily: system-ui
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.2
  headline-md:
    fontFamily: system-ui
    fontSize: 21px
    fontWeight: 650
    lineHeight: 1.5
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.66
  body-lg:
    fontFamily: system-ui
    fontSize: 17.5px
    fontWeight: 500
    lineHeight: 1.3
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.66
rounded:
  md: 10.56px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 64px
  gutter: 16px
components:
  button-ghost:
    rounded: "{rounded.md}"
    padding: 8px 18px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Jenkins Design System

## Overview

Jenkins describes itself as: “Jenkins – an open source automation server which enables developers around the world to reliably build, test, and deploy their software” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#000C1A)** text, and **Vivid Blue (#006CF6)** as the main accent.

Type is set in **georgia** and **system-ui**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 10.56px.

Measured from [jenkins.io](https://www.jenkins.io/) on November 4, 2026 at 1440×900 and 390×844 from 202 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`, CSS `--docsearch-footer-background`.
- **Deep Blue (#000C1A):** Primary text and headings, seen 31 times. Token `on-surface`, CSS `--color`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Vivid Blue 10% (#006CF61A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Vivid Blue (#006CF6):** Links and interactive text, seen 35 times. Token `primary`, CSS `--accent-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#9EC5FE):** Accent (CSS variable). Token `secondary`.
- **Deep Blue (#052C65):** Accent (CSS variable). Token `tertiary`.

## Typography

**georgia** and **system-ui** share the interface. Fallback stack: `georgia`.

- **headline-display:** georgia 64px at weight 700. Page title (h1).
- **headline-lg:** system-ui 28px at weight 700, line height 1.2. Section headings (h2).
- **headline-md:** system-ui 21px at weight 650, line height 1.5. Sub-section headings.
- **body-md:** system-ui 16px at weight 450, line height 1.66. Body text.
- **body-lg:** system-ui 17.5px at weight 500, line height 1.3. Lead paragraphs.
- **body-sm:** system-ui 13px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** system-ui 16px at weight 400, line height 1.66. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3px, sm 8px, md 16px, lg 20px, xl 64px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 575.98px, 576px, 767.98px, 768px, 991.98px, 992px, 1199.98px, 1200px, 1399.98px, 1400px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 40, 0.3) 0px 30px 70px -50px`

## Shapes

Most elements use 10.56px corners. Measured radii, most used first:

- **md (10.56px):** 52 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Download”):** transparent fill, 14px/450, 10.56px radius, padding 8px 18px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 10px`.
- **card:** transparent fill, #000C1A text, 16px/400, 10.56px radius, padding 0px, shadow `rgba(0, 0, 40, 0.3) 0px 30px 70px -50px`.
- **link:** transparent fill, #006CF6 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do use #006CF6 for links and interactive text.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 10.56px corners on most elements.
- Don't introduce new font families beyond georgia and system-ui.
- Don't use #006CF6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.6s, 0.15s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/jenkins.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

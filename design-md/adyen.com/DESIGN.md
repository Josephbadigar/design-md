---
version: alpha
name: Adyen
description: "Dark interface measured from adyen.com: Adyen type, teal accents, flat surfaces and 6px corners."
colors:
  background: "#001222"
  surface: "#001222"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#636F7A"
  overlay: "#FFFFFF1B"
  primary: "#00D16A"
  on-primary: "#001222"
  secondary: "#007F41"
typography:
  headline-display:
    fontFamily: Adyen
    fontSize: 80px
    fontWeight: 436
    lineHeight: 1.02
  headline-lg:
    fontFamily: Adyen
    fontSize: 32px
    fontWeight: 484
    lineHeight: 1.18
  headline-md:
    fontFamily: Adyen
    fontSize: 20px
    fontWeight: 496
    lineHeight: 1.3
  body-md:
    fontFamily: Adyen
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.34
  label-md:
    fontFamily: Adyen
    fontSize: 16.5px
    fontWeight: 400
    lineHeight: 1.6
  label-sm:
    fontFamily: Adyen
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.34
  headline-lg-mobile:
    fontFamily: Adyen
    fontSize: 30px
    fontWeight: 484
    lineHeight: 1.18
  headline-md-mobile:
    fontFamily: Adyen
    fontSize: 19px
    fontWeight: 496
    lineHeight: 1.3
rounded:
  md: 6px
spacing:
  xs: 2.5px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 24px
  section: 240px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 24px
  link:
    textColor: "{colors.on-surface}"
---

# Adyen Design System

## Overview

Adyen describes itself as: “Run payments, manage your data, and offer financial products in one platform. Adyen is purpose-built for the world's leading businesses.” The interface is dark, built on **Deep Blue (#001222)** with **White (#FFFFFF)** text, and **Teal (#00D16A)** as the main accent.

Type is set in **Adyen**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 6px.

Measured from [adyen.com](https://www.adyen.com/) on November 4, 2026 at 1440×900 and 390×844 from 371 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Deep Blue (#001222):** Page background, seen 26 times. Token `background`, CSS `--color-black-3200`.
- **White (#FFFFFF):** Primary text and headings, seen 7 times. Token `on-surface`, CSS `--main-surface`.
- **Blue (#636F7A):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **White 11% (#FFFFFF1B):** Translucent fill for cards and controls, seen 12 times. Token `overlay`.
- **Teal (#00D16A):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--active-primary`.
- **Deep Blue (#001222):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#007F41):** Accent (CSS variable). Token `secondary`.

## Typography

**Adyen** carries the whole interface. Fallback stack: `Adyen, Helvetica, Arial, sans-serif`. Other loaded fonts: AdyenMono.

- **headline-display:** Adyen 80px at weight 436, line height 1.02. Page title (h1).
- **headline-lg:** Adyen 32px at weight 484, line height 1.18 (30px on mobile). Section headings (h2).
- **headline-md:** Adyen 20px at weight 496, line height 1.3 (19px on mobile). Sub-section headings.
- **body-md:** Adyen 16px at weight 400, line height 1.34. Body text.
- **label-md:** Adyen 16.5px at weight 400, line height 1.6. Buttons, navigation and labels.
- **label-sm:** Adyen 16px at weight 500, line height 1.34. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 60% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2.5px, sm 6px, md 16px, lg 24px, xl 48px.
- **Sections:** 240px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Breakpoints:** 320px, 767px, 768px, 1223px, 1224px, 1655px, 1992px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 236 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Talk to our team”):** #00D16A fill, #001222 text, 16.5626px/400, 6px radius, padding 0px 16px.
- **button-ghost (“INTELLIGENT MONEY MOVEMENT”):** transparent fill, #FFFFFF text, 16.5626px/400, padding 24px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #001222 for the page.
- Do keep text in 2 levels: #FFFFFF, #636F7A.
- Do reserve #00D16A for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 6px corners on most elements.
- Don't use #636F7A for body text; it reaches 3.68:1 on #001222. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Adyen.
- Don't use #00D16A for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.6s, 0.15s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.19, 1, 0.22, 1)`, `linear(0 0%, 0.0059 1%, 0.0225 2%, 0.0479 3%, 0.0806 4%, 0.1191 5%, 0.1621 6%, 0.2085 7%, 0.2573 8%, 0.3075 9%, 0.3583 10%, 0.4092 11%, 0.4593 12%, 0.5084 13%, 0.556 14%, 0.6018 15%, 0.6454 16%, 0.6867 17%, 0.7256 18%, 0.762 19%, 0.7958 20%, 0.827 21%, 0.8557 22%, 0.8818 23%, 0.9054 24%, 0.9267 25%, 0.9457 26%, 0.9626 27%, 0.9774 28%, 0.9903 29%, 1.0014 30%, 1.0109 31%, 1.0189 32%, 1.0255 33%, 1.0308 34%, 1.035 35%, 1.0382 36%, 1.0404 37%, 1.0419 38%, 1.0427 39%, 1.0428 40%, 1.0425 41%, 1.0417 42%, 1.0405 43%, 1.0391 44%, 1.0374 45%, 1.0355 46%, 1.0335 47%, 1.0314 48%, 1.0292 49%, 1.027 50%, 1.0249 51%, 1.0227 52%, 1.0206 53%, 1.0186 54%, 1.0167 55%, 1.0148 56%, 1.0131 57%, 1.0114 58%, 1.0099 59%, 1.0085 60%, 1.0071 61%, 1.0059 62%, 1.0048 63%, 1.0039 64%, 1.003 65%, 1.0022 66%, 1.0015 67%, 1.0008 68%, 1.0003 69%, 0.9998 70%, 0.9995 71%, 0.9991 72%, 0.9989 73%, 0.9986 74%, 0.9985 75%, 0.9983 76%, 0.9983 77%, 0.9982 78%, 0.9982 79%, 0.9982 80%, 0.9982 81%, 0.9982 82%, 0.9983 83%, 0.9983 84%, 0.9984 85%, 0.9985 86%, 0.9986 87%, 0.9987 88%, 0.9988 89%, 0.9989 90%, 0.999 91%, 0.999 92%, 0.9991 93%, 0.9992 94%, 0.9993 95%, 0.9994 96%, 0.9995 97%, 0.9995 98%, 0.9996 99%, 0.9997 100%)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/adyen.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

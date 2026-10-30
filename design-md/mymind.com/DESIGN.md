---
version: alpha
name: mymind
description: "Light interface measured from mymind.com: Avenir LT W01 45 Book1475508 type with Louize-Regular-205TF, vivid red accents, tonal surfaces and 100px corners."
colors:
  background: "#F9FAFC"
  surface: "#F9FAFC"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#3A475A"
  on-surface-muted: "#4A5465"
  on-surface-subtle: "#717286"
  surface-container-low: "#FFFFFF"
  surface-container: "#FFF1F1"
  outline: "#E98F53"
  outline-variant: "#E48ABF"
  primary: "#FF5924"
  on-primary: "#6E5558"
  inverse-surface: "#AFB5C1"
  secondary: "#5CB13E"
typography:
  headline-display:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 140px
    fontWeight: 400
    lineHeight: 0.85
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 96px
    fontWeight: 400
    lineHeight: 0.88
  headline-md:
    fontFamily: Louize-Regular-205TF
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 48px
    fontWeight: 400
    lineHeight: 0.92
  title-lg:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 42px
    fontWeight: 400
    lineHeight: 1.19
  body-md:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.67
  body-sm:
    fontFamily: Open Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.67
  caption:
    fontFamily: Nunito-SemiBold
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: 0.025em
  headline-display-mobile:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 50px
    fontWeight: 400
    lineHeight: 0.96
  headline-lg-mobile:
    fontFamily: Avenir LT W01 45 Book1475508
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.08
rounded:
  sm: 30px
  md: 36px
  lg: 100px
  xl: 120px
spacing:
  xs: 2px
  md: 10px
  lg: 24px
  xl: 33px
  section: 164px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#4A5465CC"
    typography: "{typography.body-md}"
    padding: 0px
    height: 24px
  button-primary-hover:
    textColor: "#24272D"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    padding: 0px
    height: 24px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# mymind Design System

## Overview

mymind describes itself as: “A private place to save your most precious notes, images, quotes and highlights. Enhanced with AI to help you remember without wasting time on categorizing & organizing.” The interface is light, built on **Snow (#F9FAFC)** with **Near Black (#000000)** text, and **Vivid Red (#FF5924)** as the main accent.

Type is set in **Avenir LT W01 45 Book1475508** and **Louize-Regular-205TF**. Headlines run large with tight negative tracking; body text is 20px. The surface language is flat. Corners are mostly 100px.

Measured from [mymind.com](https://mymind.com/) on October 29, 2026 at 1440×900 and 390×844 from 223 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #FF5924, #FFC0B4.

- **Snow (#F9FAFC):** Page background. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 21 times. Token `on-surface`.
- **Dark Blue (#3A475A):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Dark Blue (#4A5465):** Muted text and metadata, seen 13 times. Token `on-surface-muted`.
- **Cool Slate (#717286):** Subtle text and placeholders, seen 13 times. Token `on-surface-subtle`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Warm Snow (#FFF1F1):** Cards and panels, seen 4 times. Token `surface-container`.
- **Orange (#E98F53):** Borders and dividers, seen 1 time. Token `outline`.
- **Light Pink (#E48ABF):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Red (#FF5924):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **Red (#6E5558):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#AFB5C1):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Green (#5CB13E):** Secondary buttons, seen 1 time. Token `secondary`.

## Typography

**Avenir LT W01 45 Book1475508**, **Louize-Regular-205TF**, **Open Sans** and **Nunito-SemiBold** share the interface. Fallback stack: `Avenir LT W01_45 Book1475508, sans-serif`. Other loaded fonts: Avenir LT W01_45 Book1475508, Louize-Italic-205TF, Louize-Medium-205TF, Louize-Bold-205TF.

- **headline-display:** Avenir LT W01 45 Book1475508 140px at weight 400, line height 0.85, tracking -0.06em (50px on mobile). Page title (h1).
- **headline-lg:** Avenir LT W01 45 Book1475508 96px at weight 400, line height 0.88 (48px on mobile). Section headings (h2).
- **headline-md:** Louize-Regular-205TF 52px at weight 400, line height 1.3, tracking -0.025em. Sub-section headings.
- **headline-sm:** Avenir LT W01 45 Book1475508 48px at weight 400, line height 0.92. Card and feature titles.
- **title-lg:** Avenir LT W01 45 Book1475508 42px at weight 400, line height 1.19. Small titles.
- **body-md:** Avenir LT W01 45 Book1475508 20px at weight 400, line height 1.4. Body text.
- **body-lg:** Avenir LT W01 45 Book1475508 24px at weight 400, line height 1.67. Lead paragraphs.
- **body-sm:** Open Sans 18px at weight 400, line height 1.67. Secondary and small text.
- **caption:** Nunito-SemiBold 16px at weight 400, line height 1.67, tracking 0.025em. Captions and fine print.

## Layout

Spacing does not follow a strict grid: 32% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, md 10px, lg 24px, xl 33px.
- **Sections:** 164px vertical padding between major sections.
- **Breakpoints:** 543px, 543.98px, 544px, 767px, 767.98px, 768px, 991px, 991.98px, 992px, 1024px, 1080px, 1169px, 1169.98px, 1170px, 1400px, 1440px, 1651px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF → #FFF1F1) and #E98F53 borders.

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 52 elements.
- **md (36px):** 20 elements.
- **xl (120px):** 8 elements.
- **sm (30px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“What”):** #FF5924 fill, #4A5465CC text, 20px/400, 50% radius, padding 0px.
- **button-primary-hover:** background #FF5924, text #24272D on hover.
- **button-secondary (“Log in”):** #5CB13E fill, #4A5465 text, 20px/400, 50% radius, padding 0px.
- **link:** transparent fill, #717286 text, padding 0px.

## Do's and Don'ts

- Do use #F9FAFC for the page and lift surfaces in small steps: #FFFFFF, #FFF1F1.
- Do keep text in 4 levels: #000000, #3A475A, #4A5465, #717286.
- Do reserve #FF5924 for primary actions and key highlights.
- Do set headlines in Avenir LT W01 45 Book1475508 with tight tracking (-0.06em).
- Do reuse the measured spacing steps (10px, 24px).
- Do use 100px corners on most elements; larger surfaces also use 36px, 120px and 30px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Avenir LT W01 45 Book1475508, Louize-Regular-205TF, Open Sans and Nunito-SemiBold.
- Don't use #FF5924 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.25s, 0.5s, 0.6s. Longer ambient animations run 0.7s, 5s.

- **Easing:** `linear`, `cubic-bezier(0.19, 1, 0.22, 1)`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mymind.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).

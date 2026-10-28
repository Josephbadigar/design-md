---
version: alpha
name: Mailchimp
description: "Light interface measured from mailchimp.com: Means Web type with Graphik Web, vivid amber accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#231E15"
  on-surface-muted: "#403B3B"
  on-surface-subtle: "#706D67"
  surface-container-low: "#F5F5F5"
  outline: "#DBD9D2"
  outline-variant: "#DEDEDE"
  primary: "#FFE01B"
  on-primary: "#231E15"
  secondary: "#004E56"
  warning: "#E7B75F"
typography:
  headline-display:
    fontFamily: Means Web
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.019em
  headline-lg:
    fontFamily: Means Web
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.17
  headline-md:
    fontFamily: Means Web
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.013em
  headline-sm:
    fontFamily: Graphik Web
    fontSize: 23px
    fontWeight: 400
    lineHeight: 1.3
  title-lg:
    fontFamily: Graphik Web
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.6
  body-md:
    fontFamily: Graphik Web
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.35
  body-sm:
    fontFamily: Graphik Web
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.35
  caption:
    fontFamily: Graphik Web
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.45
  label-lg:
    fontFamily: Graphik Web
    fontSize: 15px
    fontWeight: 500
    lineHeight: 2.13
  label-md:
    fontFamily: Graphik Web
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Graphik Web
    fontSize: 11px
    fontWeight: 700
    lineHeight: 1.45
  headline-display-mobile:
    fontFamily: Means Web
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.3
  headline-md-mobile:
    fontFamily: Means Web
    fontSize: 29px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.017em
rounded:
  xs: 4px
  sm: 16px
  md: 24px
  lg: 26px
  xl: 30px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  section: 80px
  margin: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 12px 24px
    height: 44px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xs}"
    padding: 10px 16px
    height: 44px
  button-ghost:
    backgroundColor: "#241C15"
    textColor: "{colors.background}"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 12px 30px
    height: 31px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 24px 8px 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Mailchimp Design System

## Overview

Mailchimp describes itself as: “Utilize real-time user behavior data and artificial intelligence to convert more customers. Easy to use, get started for free!” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Amber (#FFE01B)** as the main accent.

Type is set in **Means Web** and **Graphik Web**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [mailchimp.com](https://mailchimp.com/) on October 21, 2026 at 1440×900 and 390×844 from 371 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #FFE01B.

- **White (#FFFFFF):** Page background, seen 20 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 58 times. Token `on-surface`.
- **Warm Charcoal (#231E15):** Secondary text, seen 105 times. Token `on-surface-variant`, CSS `--cta-depth-color`.
- **Graphite (#403B3B):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **Warm Slate (#706D67):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`, CSS `--copy-color-light`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Warm Silver (#DBD9D2):** Borders and dividers, seen 10 times. Token `outline`, CSS `--cta-background-color-disabled`.
- **Silver (#DEDEDE):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Amber (#FFE01B):** Primary buttons and calls to action, seen 21 times. Token `primary`, CSS `--cta-background-color`.
- **Warm Charcoal (#231E15):** Text and icons on primary. Token `on-primary`.
- **Deep Cyan (#004E56):** Most used accent color, seen 8 times. Token `secondary`.
- **Orange (#E7B75F):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**Means Web** and **Graphik Web** share the interface. Fallback stack: `Means Web, Georgia, Times, Times New Roman`.

- **headline-display:** Means Web 64px at weight 400, line height 1.2, tracking -0.019em (36px on mobile). Page title (h1).
- **headline-lg:** Means Web 48px at weight 400, line height 1.17. Section headings (h2).
- **headline-md:** Means Web 40px at weight 400, line height 1, tracking -0.013em (29px on mobile). Sub-section headings.
- **headline-sm:** Graphik Web 23px at weight 400, line height 1.3. Card and feature titles.
- **title-lg:** Graphik Web 20px at weight 400, line height 1.6. Small titles.
- **body-md:** Graphik Web 16px at weight 400, line height 1.35. Body text.
- **body-sm:** Graphik Web 13px at weight 400, line height 1.35. Secondary and small text.
- **caption:** Graphik Web 11px at weight 400, line height 1.45. Captions and fine print.
- **label-lg:** Graphik Web 15px at weight 500, line height 2.13. Large buttons and tabs.
- **label-md:** Graphik Web 13px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Graphik Web 11px at weight 700, line height 1.45. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 12px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.086) 0px 15.547px 44px 0px`
- `rgba(0, 0, 0, 0.06) 0px 4px 16px 0px`

Hairline rings and inset highlights also appear: `rgb(35, 30, 21) 0px 0px 0px 1px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 84 elements.
- **sm (16px):** 68 elements.
- **lg (26px):** 40 elements.
- **full (9999px):** 24 elements.
- **md (24px):** 16 elements.
- **xl (30px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #FFE01B fill, #231E15 text, 13px/500, 26px radius, padding 12px 24px, shadow `rgb(35, 30, 21) 0px 0px 0px 1px`.
- **button-outline (“Select”):** #FFFFFF fill, #231E15 text, 16px/400, 4px radius, padding 10px 16px, border 1px solid #231E15A6.
- **button-ghost (“Customize settings”):** #241C15 fill, #FFFFFF text, 11px/200, padding 12px 30px, border 1px solid #FFFFFF.
- **input-field (“Currency”):** transparent fill, #231E15 text, 13px/500, padding 8px 24px 8px 0px.
- **card:** #FFFFFF fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #231E15 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5.
- Do keep text in 4 levels: #000000, #231E15, #403B3B, #706D67.
- Do reserve #FFE01B for primary actions and key highlights.
- Do set headlines in Means Web with tight tracking (-0.019em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 16px, 26px and 24px.
- Don't introduce new font families beyond Means Web and Graphik Web.
- Don't use #FFE01B for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.4s, 0.15s, 0.3s.

- **Easing:** `ease`, `ease-out`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mailchimp.com/), the free DESIGN.md generator.

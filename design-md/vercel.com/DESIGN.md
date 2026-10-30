---
version: alpha
name: Vercel
description: "Light interface measured from vercel.com: GeistSans type, red accents, tonal surfaces and 6px corners."
colors:
  background: "#FAFAFA"
  surface: "#FAFAFA"
  on-surface: "#171717"
  on-background: "#171717"
  on-surface-variant: "#4D4D4D"
  on-surface-muted: "#8F8F8F"
  surface-container-low: "#FFFFFF"
  surface-container: "#EBEBEB"
  primary: "#BA1638"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: GeistSans
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: GeistSans
    fontSize: 56px
    fontWeight: 450
    lineHeight: 1
    letterSpacing: -0.06em
  body-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: GeistSans
    fontSize: 24px
    fontWeight: 450
    lineHeight: 1.33
    letterSpacing: -0.04em
  label-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: GeistSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  code:
    fontFamily: Geist Mono
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.67
  headline-display-mobile:
    fontFamily: GeistSans
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.17
    letterSpacing: -0.06em
rounded:
  sm: 4px
  md: 6px
  lg: 20px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 20px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 0px 6px
    height: 32px
  button-outline-hover:
    backgroundColor: "#F2F2F2"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 0px 6px
    height: 32px
  button-secondary-hover:
    backgroundColor: "#383838"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Vercel Design System

## Overview

Vercel describes itself as: “The autonomous stack for every app and agent.” The interface is light, built on **Snow (#FAFAFA)** with **Charcoal (#171717)** text, and **Red (#BA1638)** as the main accent.

Type is set in **GeistSans**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 6px.

Measured from [vercel.com](https://vercel.com/) on October 30, 2026 at 1440×900 and 390×844 from 358 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Snow (#FAFAFA):** Page background, seen 5 times. Token `background`, CSS `--ds-background-200`.
- **Charcoal (#171717):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Slate (#4D4D4D):** Secondary text, seen 92 times. Token `on-surface-variant`.
- **Gray (#8F8F8F):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`, CSS `--dropdown-triangle-stroke`.
- **Mist (#EBEBEB):** Cards and panels, seen 4 times. Token `surface-container`.
- **Red (#BA1638):** Brand color in the logo. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**GeistSans** and **Geist Mono** (monospace) share the interface. Fallback stack: `GeistSans, GeistSans Fallback`.

- **headline-display:** GeistSans 64px at weight 400, line height 1, tracking -0.06em (48px on mobile). Page title (h1).
- **headline-lg:** GeistSans 56px at weight 450, line height 1, tracking -0.06em. Section headings (h2).
- **body-md:** GeistSans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** GeistSans 24px at weight 450, line height 1.33, tracking -0.04em. Lead paragraphs.
- **label-md:** GeistSans 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** GeistSans 14px at weight 400, line height 1.43. Small labels and badges.
- **code:** Geist Mono 12px at weight 500, line height 1.67, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 15% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 20px, xl 40px.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Breakpoints:** 401px, 600px, 601px, 880px, 960px, 961px, 992px, 1024px, 1200px, 1400px, 1600px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFF → #EBEBEB):

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(235, 235, 235) 0px 0px 0px 1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(235, 235, 235) 0px 0px 0px 1px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 0px 0px 1px, rgb(250, 250, 250) 0px 0px 0px 1px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 2px 2px 0px, rgb(250, 250, 250) 0px 0px 0px 1px`.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 24 elements.
- **lg (20px):** 24 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Get a Demo”):** #FFFFFF fill, #171717 text, 14px/500, 6px radius, padding 0px 6px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(235, 235, 235) 0px 0px 0px 1px`.
- **button-outline-hover:** background #F2F2F2, text #171717 on hover.
- **button-secondary (“Sign Up”):** #171717 fill, #FFFFFF text, 14px/500, 6px radius, padding 0px 6px.
- **button-secondary-hover:** background #383838, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #4D4D4D text, 14px/400, padding 0px.
- **link:** transparent fill, #4D4D4D text, padding 0px.

## Do's and Don'ts

- Do use #FAFAFA for the page and lift surfaces in small steps: #FFFFFF, #EBEBEB.
- Do keep text in 3 levels: #171717, #4D4D4D, #8F8F8F.
- Do use #BA1638 as the brand accent: header, logo and key highlights.
- Do set headlines in GeistSans with tight tracking (-0.06em).
- Do reuse the measured spacing steps (6px, 12px, 20px).
- Do use 6px corners on most elements; larger surfaces also use 20px and 4px.
- Don't use #8F8F8F for body text; it reaches 3.10:1 on #FAFAFA. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond GeistSans and Geist Mono.
- Don't use #BA1638 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.2s, 0.5s. Longer ambient animations run 0.95s, 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/vercel.com/), the free DESIGN.md generator (engine 2026.10.29+bf9d681d83cf).

---
version: alpha
name: Supabase
description: "Dark interface measured from supabase.com: Manrope type with Inter, deep teal accents, tonal surfaces and 8px corners."
colors:
  background: "#131413"
  surface: "#131413"
  on-surface: "#EDEFEE"
  on-background: "#EDEFEE"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#BCBDBC"
  on-surface-muted: "#989A99"
  surface-container-low: "#0C0F24"
  surface-container: "#181A19"
  surface-container-high: "#000000"
  overlay: "#EDEFEE08"
  overlay-strong: "#0000001F"
  outline: "#EEEFEE13"
  outline-variant: "#EEEFEE22"
  primary: "#006338"
  on-primary: "#EDEFEE"
  secondary: "#BDA4FF"
  tertiary: "#FFCDA1"
  success: "#3ECF8E"
typography:
  headline-display:
    fontFamily: Manrope
    fontSize: 46px
    fontWeight: 500
    lineHeight: 1
  headline-lg:
    fontFamily: Manrope
    fontSize: 34px
    fontWeight: 600
    lineHeight: 1.11
  headline-md:
    fontFamily: Manrope
    fontSize: 22px
    fontWeight: 450
    lineHeight: 1.38
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 450
    lineHeight: 1.43
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 450
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 450
    lineHeight: 1.33
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.5
  label-md:
    fontFamily: Manrope
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Manrope
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.11
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.33
rounded:
  xs: 8px
  sm: 9.29px
  md: 10.67px
  lg: 16px
  xl: 21.33px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xs}"
    padding: 4px 10px
    height: 26px
  button-primary-hover:
    backgroundColor: "#076E43"
  button-secondary:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xs}"
    padding: 4px 10px
    height: 26px
  button-secondary-hover:
    backgroundColor: "#EDEFEE0C"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 8px 32px
    height: 38px
  button-ghost:
    typography: "{typography.label-sm}"
    rounded: 8.86px
    padding: 8px 10px
  card:
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 24px
  link:
    textColor: "{colors.on-surface}"
---

# Supabase Design System

## Overview

Supabase describes itself as: “Build production-grade applications with a Postgres database, Authentication, instant APIs, Realtime, Functions, Storage and Vector embeddings. Start for free.” The interface is dark, built on **Charcoal (#131413)** with **Mist (#EDEFEE)** text, and **Deep Teal (#006338)** as the main accent.

Type is set in **Manrope** and **Inter**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [supabase.com](https://supabase.com/) on October 21, 2026 at 1440×900 and 390×844 from 430 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #FD49A8, #FD2980, #FC1A58, #FA1F41.

- **Charcoal (#131413):** Page background, seen 5 times. Token `background`.
- **Mist (#EDEFEE):** Primary text and headings, seen 49 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 27 times. Token `on-surface-strong`, CSS `--color-white`.
- **Silver (#BCBDBC):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Gray (#989A99):** Muted text and metadata, seen 15 times. Token `on-surface-muted`.
- **Deep Indigo (#0C0F24):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Charcoal (#181A19):** Cards and panels, seen 23 times. Token `surface-container`.
- **Near Black (#000000):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Mist 3% (#EDEFEE08):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Near Black 12% (#0000001F):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Mist 8% (#EEEFEE13):** Borders and dividers, seen 34 times. Token `outline`.
- **Mist 13% (#EEEFEE22):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Deep Teal (#006338):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **Mist (#EDEFEE):** Text and icons on primary. Token `on-primary`.
- **Light Violet (#BDA4FF):** Most used accent color, seen 15 times. Token `secondary`.
- **Light Orange (#FFCDA1):** Most used accent color, seen 5 times. Token `tertiary`.
- **Teal (#3ECF8E):** Success and positive states, seen 14 times. Token `success`.

## Typography

**Manrope** and **Inter** share the interface. Fallback stack: `Manrope, Manrope Fallback, system-ui, Helvetica Neue`. Other loaded fonts: Manrope Fallback, Inter Fallback, Source Code Pro.

- **headline-display:** Manrope 46px at weight 500, line height 1 (34px on mobile). Page title (h1).
- **headline-lg:** Manrope 34px at weight 600, line height 1.11 (22px on mobile). Section headings (h2).
- **headline-md:** Manrope 22px at weight 450, line height 1.38. Sub-section headings.
- **body-md:** Inter 14px at weight 450, line height 1.43. Body text.
- **body-lg:** Inter 15px at weight 450, line height 1.5. Lead paragraphs.
- **body-sm:** Inter 12px at weight 450, line height 1.33. Secondary and small text.
- **label-lg:** Inter 16px at weight 450, line height 1.5. Large buttons and tabs.
- **label-md:** Manrope 15px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.2) 0px 1px 3px 0px, rgba(255, 255, 255, 0.04) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.06) 0px -1px 0px 0px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.2) 0px 1px 3px 0px, rgba(255, 255, 255, 0.04) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.06) 0px 0px 0px 1px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`

Hairline rings and inset highlights also appear: `rgba(255, 255, 255, 0.12) 0px 0px 0px 1px inset`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **xs (8px):** 76 elements.
- **xl (21.33px):** 60 elements.
- **lg (16px):** 28 elements.
- **md (10.67px):** 24 elements.
- **sm (9.29px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start your project”):** #006338 fill, #EDEFEE text, 12px/500, 8px radius, padding 4px 10px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.2) 0px 1px 3px 0px, rgba(255, 255, 255, 0.04) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.06) 0px 0px 0px 1px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`.
- **button-primary-hover:** background #076E43, text #EDEFEE on hover.
- **button-secondary (“Sign in”):** #EDEFEE08 fill, #EDEFEE text, 12px/500, 8px radius, padding 4px 10px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.2) 0px 1px 3px 0px, rgba(255, 255, 255, 0.04) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.06) 0px -1px 0px 0px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`.
- **button-secondary-hover:** background #EDEFEE0C, text #EDEFEE on hover.
- **button-outline (“Table Editor”):** #131413 fill, #EDEFEE text, 14px/450, 3.35544e+07px radius, padding 8px 32px, border 1px solid #EDEFEE.
- **button-ghost (“Product”):** transparent fill, 14px/500, 8.86154px radius, padding 8px 10px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** transparent fill, 16px/450, 21.3333px radius, padding 24px.
- **link:** transparent fill, #EDEFEE text, padding 0px.

## Do's and Don'ts

- Do use #131413 for the page and lift surfaces in small steps: #0C0F24, #181A19, #000000.
- Do keep text in 4 levels: #EDEFEE, #FFFFFF, #BCBDBC, #989A99.
- Do reserve #006338 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 21.33px, 16px and 10.67px.
- Don't introduce new font families beyond Manrope and Inter.
- Don't use #006338 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/supabase.com/), the free DESIGN.md generator.

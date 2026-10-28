---
version: alpha
name: Flutter
description: "Dark interface measured from flutter.dev: Google Sans Flex type, blue accents, flat surfaces and 24px corners."
colors:
  background: "#1A68D3"
  surface: "#1A68D3"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#000000"
  outline: "#0468D7"
  primary: "#1A68D3"
  on-primary: "#FFFFFF"
  secondary: "#14C2AD"
  error: "#F25D50"
typography:
  headline-display:
    fontFamily: Google Sans Flex
    fontSize: 60px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.005em
  headline-lg:
    fontFamily: Google Sans Flex
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.005em
  headline-md:
    fontFamily: Google Sans Flex
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.005em
  body-md:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Google Sans Flex
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Google Sans Flex
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Google Sans Flex
    fontSize: 46px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.005em
rounded:
  sm: 8px
  md: 24px
spacing:
  sm: 8px
  md: 12px
  lg: 32px
  xl: 50px
  section: 70px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.outline}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 0px 32px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 8px 12px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 8px 0px
  card:
    textColor: "#4A4A4A"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "#4A4A4A"
---

# Flutter Design System

## Overview

Flutter describes itself as: “Flutter transforms the entire app development process. Build, test, and deploy beautiful mobile, web, desktop, and embedded apps from a single codebase.” The interface is dark, built on **Blue (#1A68D3)** with **White (#FFFFFF)** text, and **Blue (#1A68D3)** as the main accent.

Type is set in **Google Sans Flex**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 24px.

Measured from [flutter.dev](https://flutter.dev/) on October 21, 2026 at 1440×900 and 390×844 from 245 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles, plus gradient stops #1A68D3, #71C7EE, #027DFD, #833EF2.

- **Blue (#1A68D3):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 16 times. Token `on-surface`.
- **Near Black (#000000):** Secondary text, seen 62 times. Token `on-surface-variant`.
- **Vivid Blue (#0468D7):** Borders and dividers, seen 6 times. Token `outline`, CSS `--site-filledButton-bgColor`.
- **Blue (#1A68D3):** Brand color on large areas, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Teal (#14C2AD):** Most used accent color, seen 3 times. Token `secondary`.
- **Red (#F25D50):** Errors and destructive states, seen 1 time. Token `error`, CSS `--coral`.

## Typography

**Google Sans Flex** carries the whole interface. Fallback stack: `Google Sans Flex, Roboto, ui-sans, sans-serif`. Other loaded fonts: Material Symbols Rounded.

- **headline-display:** Google Sans Flex 60px at weight 600, line height 1, tracking -0.005em (46px on mobile). Page title (h1).
- **headline-lg:** Google Sans Flex 36px at weight 400, line height 1.2, tracking -0.005em. Section headings (h2).
- **headline-md:** Google Sans Flex 28px at weight 600, line height 1.2, tracking -0.005em. Sub-section headings.
- **body-md:** Google Sans Flex 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Google Sans Flex 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Google Sans Flex 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Google Sans Flex 14px at weight 600, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (71% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 12px, lg 32px, xl 50px.
- **Sections:** 70px vertical padding between major sections.
- **Breakpoints:** 350px, 360px, 380px, 390px, 420px, 540px, 576px, 600px, 640px, 768px, 900px, 1023px, 1024px, 1280px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.25) 0px 8px 24px 0px`
- `rgba(0, 0, 0, 0.35) 0px 16px 48px 0px`

## Shapes

Most elements use 24px corners. Measured radii, most used first:

- **md (24px):** 196 elements.
- **sm (8px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FFFFFF fill, #0468D7 text, 14px/600, 24px radius, padding 0px 32px.
- **button-ghost (“Development”):** transparent fill, #FFFFFF text, 14px/600, 24px radius, padding 8px 12px.
- **input-field (“Enter your email address”):** transparent fill, #000000 text, 16px/400, padding 8px 0px.
- **card:** transparent fill, #4A4A4A text, 14px/400, 8px radius, padding 0px, shadow `rgba(0, 0, 0, 0.25) 0px 8px 24px 0px`.
- **link:** transparent fill, #4A4A4A text, padding 0px.

## Do's and Don'ts

- Do use #1A68D3 for the page.
- Do keep text in 2 levels: #FFFFFF, #000000.
- Do use #1A68D3 as the brand accent: header, logo and key highlights.
- Do set headlines in Google Sans Flex with tight tracking (-0.005em).
- Do reuse the measured spacing steps (8px, 12px, 32px).
- Do use 24px corners on most elements; larger surfaces also use 8px.
- Don't use #000000 for body text; it reaches 4.0:1 on #1A68D3. Keep it for large text or metadata.
- Don't introduce new font families beyond Google Sans Flex.
- Don't use #1A68D3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.25s, 0.4s, 0.2s. Longer ambient animations run 0.75s.

- **Easing:** `ease`, `ease-in`, `cubic-bezier(0.27, 0.89, 0.39, 0.95)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/flutter.dev/), the free DESIGN.md generator.

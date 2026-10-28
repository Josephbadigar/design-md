---
version: alpha
name: Later
description: "Light interface measured from later.com: Super X sans Display type with Inter Tight, vivid red accents, tonal surfaces and square corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#FEFCFB"
  surface-container: "#F8F2EA"
  outline: "#F8F2EA"
  outline-variant: "#FEFCFB"
  primary: "#FE3F00"
  on-primary: "#F8F2EA"
  secondary: "#5124C1"
typography:
  headline-display:
    fontFamily: Super X sans Display
    fontSize: 80.5px
    fontWeight: 900
    lineHeight: 1
    letterSpacing: 0.005em
  headline-lg:
    fontFamily: Super X sans Display
    fontSize: 70px
    fontWeight: 900
    lineHeight: 1.25
    letterSpacing: 0.005em
  headline-md:
    fontFamily: Super X sans Display
    fontSize: 56px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: 0.005em
  headline-sm:
    fontFamily: Super X sans Display
    fontSize: 44px
    fontWeight: 800
    lineHeight: 1.25
    letterSpacing: 0.005em
  title-lg:
    fontFamily: Super X sans Display
    fontSize: 38px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: 0.005em
  body-md:
    fontFamily: Inter Tight
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter Tight
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter Tight
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Inter Tight
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
  label-md:
    fontFamily: Inter Tight
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter Tight
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: Super X sans Display
    fontSize: 32px
    fontWeight: 900
    lineHeight: 1
    letterSpacing: 0.005em
rounded:
  none: 0px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 32px
  section: 70px
  margin: 40px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 12px 40px 12px 24px
    height: 55px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 12px 40px 12px 24px
    height: 55px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 12px 40px 12px 24px
    height: 47px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 0px 8px
  input-field:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 8px 16px
  link:
    textColor: "#F9F3ECCC"
---

# Later Design System

## Overview

Later describes itself as: “Influencer marketing built for creators and trusted by brands. Run campaigns, manage social media, and track performance with AI-powered insights.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Red (#FE3F00)** as the main accent.

Type is set in **Super X sans Display** and **Inter Tight**. Headlines run large; body text is 14px. The surface language is flat. Corners are square.

Measured from [later.com](https://later.com/) on October 21, 2026 at 1440×900 and 390×844 from 343 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background. Token `background`, CSS `--color-white`.
- **Near Black (#000000):** Primary text and headings, seen 28 times. Token `on-surface`, CSS `--tiktok`.
- **Snow (#FEFCFB):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Warm Mist (#F8F2EA):** Cards and panels, seen 6 times. Token `surface-container`, CSS `--lib`.
- **Warm Mist (#F8F2EA):** Borders and dividers, seen 8 times. Token `outline`, CSS `--lib`.
- **Snow (#FEFCFB):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Red (#FE3F00):** Primary buttons and calls to action, seen 7 times. Token `primary`.
- **Warm Mist (#F8F2EA):** Text and icons on primary. Token `on-primary`.
- **Violet (#5124C1):** Accent, seen 8 times. Token `secondary`.

## Typography

**Super X sans Display** and **Inter Tight** share the interface. Fallback stack: `Super X sans Display, Helvetica Neue, Helvetica, Arial`.

- **headline-display:** Super X sans Display 80.5px at weight 900, line height 1, tracking 0.005em (32px on mobile). Page title (h1).
- **headline-lg:** Super X sans Display 70px at weight 900, line height 1.25, tracking 0.005em. Section headings (h2).
- **headline-md:** Super X sans Display 56px at weight 800, line height 1, tracking 0.005em. Sub-section headings.
- **headline-sm:** Super X sans Display 44px at weight 800, line height 1.25, tracking 0.005em. Card and feature titles.
- **title-lg:** Super X sans Display 38px at weight 700, line height 1.25, tracking 0.005em. Small titles.
- **body-md:** Inter Tight 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter Tight 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Inter Tight 13px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Inter Tight 16px at weight 400, line height 1.25. Large buttons and tabs.
- **label-md:** Inter Tight 15px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter Tight 14px at weight 600, line height 1.25, tracking 0.03em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 70px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 500px, 501px, 799px, 800px, 991px, 992px, 1199px, 1200px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FEFCFB → #F8F2EA) and #F8F2EA borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start your campaign”):** #FE3F00 fill, #F8F2EA text, 16px/400, padding 12px 40px 12px 24px, border 2px solid #FE3F00.
- **button-secondary (“Earn as a creator”):** #000000 fill, #000000 text, 16px/400, padding 12px 40px 12px 24px, border 2px solid #000000.
- **button-tertiary (“Get Later”):** #000000 fill, #F8F2EA text, 16px/400, padding 12px 40px 12px 24px, border 2px solid #000000.
- **button-ghost (“Sign in”):** transparent fill, #000000 text, 16px/400, padding 0px 8px.
- **input-field (“Enter your email address”):** transparent fill, #FEFCFB text, 16px/400, padding 8px 16px, border 1px solid #FEFCFB, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 3.2px, rgba(0, 0, 0, 0) 0px 0px 0px 6.4px`.
- **link:** transparent fill, #F9F3ECCC text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FEFCFB, #F8F2EA.
- Do reserve #FE3F00 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Super X sans Display and Inter Tight.
- Don't use #FE3F00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.000001s.

## Motion

Interface transitions are quick: 1e-06s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/later.com/), the free DESIGN.md generator.

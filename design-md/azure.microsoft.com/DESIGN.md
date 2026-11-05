---
version: alpha
name: Microsoft Azure
description: "Dark interface measured from azure.microsoft.com: Segoe UI Variable Display type with Segoe UI Variable Text, blue accents, flat surfaces and 8px corners."
colors:
  background: "#002948"
  surface: "#002948"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F4FAFD"
  on-surface-muted: "#616161"
  overlay: "#0055971A"
  outline: "#000000"
  outline-variant: "#17253D"
  primary: "#0078D4"
  on-primary: "#FFFFFF"
  inverse-surface: "#FEFEFE"
  secondary: "#B3DAF0"
  tertiary: "#05037B"
typography:
  headline-display:
    fontFamily: Segoe UI Variable Display
    fontSize: 62px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Segoe UI Variable Display
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.17
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Segoe UI Variable Display
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Segoe UI Variable Display
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.01em
  title-lg:
    fontFamily: Segoe UI Variable Display
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: Segoe UI Variable Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.03em
  body-sm:
    fontFamily: Segoe UI
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: -0.044em
  label-lg:
    fontFamily: Segoe UI Variable Text
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Segoe UI Variable Text
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.47
    letterSpacing: -0.02em
  label-sm:
    fontFamily: Segoe UI Variable Text
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Segoe UI Variable Display
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
  title-lg-mobile:
    fontFamily: Segoe UI Variable Display
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.33
rounded:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 200px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
  gutter: 8px
  margin: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.xs}"
    padding: 4px 8px 12px 8px
    height: 31px
  button-primary-hover:
    backgroundColor: "#006DC1"
  button-secondary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.outline}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 16px
    height: 66px
  button-tertiary:
    backgroundColor: "{colors.secondary}"
    textColor: "#0E1726"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 52px
  button-ghost:
    textColor: "#262626"
    rounded: 0px
    padding: 1px 8px
  input-field:
    textColor: "{colors.outline}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 20px 60px 20px 16px
  card:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.outline-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 96px 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Microsoft Azure Design System

## Overview

Microsoft Azure describes itself as: “Invent with purpose, realize cost savings, and make your organization more efficient with Microsoft Azure’s open and flexible cloud computing platform.” The interface is dark, built on **Deep Blue (#002948)** with **White (#FFFFFF)** text, and **Blue (#0078D4)** as the main accent.

Type is set in **Segoe UI Variable Display** and **Segoe UI Variable Text**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [azure.microsoft.com/en-us](https://azure.microsoft.com/en-us) (the site sent our reader to its /en-us version; azure.microsoft.com was asked for) on November 4, 2026 at 1440×900 and 390×844 from 287 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Deep Blue (#002948):** Page background. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 13 times. Token `on-surface`.
- **Cool Snow (#F4FAFD):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Slate (#616161):** Muted text and metadata, seen 44 times. Token `on-surface-muted`.
- **Dark Blue 10% (#0055971A):** Translucent fill for cards and controls, seen 9 times. Token `overlay`.
- **Near Black (#000000):** Borders and dividers, seen 1 time. Token `outline`.
- **Deep Blue (#17253D):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--ds-comp-color-input-field-label-text-default`.
- **Blue (#0078D4):** Primary buttons and calls to action, seen 12 times. Token `primary`, CSS `--root-color-brilliant-blue-500`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **White (#FEFEFE):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Light Blue (#B3DAF0):** Secondary buttons, seen 1 time. Token `secondary`.
- **Dark Indigo (#05037B):** Accent in logos and imagery. Token `tertiary`.

## Typography

**Segoe UI Variable Display**, **Segoe UI Variable Text** and **Segoe UI** share the interface. Fallback stack: `Segoe UI Variable Display, Segoe UI, segoeui, Helvetica Neue`. Other loaded fonts: MWF-FLUENT-ICONS, SegoeUI, FabricMDL2Icons.

- **headline-display:** Segoe UI Variable Display 62px at weight 500, line height 1.16, tracking -0.025em (40px on mobile). Page title (h1).
- **headline-lg:** Segoe UI Variable Display 48px at weight 500, line height 1.17, tracking -0.025em. Section headings (h2).
- **headline-md:** Segoe UI Variable Display 32px at weight 500, line height 1.25, tracking -0.015em. Sub-section headings.
- **headline-sm:** Segoe UI Variable Display 24px at weight 500, line height 1.33, tracking -0.01em. Card and feature titles.
- **title-lg:** Segoe UI Variable Display 20px at weight 600, line height 1.4 (18px on mobile). Small titles.
- **body-md:** Segoe UI Variable Text 16px at weight 400, line height 1.5, tracking -0.03em. Body text.
- **body-sm:** Segoe UI 11px at weight 400, line height 1.45, tracking -0.044em. Secondary and small text.
- **label-lg:** Segoe UI Variable Text 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Segoe UI Variable Text 15px at weight 600, line height 1.47, tracking -0.02em. Buttons, navigation and labels.
- **label-sm:** Segoe UI Variable Text 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (88% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 72px on each side of full-width sections.
- **Breakpoints:** 540px, 859px, 859.98px, 860px, 1083px, 1084px, 1400px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 1.008px 2px 0px`
- `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 2px 4px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 68 elements.
- **xl (200px):** 44 elements.
- **lg (24px):** 24 elements.
- **xs (3px):** 16 elements.
- **md (16px):** 5 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started with Azure”):** #0078D4 fill, #FFFFFF text, 13px/400, 3px radius, padding 4px 8px 12px 8px.
- **button-primary-hover:** background #006DC1, text #FFFFFF on hover.
- **button-secondary (“Ask Microsoft​”):** #F4FAFD fill, #000000 text, 14px/400, 8px radius, padding 16px, border 1px solid #CBE6F4, shadow `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 8px 16px 0px`.
- **button-tertiary (“Get started with Azure”):** #B3DAF0 fill, #0E1726 text, 15px/600, 8px radius, padding 12px 16px.
- **button-ghost (“Explore”):** transparent fill, #262626 text, 13px/400, padding 1px 8px.
- **input-field (“Ask a question about Azure.”):** transparent fill, #000000 text, 16px/400, 8px radius, padding 20px 60px 20px 16px.
- **card:** #F4FAFD fill, #17253D text, 16px/400, padding 96px 0px.
- **link:** transparent fill, #616161 text, padding 0px.

## Do's and Don'ts

- Do use #002948 for the page.
- Do keep text in 3 levels: #FFFFFF, #F4FAFD, #616161.
- Do reserve #0078D4 for primary actions and key highlights.
- Do set headlines in Segoe UI Variable Display with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 200px, 24px and 3px.
- Don't use #616161 for body text; it reaches 2.40:1 on #002948. Keep it for large text or metadata.
- Don't introduce new font families beyond Segoe UI Variable Display, Segoe UI Variable Text and Segoe UI.
- Don't use #0078D4 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.125s, 0.2s. Longer ambient animations run 1.2s, 0.8s, 2.4s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/azure.microsoft.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

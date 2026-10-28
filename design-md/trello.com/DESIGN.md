---
version: alpha
name: Trello
description: "Light interface measured from trello.com: Charlie Display type with Charlie Text, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F4F5F7"
  surface: "#F4F5F7"
  on-surface: "#091E42"
  on-background: "#091E42"
  on-surface-strong: "#000000"
  on-surface-variant: "#172B4D"
  surface-container-low: "#F0F0F0"
  surface-container: "#FFFFFF"
  surface-container-high: "#DEEBFF"
  outline: "#FFFFFF"
  outline-variant: "#DFE1E6"
  primary: "#0065FF"
  on-primary: "#FFFFFF"
  secondary: "#0052CC"
  tertiary: "#253858"
typography:
  headline-display:
    fontFamily: Charlie Display
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.25
  headline-lg:
    fontFamily: Charlie Display
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.33
  headline-md:
    fontFamily: Charlie Display
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
  body-md:
    fontFamily: Charlie Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Charlie Display
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
  body-sm:
    fontFamily: Charlie Text
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Charlie Text
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Charlie Display
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
  headline-display-mobile:
    fontFamily: Charlie Display
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: Charlie Display
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
rounded:
  md: 4.8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: 0px
    padding: 8px 24px
    height: 60px
  button-primary-hover:
    backgroundColor: "#0747A6"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 20px 16px 16px 16px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 11.2px 12px 12.8px 12px
  link:
    textColor: "{colors.on-primary}"
---

# Trello Design System

## Overview

Trello describes itself as: “Make the impossible, possible with Trello. The ultimate tool to boost your productivity. Escape the clutter and chaos—stay efficient with Inbox, Boards, and Planner from anywhere, even on mobile.” The interface is light, built on **Snow (#F4F5F7)** with **Deep Blue (#091E42)** text, and **Vivid Blue (#0065FF)** as the main accent.

Type is set in **Charlie Display** and **Charlie Text**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [trello.com](https://trello.com/) on October 21, 2026 at 1440×900 and 390×844 from 196 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#F4F5F7):** Page background, seen 2 times. Token `background`.
- **Deep Blue (#091E42):** Primary text and headings, seen 34 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Deep Blue (#172B4D):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Mist (#F0F0F0):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 6 times. Token `surface-container`.
- **Pale Blue (#DEEBFF):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White (#FFFFFF):** Borders and dividers, seen 5 times. Token `outline`.
- **Cool Mist (#DFE1E6):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Blue (#0065FF):** Primary buttons and calls to action, seen 9 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#0052CC):** Brand color in the logo, seen 30 times. Token `secondary`.
- **Dark Blue (#253858):** Brand color in the logo, seen 15 times. Token `tertiary`.

## Typography

**Charlie Display** and **Charlie Text** share the interface. Fallback stack: `Charlie Display, sans-serif`.

- **headline-display:** Charlie Display 48px at weight 500, line height 1.25 (32px on mobile). Page title (h1).
- **headline-lg:** Charlie Display 36px at weight 500, line height 1.33 (24px on mobile). Section headings (h2).
- **headline-md:** Charlie Display 24px at weight 500, line height 1.33. Sub-section headings.
- **body-md:** Charlie Text 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Charlie Display 20px at weight 500, line height 1.2. Lead paragraphs.
- **body-sm:** Charlie Text 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** Charlie Text 20px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Charlie Display 16px at weight 500, line height 1.25. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (90% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(9, 30, 66, 0.15) 0px 8px 16px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4.8px):** 76 elements.
- **full (9999px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Trello for free”):** #0065FF fill, #FFFFFF text, 19.2px/400, padding 8px 24px.
- **button-primary-hover:** background #0747A6, text #FFFFFF on hover.
- **button-ghost (“Features”):** transparent fill, #172B4D text, 16px/400, padding 20px 16px 16px 16px.
- **input-field (“Email”):** #FFFFFF fill, #000000 text, 16px/400, 4.8px radius, padding 11.2px 12px 12.8px 12px, border 1px solid #DFE1E6.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #F4F5F7 for the page and lift surfaces in small steps: #F0F0F0, #FFFFFF, #DEEBFF.
- Do keep text in 3 levels: #091E42, #000000, #172B4D.
- Do reserve #0065FF for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4.8px corners.
- Don't introduce new font families beyond Charlie Display and Charlie Text.
- Don't use #0065FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.25s, 0.3s, 0.15s.

- **Easing:** `ease-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/trello.com/), the free DESIGN.md generator.

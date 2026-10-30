---
version: alpha
name: Atlassian
description: "Light interface measured from atlassian.com: Charlie Display type with Charlie Text, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#292A2E"
  on-background: "#292A2E"
  on-surface-strong: "#101214"
  on-surface-variant: "#1C2B42"
  surface-container-low: "#F8F8F8"
  outline: "#FFAB00"
  primary: "#1868DB"
  on-primary: "#FFFFFF"
  secondary: "#7EE2B8"
  tertiary: "#BAF3DB"
typography:
  headline-display:
    fontFamily: Charlie Display
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.04
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Charlie Display
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Charlie Display
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Charlie Display
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.24
  title-lg:
    fontFamily: Charlie Display
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.36
    letterSpacing: -0.01em
  body-md:
    fontFamily: Charlie Text
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: Charlie Text
    fontSize: 18px
    fontWeight: 400
  body-sm:
    fontFamily: Charlie Display
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.03em
  caption:
    fontFamily: Charlie Text
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.56
  label-lg:
    fontFamily: Charlie Text
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1
  label-md:
    fontFamily: Charlie Text
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Charlie Display
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0.067em
  headline-display-mobile:
    fontFamily: Charlie Display
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.04
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Charlie Display
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.02em
  headline-sm-mobile:
    fontFamily: Charlie Display
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.24
rounded:
  sm: 3px
  md: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 40px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.full}"
    padding: 10px 26px
    height: 48px
  button-primary-hover:
    backgroundColor: "#123263"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    padding: 8px
    height: 40px
  button-outline-hover:
    textColor: "{colors.primary}"
  button-secondary:
    backgroundColor: "#DDDEE1"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    padding: 0px
    height: 40px
  input-field:
    textColor: "#42526E"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Atlassian Design System

## Overview

Atlassian describes itself as: “Atlassian's team collaboration software like Jira, Confluence and Trello help teams organize, discuss, and complete shared work.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#292A2E)** text, and **Vivid Blue (#1868DB)** as the main accent.

Type is set in **Charlie Display** and **Charlie Text**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [atlassian.com](https://www.atlassian.com/) on October 29, 2026 at 1440×900 and 390×844 from 400 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--ds-background-input-pressed`.
- **Graphite (#292A2E):** Primary text and headings, seen 23 times. Token `on-surface`, CSS `--wac-color-body`.
- **Charcoal (#101214):** Headings and emphasis, seen 69 times. Token `on-surface-strong`.
- **Deep Blue (#1C2B42):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Snow (#F8F8F8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Vivid Amber (#FFAB00):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Blue (#1868DB):** Primary buttons and calls to action, seen 19 times. Token `primary`, CSS `--ds-chart-information-hovered`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Teal (#7EE2B8):** Accent (CSS variable). Token `secondary`.
- **Light Teal (#BAF3DB):** Accent (CSS variable). Token `tertiary`.

## Typography

**Charlie Display** and **Charlie Text** share the interface. Fallback stack: `Charlie Display, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: Atlassian Mono.

- **headline-display:** Charlie Display 64px at weight 500, line height 1.04, tracking -0.02em (44px on mobile). Page title (h1).
- **headline-lg:** Charlie Display 48px at weight 500, line height 1.16, tracking -0.02em (32px on mobile). Section headings (h2).
- **headline-md:** Charlie Display 40px at weight 500, line height 1.2, tracking -0.01em. Sub-section headings.
- **headline-sm:** Charlie Display 32px at weight 500, line height 1.24 (20px on mobile). Card and feature titles.
- **title-lg:** Charlie Display 24px at weight 400, line height 1.36, tracking -0.01em. Small titles.
- **body-md:** Charlie Text 16px at weight 400. Body text.
- **body-lg:** Charlie Text 18px at weight 400. Lead paragraphs.
- **body-sm:** Charlie Display 14px at weight 400, line height 1, tracking 0.03em. Secondary and small text.
- **caption:** Charlie Text 12px at weight 400, line height 1.56. Captions and fine print.
- **label-lg:** Charlie Text 14px at weight 700, line height 1. Large buttons and tabs.
- **label-md:** Charlie Text 13px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Charlie Display 12px at weight 500, line height 1.3, tracking 0.067em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 40px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F8F8F8) and #FFAB00 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 44 elements.
- **sm (3px):** 36 elements.
- **md (20px):** 36 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started with Jira”):** #1868DB fill, #FFFFFF text, 20px/400, 10000px radius, padding 10px 26px.
- **button-primary-hover:** background #123263, text #FFFFFF on hover.
- **button-outline (“search”):** #F8F8F8 fill, #101214 text, 13.3333px/400, 50% radius, padding 8px.
- **button-outline-hover:** background #F8F8F8, text #1868DB on hover.
- **button-secondary (“Pause video”):** #DDDEE1 fill, #101214 text, 13.3333px/400, 100% radius, padding 0px.
- **input-field (“Choose your language”):** transparent fill, #42526E text, 14px/400, padding 0px.
- **link:** transparent fill, #101214 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F8F8.
- Do keep text in 3 levels: #292A2E, #101214, #1C2B42.
- Do reserve #1868DB for primary actions and key highlights.
- Do set headlines in Charlie Display with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 3px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Charlie Display and Charlie Text.
- Don't use #1868DB for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.25s, 0.3s, 0.5s.

- **Easing:** `cubic-bezier(0.4, 0, 0, 1)`, `ease-in-out`, `cubic-bezier(0.6, 0.01, 0.8, 0.6)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/atlassian.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).

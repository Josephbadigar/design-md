---
version: alpha
name: HubSpot
description: "Light interface measured from hubspot.com: HubSpot Serif type with HubSpot Sans, vivid orange accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F1F1F"
  on-background: "#1F1F1F"
  on-surface-strong: "#000000"
  on-surface-variant: "#616161"
  surface-container-low: "#FCFCFA"
  overlay: "#0000001C"
  outline: "#0000001C"
  outline-variant: "#FFFFFF66"
  primary: "#FF4800"
  on-primary: "#FFFFFF"
  secondary: "#FCC6B1"
  tertiary: "#800051"
typography:
  headline-display:
    fontFamily: HubSpot Serif
    fontSize: 65px
    fontWeight: 300
    lineHeight: 1.2
  headline-lg:
    fontFamily: HubSpot Serif
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
  headline-md:
    fontFamily: HubSpot Serif
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.1
  headline-sm:
    fontFamily: HubSpot Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.42
  title-lg:
    fontFamily: HubSpot Sans
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.6
  body-md:
    fontFamily: HubSpot Sans
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.75
  body-lg:
    fontFamily: HubSpot Sans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.56
  body-sm:
    fontFamily: HubSpot Sans
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.57
  caption:
    fontFamily: HubSpot Sans
    fontSize: 13px
    fontWeight: 300
    lineHeight: 1.5
  label-lg:
    fontFamily: HubSpot Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.75
  label-md:
    fontFamily: HubSpot Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.57
  label-sm:
    fontFamily: HubSpot Sans
    fontSize: 12px
    fontWeight: 500
  headline-display-mobile:
    fontFamily: HubSpot Serif
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.05
rounded:
  sm: 4px
  md: 8px
  lg: 16px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 12px 24px
    height: 56px
  button-primary-hover:
    backgroundColor: "#C93700"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 16px
    height: 46px
  button-outline-hover:
    backgroundColor: "{colors.background}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 3.2px 8px
  card:
    backgroundColor: "#061C1D"
    textColor: "#F8F5EE"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# HubSpot Design System

## Overview

HubSpot describes itself as: “HubSpot's customer platform includes all the marketing, sales, customer service, and CRM software you need to grow your business.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1F1F1F)** text, and **Vivid Orange (#FF4800)** as the main accent.

Type is set in **HubSpot Serif** and **HubSpot Sans**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [hubspot.com](https://www.hubspot.com/) on October 21, 2026 at 1440×900 and 390×844 from 399 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 28 times. Token `background`, CSS `--cl-color-container-01`.
- **Charcoal (#1F1F1F):** Primary text and headings, seen 122 times. Token `on-surface`, CSS `--light-theme-pressed-link-01`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Slate (#616161):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--cl-color-social-button-fill-hover`.
- **Snow (#FCFCFA):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`.
- **Near Black 11% (#0000001C):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 11% (#0000001C):** Borders and dividers, seen 25 times. Token `outline`.
- **White 40% (#FFFFFF66):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--dark-theme-text-placeholder-01`.
- **Vivid Orange (#FF4800):** Primary buttons and calls to action, seen 16 times. Token `primary`, CSS `--cl-color-button-primary-fill-idle`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Orange (#FCC6B1):** Brand accent (CSS variable), seen 24 times. Token `secondary`.
- **Dark Pink (#800051):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.

## Typography

**HubSpot Serif** and **HubSpot Sans** share the interface. Fallback stack: `HubSpot Serif, serif`.

- **headline-display:** HubSpot Serif 65px at weight 300, line height 1.2 (40px on mobile). Page title (h1).
- **headline-lg:** HubSpot Serif 40px at weight 300, line height 1.1. Section headings (h2).
- **headline-md:** HubSpot Serif 28px at weight 300, line height 1.1. Sub-section headings.
- **headline-sm:** HubSpot Sans 24px at weight 500, line height 1.42. Card and feature titles.
- **title-lg:** HubSpot Sans 22px at weight 500, line height 1.6. Small titles.
- **body-md:** HubSpot Sans 16px at weight 300, line height 1.75. Body text.
- **body-lg:** HubSpot Sans 18px at weight 500, line height 1.56. Lead paragraphs.
- **body-sm:** HubSpot Sans 14px at weight 300, line height 1.57. Secondary and small text.
- **caption:** HubSpot Sans 13px at weight 300, line height 1.5. Captions and fine print.
- **label-lg:** HubSpot Sans 16px at weight 500, line height 1.75. Large buttons and tabs.
- **label-md:** HubSpot Sans 14px at weight 500, line height 1.57. Buttons, navigation and labels.
- **label-sm:** HubSpot Sans 12px at weight 500. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 61% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 16px, lg 32px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 450px, 568px, 800px, 850px, 1080px, 1152px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(33, 51, 67, 0.12) 0px 2px 4px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 108 elements.
- **lg (16px):** 36 elements.
- **full (9999px):** 20 elements.
- **sm (4px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get a demo of HubSpot's software”):** #FF4800 fill, #FFFFFF text, 16px/500, 8px radius, padding 12px 24px.
- **button-primary-hover:** background #C93700, text #FFFFFF on hover.
- **button-outline (“Accept All”):** #FFFFFF fill, #1F1F1F text, 14px/500, 8px radius, padding 8px 16px.
- **button-outline-hover:** background #FFFFFFE6, text #1F1F1F on hover.
- **button-ghost (“Select a language”):** transparent fill, #1F1F1F text, 16px/400, padding 0px.
- **input-field (“Search HubSpot”):** transparent fill, #1F1F1F text, 16px/300, 4px radius, padding 3.2px 8px.
- **card:** #061C1D fill, #F8F5EE text, 16px/300, padding 0px.
- **link:** transparent fill, #FFFFFF9E text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FCFCFA.
- Do keep text in 3 levels: #1F1F1F, #000000, #616161.
- Do reserve #FF4800 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 16px and 4px.
- Don't introduce new font families beyond HubSpot Serif and HubSpot Sans.
- Don't use #FF4800 for large backgrounds or body text.
- Don't make interface transitions slower than 0.001s.

## Motion

Interface transitions are quick: 0.001s.

- **Easing:** `ease`, `linear`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/hubspot.com/), the free DESIGN.md generator.

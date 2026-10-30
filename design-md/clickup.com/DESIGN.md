---
version: alpha
name: ClickUp
description: "Light interface measured from clickup.com: Plus Jakarta Sans type with Inter, vivid amber accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#646464"
  on-background: "#646464"
  on-surface-strong: "#202020"
  on-surface-variant: "#8A8A94"
  on-surface-muted: "#B4B4B4"
  surface-container-low: "#E7F9F5"
  surface-container: "#FEEFF6"
  surface-container-high: "#F0F0F0"
  surface-container-highest: "#ECECEF"
  overlay: "#0000000F"
  outline: "#E8E8E8"
  outline-variant: "#D9D9D9"
  primary: "#FFC53D"
  on-primary: "#000000"
  secondary: "#12A594"
  tertiary: "#0091FF"
typography:
  headline-display:
    fontFamily: Plus Jakarta Sans
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: 650
    lineHeight: 1.25
    letterSpacing: -0.035em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: 650
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 26px
    fontWeight: 650
    lineHeight: 1.25
    letterSpacing: -0.035em
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.02em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.016em
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.47
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  code:
    fontFamily: Sometype Mono
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
  headline-display-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 34px
    fontWeight: 650
    lineHeight: 1.18
    letterSpacing: -0.047em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 34px
    fontWeight: 650
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: 650
    lineHeight: 1.21
    letterSpacing: -0.027em
rounded:
  xs: 6px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 54px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 10px
  lg: 24px
  xl: 56px
  gutter: 10px
  section: 80px
  margin: 20px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 32px
  button-primary-hover:
    backgroundColor: "#202020CC"
  button-outline:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xl}"
    padding: 4px 12px
    height: 30px
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 32px
  card:
    backgroundColor: "{colors.on-primary}"
    textColor: "#292D34"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 0px 80px 0px
  link:
    textColor: "{colors.on-surface}"
---

# ClickUp Design System

## Overview

ClickUp describes itself as: “Our mission is to make the world more productive. To do this, we built the everything app for work - Tasks, Docs, Goals, and Chat.” The interface is light, built on **White (#FFFFFF)** with **Slate (#646464)** text, and **Vivid Amber (#FFC53D)** as the main accent.

Type is set in **Plus Jakarta Sans** and **Inter**, with **Sometype Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [clickup.com](https://clickup.com/) on October 29, 2026 at 1440×900 and 390×844 from 435 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #0091FF, #A43CB4, #F100E3, #FA24CE.

- **White (#FFFFFF):** Page background, seen 57 times. Token `background`, CSS `--color-core-utilities-white`.
- **Slate (#646464):** Primary text and headings, seen 25 times. Token `on-surface`, CSS `--Core-Text-Secondary`.
- **Charcoal (#202020):** Headings and emphasis, seen 7 times. Token `on-surface-strong`, CSS `--color-core-text-main`.
- **Cool Gray (#8A8A94):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Gray (#B4B4B4):** Muted text and metadata, seen 9 times. Token `on-surface-muted`.
- **Pale Teal (#E7F9F5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Warm Snow (#FEEFF6):** Cards and panels, seen 1 time. Token `surface-container`.
- **Mist (#F0F0F0):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Mist (#ECECEF):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 6% (#0000000F):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Mist (#E8E8E8):** Borders and dividers, seen 49 times. Token `outline`, CSS `--color-motion-button-border`.
- **Silver (#D9D9D9):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Amber (#FFC53D):** Brand accent (CSS variable), seen 1 time. Token `primary`, CSS `--color-motion-event-yellow-bar`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#12A594):** Accent (CSS variable). Token `secondary`.
- **Vivid Blue (#0091FF):** Accent in text, fills and borders, seen 5 times. Token `tertiary`, CSS `--color-team-tabs-tab-active-border`.

## Typography

**Plus Jakarta Sans**, **Inter** and **Sometype Mono** (monospace) share the interface. Fallback stack: `Plus Jakarta Sans`.

- **headline-display:** Plus Jakarta Sans 60px at weight 700, line height 1.1, tracking -0.035em (34px on mobile). Page title (h1).
- **headline-lg:** Plus Jakarta Sans 48px at weight 650, line height 1.25, tracking -0.035em (34px on mobile). Section headings (h2).
- **headline-md:** Plus Jakarta Sans 40px at weight 650, line height 1.2, tracking -0.04em. Sub-section headings.
- **headline-sm:** Plus Jakarta Sans 26px at weight 650, line height 1.25, tracking -0.035em (15px on mobile). Card and feature titles.
- **body-md:** Plus Jakarta Sans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 500, line height 1.33, tracking -0.02em. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Inter 16px at weight 500, line height 1.33, tracking -0.016em. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500, line height 1.47, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1. Small labels and badges.
- **code:** Sometype Mono 14px at weight 500, line height 1.29. Code and technical values.

## Layout

Spacing does not follow a strict grid: 50% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 5px, md 10px, lg 24px, xl 56px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 400px, 500px, 600px, 768px, 900px, 1000px, 1100px, 1160px, 1200px, 1400px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0.55) 0px -13px 32px 0px`
- `rgba(0, 0, 0, 0.55) 0px -12px 29px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 44 elements.
- **md (12px):** 44 elements.
- **xs (6px):** 28 elements.
- **xl (54px):** 28 elements.
- **full (9999px):** 16 elements.
- **lg (16px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #202020 fill, #FFFFFF text, 14px/600, 8px radius, padding 8px 12px.
- **button-primary-hover:** background #202020CC, text #FFFFFF on hover.
- **button-outline (“The Best AI is”):** #E8E8E8 fill, #202020 text, 14px/600, 54px radius, padding 4px 12px.
- **button-ghost (“Login”):** #F0F0F0 fill, #000000 text, 14px/600, 8px radius, padding 8px 12px.
- **card:** #000000 fill, #292D34 text, 16px/400, padding 0px 0px 80px 0px.
- **link:** transparent fill, #646464 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #E7F9F5, #FEEFF6, #F0F0F0, #ECECEF.
- Do keep text in 4 levels: #646464, #202020, #8A8A94, #B4B4B4.
- Do use #FFC53D as the brand accent: header, logo and key highlights.
- Do set headlines in Plus Jakarta Sans with tight tracking (-0.035em).
- Do reuse the measured spacing steps (5px, 10px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 12px, 6px and 54px.
- Don't use #8A8A94 for body text; it reaches 3.42:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use #B4B4B4 for body text; it reaches 2.07:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Plus Jakarta Sans, Inter and Sometype Mono.
- Don't use #FFC53D for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.25s, 0.2s, 0.3s, 0.16s.

- **Easing:** `cubic-bezier(0.5, 0, 0.5, 1)`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/clickup.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).

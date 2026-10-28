---
version: alpha
name: Fly.io
description: "Light interface measured from fly.io: Mackinac type with Fricolage Grotesque, vivid violet accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F4F6EB"
  surface: "#F4F6EB"
  on-surface: "#5B5077"
  on-background: "#5B5077"
  on-surface-strong: "#281950"
  on-surface-variant: "#686082"
  on-surface-muted: "#A39AC1"
  surface-container-low: "#FFFFFF"
  overlay: "#F4F3FBBF"
  overlay-strong: "#FFFFFF66"
  outline: "#FFFFFF40"
  outline-variant: "#E6E0FE"
  primary: "#7C3AED"
  on-primary: "#FFFFFF"
  secondary: "#CAE3FD"
  success: "#10B981"
  error: "#CC0000"
  link: "#281950BF"
typography:
  headline-display:
    fontFamily: Mackinac
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.045em
  headline-lg:
    fontFamily: Mackinac
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.025em
  body-md:
    fontFamily: Fricolage Grotesque
    fontSize: 16px
    fontWeight: 325
    lineHeight: 1.5
  body-lg:
    fontFamily: Fricolage Grotesque
    fontSize: 19px
    fontWeight: 325
    lineHeight: 1.5
  body-sm:
    fontFamily: Fricolage Grotesque
    fontSize: 14.5px
    fontWeight: 450
    lineHeight: 1.66
  label-lg:
    fontFamily: Fricolage Grotesque
    fontSize: 15px
    fontWeight: 450
    lineHeight: 1.5
  label-md:
    fontFamily: Fricolage Grotesque
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Fricolage Grotesque
    fontSize: 12px
    fontWeight: 575
    lineHeight: 1.5
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Mackinac
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.045em
  headline-lg-mobile:
    fontFamily: Mackinac
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.32
    letterSpacing: -0.025em
rounded:
  xs: 6px
  sm: 8px
  md: 10px
  lg: 16px
  xl: 20px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  gutter: 32px
  section: 128px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px 0px 10px
    height: 32px
  button-primary-hover:
    backgroundColor: "#6D28D9"
  button-outline:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "#202237"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xl}"
    padding: 0px 10px 0px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "#F5F3FF66"
    textColor: "{colors.primary}"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xs}"
    padding: 4px 12px
  input-field:
    backgroundColor: "#22183C"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
  link:
    textColor: "{colors.link}"
---

# Fly.io Design System

## Overview

Fly.io describes itself as: “Deploy apps, agents, and databases on fast, hardware-isolated VMs. Pay only for the seconds they run. Sign up free.” The interface is light, built on **Mist (#F4F6EB)** with **Violet (#5B5077)** text, and **Vivid Violet (#7C3AED)** as the main accent.

Type is set in **Mackinac** and **Fricolage Grotesque**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [fly.io](https://fly.io/) on October 21, 2026 at 1440×900 and 390×844 from 325 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #A02BE4, #4F46E5, #7C3AED, #8919C9.

- **Mist (#F4F6EB):** Page background. Token `background`.
- **Violet (#5B5077):** Primary text and headings. Token `on-surface`.
- **Deep Violet (#281950):** Headings and emphasis, seen 21 times. Token `on-surface-strong`.
- **Violet (#686082):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Violet (#A39AC1):** Muted text and metadata, seen 23 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **Cool Snow 75% (#F4F3FBBF):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 40% (#FFFFFF66):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 25% (#FFFFFF40):** Borders and dividers, seen 10 times. Token `outline`.
- **Pale Violet (#E6E0FE):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Violet (#7C3AED):** Primary buttons and calls to action, seen 13 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pale Blue (#CAE3FD):** Brand color in logos and imagery, seen 27 times. Token `secondary`.
- **Teal (#10B981):** Success and positive states, seen 5 times. Token `success`.
- **Red (#CC0000):** Errors and destructive states, seen 1 time. Token `error`.
- **Deep Violet 75% (#281950BF):** Inline links, seen 26 times. Token `link`.

## Typography

**Mackinac** and **Fricolage Grotesque** share the interface. Fallback stack: `Mackinac, ui-serif, Georgia, Cambria`. Other loaded fonts: Fragment Mono.

- **headline-display:** Mackinac 64px at weight 500, line height 1.15, tracking -0.045em (32px on mobile). Page title (h1).
- **headline-lg:** Mackinac 36px at weight 500, line height 1.33, tracking -0.025em (24px on mobile). Section headings (h2).
- **body-md:** Fricolage Grotesque 16px at weight 325, line height 1.5. Body text.
- **body-lg:** Fricolage Grotesque 19px at weight 325, line height 1.5. Lead paragraphs.
- **body-sm:** Fricolage Grotesque 14.5px at weight 450, line height 1.66. Secondary and small text.
- **label-lg:** Fricolage Grotesque 15px at weight 450, line height 1.5. Large buttons and tabs.
- **label-md:** Fricolage Grotesque 14.5px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Fricolage Grotesque 12px at weight 575, line height 1.5, tracking 0.05em, uppercase. Small labels and badges.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 64px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Breakpoints:** 480px, 640px, 767px, 768px, 1023px, 1024px, 1200px, 1367px, 1400px, 1500px, 1600px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(91, 33, 182, 0.1) 0px 5px 5px -2px, rgba(91, 33, 182, 0.1) 0px 2px 4px -2px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(255, 255, 255, 0.3) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.2) 0px 10px 15px -3px, rgba(0, 0, 0, 0.2) 0px 4px 6px -4px`

Hairline rings and inset highlights also appear: `rgba(67, 56, 202, 0.25) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **lg (16px):** 36 elements.
- **sm (8px):** 20 elements.
- **full (9999px):** 20 elements.
- **md (10px):** 12 elements.
- **xs (6px):** 4 elements.
- **xl (20px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #7C3AED fill, #FFFFFF text, 14.5px/450, 8px 20px 20px 8px radius, padding 0px 12px 0px 10px, shadow `rgba(67, 56, 202, 0.25) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-primary-hover:** background #6D28D9, text #FFFFFF on hover.
- **button-outline (“Log In”):** #FFFFFF66 fill, #202237 text, 14.5px/450, 20px 8px 8px 20px radius, padding 0px 10px 0px 12px, border 1px solid #FFFFFFE6, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-outline-hover:** background #F5F3FF66, text #7C3AED on hover.
- **button-ghost (“Onboard your agent”):** transparent fill, #686082 text, 15px/450, 6px radius, padding 4px 12px.
- **input-field (“Your name”):** #22183C fill, #FFFFFF text, 14.5px/325, 8px radius, padding 8px 12px, border 1px solid #42385F.
- **link:** transparent fill, #281950BF text, padding 0px.

## Do's and Don'ts

- Do use #F4F6EB for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #5B5077, #281950, #686082, #A39AC1.
- Do reserve #7C3AED for primary actions and key highlights.
- Do set headlines in Mackinac with tight tracking (-0.045em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't use #A39AC1 for body text; it reaches 2.4:1 on #F4F6EB. Keep it for large text or metadata.
- Don't introduce new font families beyond Mackinac and Fricolage Grotesque.
- Don't use #7C3AED for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fly.io/), the free DESIGN.md generator.

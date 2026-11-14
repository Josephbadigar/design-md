---
version: alpha
name: Stripe
description: "Light interface measured from stripe.com: sohne-var type, vivid indigo accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#061B31"
  on-surface-muted: "#50617A"
  on-surface-subtle: "#64748D"
  surface-container-low: "#F8FAFD"
  surface-container: "#F5F5FF"
  surface-container-high: "#ECEDFE"
  surface-container-highest: "#E5EDF5"
  overlay: "#FFFFFFA6"
  outline: "#E5EDF5"
  outline-variant: "#E2E4FF"
  primary: "#533AFD"
  on-primary: "#FFFFFF"
  secondary: "#0A2540"
  tertiary: "#1C1E54"
typography:
  headline-display:
    fontFamily: sohne-var
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: sohne-var
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: sohne-var
    fontSize: 26px
    fontWeight: 300
    lineHeight: 1.12
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: sohne-var
    fontSize: 22px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.01em
  body-md:
    fontFamily: sohne-var
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.25
  body-lg:
    fontFamily: sohne-var
    fontSize: 18px
    fontWeight: 300
    lineHeight: 1.4
  body-sm:
    fontFamily: sohne-var
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
  caption:
    fontFamily: sohne-var
    fontSize: 12px
    fontWeight: 300
    lineHeight: 1.45
  label-md:
    fontFamily: sohne-var
    fontSize: 16px
    fontWeight: 400
  headline-display-mobile:
    fontFamily: sohne-var
    fontSize: 34px
    fontWeight: 300
    lineHeight: 1.03
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: sohne-var
    fontSize: 22px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: sohne-var
    fontSize: 20px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 6px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 8px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 11.5px 20px 12.5px 20px
    height: 40px
  button-primary-hover:
    backgroundColor: "#4032C8"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 14.5px 24px 15.5px 24px
    height: 48px
  button-outline-hover:
    textColor: "#2E2B8C"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 0px 24px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 12px 0px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 11px 17px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Stripe Design System

## Overview

Stripe describes itself as: “Stripe is a financial services platform that helps all types of businesses accept payments, build flexible billing models, and manage money movement.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Indigo (#533AFD)** as the main accent.

Type is set in **sohne-var**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [stripe.com](https://stripe.com/) on November 13, 2026 at 1440×900 and 390×844 from 474 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #DA4BFECC, #FF8C6CCC, #4304EA, #715CFFCC.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`, CSS `--hds-color-util-bg-min`.
- **Near Black (#000000):** Primary text and headings, seen 19 times. Token `on-surface`.
- **Deep Blue (#061B31):** Secondary text, seen 73 times. Token `on-surface-variant`, CSS `--hds-color-heading-solid`.
- **Blue (#50617A):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Blue (#64748D):** Subtle text and placeholders, seen 34 times. Token `on-surface-subtle`, CSS `--hds-color-heading-subdued`.
- **Snow (#F8FAFD):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--hds-color-util-bg-quiet`.
- **Cool Snow (#F5F5FF):** Cards and panels, seen 2 times. Token `surface-container`.
- **Pale Indigo (#ECEDFE):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Cool Mist (#E5EDF5):** Highest raised elements, seen 8 times. Token `surface-container-highest`, CSS `--hds-color-util-neutral-50`.
- **White 65% (#FFFFFFA6):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--hds-color-action-bg-translucent`.
- **Cool Mist (#E5EDF5):** Borders and dividers, seen 4 times. Token `outline`, CSS `--hds-color-util-neutral-50`.
- **Pale Indigo (#E2E4FF):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Indigo (#533AFD):** Primary buttons and calls to action, seen 21 times. Token `primary`, CSS `--hds-color-accent-border-solid`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#0A2540):** Secondary buttons. Token `secondary`.
- **Deep Indigo (#1C1E54):** Accent (CSS variable). Token `tertiary`.

## Typography

**sohne-var** carries the whole interface. Fallback stack: `sohne-var, SF Pro Display, sans-serif`. Other loaded fonts: SourceCodePro.

- **headline-display:** sohne-var 48px at weight 300, line height 1.15, tracking -0.02em (34px on mobile). Page title (h1).
- **headline-lg:** sohne-var 32px at weight 300, line height 1.1, tracking -0.02em (22px on mobile). Section headings (h2).
- **headline-md:** sohne-var 26px at weight 300, line height 1.12, tracking -0.01em (20px on mobile). Sub-section headings.
- **headline-sm:** sohne-var 22px at weight 300, line height 1.1, tracking -0.01em. Card and feature titles.
- **body-md:** sohne-var 16px at weight 300, line height 1.25. Body text.
- **body-lg:** sohne-var 18px at weight 300, line height 1.4. Lead paragraphs.
- **body-sm:** sohne-var 14px at weight 400, line height 1. Secondary and small text.
- **caption:** sohne-var 12px at weight 300, line height 1.45. Captions and fine print.
- **label-md:** sohne-var 16px at weight 400. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F8FAFD → #F5F5FF → #ECEDFE → #E5EDF5) and #E5EDF5 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 136 elements.
- **md (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact sales”):** #533AFD fill, #FFFFFF text, 14px/400, 4px radius, padding 11.5px 20px 12.5px 20px.
- **button-primary-hover:** background #4032C8, text #FFFFFF on hover.
- **button-outline (“Sign up with Google”):** #FFFFFFA6 fill, #533AFD text, 16px/400, 4px radius, padding 14.5px 24px 15.5px 24px, border 1px solid #B9B9F9.
- **button-outline-hover:** background #FFFFFFA6, text #2E2B8C on hover.
- **button-secondary (“Chat now with sales”):** #0A2540 fill, #FFFFFF text, 15px/400, 4px radius, padding 0px 24px, border 1px solid #FFFFFF1F.
- **button-ghost (“Products”):** transparent fill, #061B31 text, 14px/400, 4px radius, padding 12px 0px.
- **input-field (“Sell software subscriptions to o”):** #FFFFFF fill, #000000 text, 16px/300, padding 11px 17px.
- **link:** transparent fill, #061B31 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8FAFD, #F5F5FF, #ECEDFE, #E5EDF5.
- Do keep text in 4 levels: #000000, #061B31, #50617A, #64748D.
- Do reserve #533AFD for primary actions and key highlights.
- Do set headlines in sohne-var with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 6px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond sohne-var.
- Don't use #533AFD for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.24s, 0.4s. Longer ambient animations run 0.8s, 1.2s.

- **Easing:** `cubic-bezier(0.25, 1, 0.5, 1)`, `linear`, `cubic-bezier(0.45, 0.05, 0.55, 0.95)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/stripe.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).

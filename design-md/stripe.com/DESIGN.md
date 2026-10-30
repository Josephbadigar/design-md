---
version: alpha
name: Stripe
description: "Light interface measured from stripe.com: sohne-var type, vivid indigo accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#061B31"
  on-background: "#061B31"
  on-surface-strong: "#000000"
  on-surface-variant: "#50617A"
  on-surface-muted: "#64748D"
  surface-container-low: "#F8FAFD"
  surface-container: "#F5F5FF"
  surface-container-high: "#E5EDF5"
  surface-container-highest: "#E8E9FF"
  overlay: "#FFFFFFA6"
  outline: "#E5EDF5"
  outline-variant: "#E2E4FF"
  primary: "#533AFD"
  on-primary: "#FFFFFF"
  secondary: "#1C1E54"
  tertiary: "#FF6118"
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
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 10.5px 20px 13.5px 20px
    height: 40px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 15px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Stripe Design System

## Overview

Stripe describes itself as: “Stripe is a financial services platform that helps all types of businesses accept payments, build flexible billing models, and manage money movement.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#061B31)** text, and **Vivid Indigo (#533AFD)** as the main accent.

Type is set in **sohne-var**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [stripe.com](https://stripe.com/) on October 30, 2026 at 1440×900 and 390×844 from 470 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #DA4BFECC, #FF8C6CCC, #8A35DF, #715CFFCC.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`, CSS `--hds-color-util-bg-min`.
- **Deep Blue (#061B31):** Primary text and headings, seen 76 times. Token `on-surface`, CSS `--hds-color-heading-solid`.
- **Near Black (#000000):** Headings and emphasis, seen 17 times. Token `on-surface-strong`.
- **Blue (#50617A):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Blue (#64748D):** Muted text and metadata, seen 31 times. Token `on-surface-muted`, CSS `--hds-color-heading-subdued`.
- **Snow (#F8FAFD):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--hds-color-util-bg-quiet`.
- **Cool Snow (#F5F5FF):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Mist (#E5EDF5):** Hover and pressed fills, seen 7 times. Token `surface-container-high`, CSS `--hds-color-util-neutral-50`.
- **Pale Indigo (#E8E9FF):** Highest raised elements, seen 3 times. Token `surface-container-highest`.
- **White 65% (#FFFFFFA6):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--hds-color-action-bg-translucent`.
- **Cool Mist (#E5EDF5):** Borders and dividers, seen 4 times. Token `outline`, CSS `--hds-color-util-neutral-50`.
- **Pale Indigo (#E2E4FF):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Indigo (#533AFD):** Primary buttons and calls to action, seen 23 times. Token `primary`, CSS `--hds-color-accent-border-solid`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Indigo (#1C1E54):** Accent (CSS variable). Token `secondary`.
- **Vivid Orange (#FF6118):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

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

Spacing is mostly on a 4px grid (80% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F8FAFD → #F5F5FF → #E5EDF5 → #E8E9FF) and #E5EDF5 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 136 elements.
- **md (6px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact sales”):** #533AFD fill, #FFFFFF text, 14px/400, 4px radius, padding 11.5px 20px 12.5px 20px.
- **button-primary-hover:** background #4032C8, text #FFFFFF on hover.
- **button-outline (“Sign up with Google”):** #FFFFFFA6 fill, #533AFD text, 16px/400, 4px radius, padding 14.5px 24px 15.5px 24px, border 1px solid #B9B9F9.
- **button-outline-hover:** background #FFFFFFA6, text #2E2B8C on hover.
- **button-ghost (“Sign in Sign in”):** transparent fill, #FFFFFF text, 14px/400, 4px radius, padding 10.5px 20px 13.5px 20px, border 1px solid #FFFFFF.
- **input-field (“Enter work email”):** transparent fill, #061B31 text, 16px/300, padding 0px 15px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8FAFD, #F5F5FF, #E5EDF5, #E8E9FF.
- Do keep text in 4 levels: #061B31, #000000, #50617A, #64748D.
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

Generated by [Sitepeel](https://sitepeel.dev/design-md/stripe.com/), the free DESIGN.md generator (engine 2026.10.29+bf9d681d83cf).

---
version: alpha
name: Poimandres
description: "Light monochrome interface measured from pmnd.rs: Inter type, flat surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#555555"
  on-background: "#555555"
  overlay: "#0000001A"
  primary: "#555555"
  on-primary: "#FFFFFF"
  secondary: "#E8756A"
typography:
  body-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.38
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  md: 6px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 24px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 0px
---

# Poimandres Design System

## Overview

Poimandres describes itself as: “Open source developer collective” The interface is light, built on **White (#FFFFFF)** with **Slate (#555555)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter**. Headlines run large; body text is 12px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [pmnd.rs](https://pmnd.rs/) on November 4, 2026 at 1440×900 and 390×844 from 218 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **White (#FFFFFF):** Page background, seen 93 times. Token `background`, CSS `--docsearch-footer-background`.
- **Slate (#555555):** Primary text and headings, seen 4 times. Token `on-surface`.
- **Near Black 10% (#0000001A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Slate (#555555):** Primary actions (the main text color; the palette is monochrome), seen 9 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#E8756A):** Accent, seen 1 time. Token `secondary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, Inter Fallback, ui-sans-serif, system-ui`.

- **body-md:** Inter 12px at weight 400, line height 1.5. Body text.
- **label-lg:** Inter 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 15px at weight 600, line height 1.38. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 24px.
- **Breakpoints:** 768px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, rgba(0, 0, 0, 0.08) 0px 1px 6px 0px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 364 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“HIDE”):** transparent fill, #555555 text, 16px/400, 3.35544e+07px radius, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do let contrast carry emphasis; primary actions use #555555 on #FFFFFF.
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Do use 6px corners on most elements.
- Don't introduce new font families beyond Inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s. Longer ambient animations run 1.078s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `linear(0 0%, 0.0078 0.769231%, 0.034 1.53846%, 0.0738 2.30769%, 0.116 3.07692%, 0.16 3.84615%, 0.203 4.61538%, 0.244 5.38462%, 0.284 6.15385%, 0.322 6.92308%, 0.357 7.69231%, 0.391 8.46154%, 0.422 9.23077%, 0.453 10%, 0.483 10.7692%, 0.51 11.5385%, 0.536 12.3077%, 0.561 13.0769%, 0.583 13.8462%, 0.606 14.6154%, 0.627 15.3846%, 0.646 16.1538%, 0.665 16.9231%, 0.683 17.6923%, 0.7 18.4615%, 0.716 19.2308%, 0.731 20%, 0.745 20.7692%, 0.759 21.5385%, 0.771 22.3077%, 0.784 23.0769%, 0.795 23.8462%, 0.806 24.6154%, 0.816 25.3846%, 0.826 26.1538%, 0.835 26.9231%, 0.844 27.6923%, 0.852 28.4615%, 0.859 29.2308%, 0.867 30%, 0.874 30.7692%, 0.881 31.5385%, 0.887 32.3077%, 0.893 33.0769%, 0.899 33.8462%, 0.904 34.6154%, 0.909 35.3846%, 0.914 36.1538%, 0.919 36.9231%, 0.923 37.6923%, 0.927 38.4615%, 0.931 39.2308%, 0.935 40%, 0.938 40.7692%, 0.941 41.5385%, 0.944 42.3077%, 0.947 43.0769%, 0.95 43.8462%, 0.953 44.6154%, 0.955 45.3846%, 0.958 46.1538%, 0.96 46.9231%, 0.962 47.6923%, 0.964 48.4615%, 0.966 49.2308%, 0.968 50%, 0.969 50.7692%, 0.971 51.5385%, 0.973 52.3077%, 0.974 53.0769%, 0.975 53.8462%, 0.977 54.6154%, 0.978 55.3846%, 0.979 56.1538%, 0.98 56.9231%, 0.981 57.6923%, 0.982 58.4615%, 0.983 59.2308%, 0.984 60%, 0.985 60.7692%, 0.986 61.5385%, 0.987 62.3077%, 0.987 63.0769%, 0.988 63.8462%, 0.989 64.6154%, 0.989 65.3846%, 0.99 66.1538%, 0.99 66.9231%, 0.991 67.6923%, 0.991 68.4615%, 0.992 69.2308%, 0.992 70%, 0.993 70.7692%, 0.993 71.5385%, 0.993 72.3077%, 0.994 73.0769%, 0.994 73.8462%, 0.994 74.6154%, 0.995 75.3846%, 0.995 76.1538%, 0.995 76.9231%, 0.995 77.6923%, 0.996 78.4615%, 0.996 79.2308%, 0.996 80%, 0.996 80.7692%, 0.997 81.5385%, 0.997 82.3077%, 0.997 83.0769%, 0.997 83.8462%, 0.997 84.6154%, 0.997 85.3846%, 0.998 86.1538%, 0.998 86.9231%, 0.998 87.6923%, 0.998 88.4615%, 0.998 89.2308%, 0.998 90%, 0.998 90.7692%, 0.998 91.5385%, 0.998 92.3077%, 0.998 93.0769%, 0.999 93.8462%, 0.999 94.6154%, 0.999 95.3846%, 0.999 96.1538%, 0.999 96.9231%, 0.999 97.6923%, 0.999 98.4615%, 0.999 99.2308%, 1 100%)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pmnd.rs/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).

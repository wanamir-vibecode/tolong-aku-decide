# Design System Anchor: Tolong Aku Decide

This document defines the immutable design tokens, layout constraints, typography, and anti-slop refusals for the "Tolong Aku Decide" mobile web application[cite: 5].

---

## 1. Dial Calibration & Spatial Enclosure

* `DESIGN_VARIANCE: 7` (Punchy kinetic balance without chaotic asymmetry)[cite: 5]
* `MOTION_INTENSITY: 8` (High-speed deceleration physics and spring feedback)[cite: 5]
* `VISUAL_DENSITY: 4` (Generous, thumb-friendly tap surfaces)[cite: 5]

### Viewport Boundary
* Layout enclosure: strictly `max-w-md mx-auto`[cite: 5].
* Vertical framing: `min-h-[100dvh]` (never `h-screen` to prevent iOS Safari address bar jumps)[cite: 5].
* Canvas alignment: vertically centered content flow with safe-area padding (`px-5 py-6`)[cite: 5].

---

## 2. Color Tokens

### Base Foundation
* Canvas Background: `#0f0f11` (Deep off-black; never pure `#000000`)[cite: 5]
* Primary Action Accent: `#ffd02f` (Canary Yellow)
* Contrast Foreground: `#ffffff`
* Subdued Foreground: `#a1a1aa` (Zinc 400)
* Dark Neutral Surface: `#1b1b1f` (Input backgrounds and inactive shells)
* Border Subtle: `#27272a` (Zinc 800)

### Dynamic Option Accents
Assigned sequentially to option cards and used for viewport-flooding reveals:
1. Coral Punch: `#ff6b6b`
2. Bright Teal: `#4ecdc4`
3. Lemon Pop: `#ffe66d`
4. Mint Leaf: `#a8e6cf`
5. Rose Dust: `#ff8b94`
6. Soft Sky: `#c7ecee`

---

## 3. Typography Hierarchy

* Display Headlines: `Slackey` (Google Font)
  * Hero Title: `text-4xl sm:text-5xl tracking-normal leading-[1.1]`
  * Winner Card: `text-3xl sm:text-4xl font-bold break-words`
* User Interface & Body: `Plus Jakarta Sans` (Google Font)
  * Subtext: `text-sm font-medium text-zinc-400 max-w-[280px] leading-relaxed`
  * Action Buttons: `text-base sm:text-lg font-bold tracking-wide`
  * Option Tags: `text-sm font-semibold`

---

## 4. Surfaces, Radii & Component Shapes

* Corner Radii: strictly pill-shaped (`rounded-full`) for all interactive surfaces[cite: 5].
  * Primary Action Button: `h-14 w-full rounded-full bg-[#ffd02f] text-black font-extrabold shadow-lg active:scale-[0.98]`[cite: 5].
  * Input Wrapper: `h-14 w-full rounded-full bg-[#1b1b1f] border border-zinc-800 px-5`[cite: 5].
  * Add Action Button: `h-10 px-5 rounded-full bg-zinc-800 text-white font-bold hover:bg-zinc-700 active:scale-95`[cite: 5].
  * Option Badges: `rounded-full px-4 py-2.5 flex items-center justify-between text-black font-bold`[cite: 5].
* Elevation & Shadows:
  * Soft drop shadows tinted to base tone.
  * No arbitrary multi-color borders.

---

## 5. Architectural & Aesthetic Refusals

* Strict zero em-dash policy: the `—` character is banned across headlines, subtext, badges, and button labels[cite: 5].
* No multi-column desktop grids (single-column mobile stack only)[cite: 5].
* No AI-purple glows, saturated magenta accents, or default blue button highlights[cite: 5].
* No unvetted generic serif typefaces[cite: 5].
* No plain card containers with hairline box borders where white space or background tinting communicates separation[cite: 5].
* No mid-word typographic hyphenation on multi-word restaurant titles.

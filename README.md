# Tolong Aku Decide

A kinetic, zero-dependency mobile web application designed to eliminate group indecision through an animated roulette wheel and negotiation flow.

Built as a single-file prototype (`index.html`) using Tailwind CSS and the Web Audio API.

---

## Live Demo

Run the application directly in any modern mobile or desktop browser:
`https://wanamir-vibecode.github.io/tolong-aku-decide/`

---

## Features

* **Kinetic Decision Engine**: High-velocity ticker with variable-friction deceleration physics.
* **Screen-Flooding Reveals**: Transitions dynamically into the winning option's assigned theme colour upon selection.
* **Smart Word-Wrapping**: Prevents awkward typography breaks across titles and restaurant names.
* **Negotiation Cycle**: Built-in resolution logic ("Happy with this choice?" leading to confirmation, re-roll, or "Do Anyways").
* **Synthesised Audio**: Mechanical tick clicks and celebration chimes generated via the native Web Audio API (zero external audio assets)[cite: 4].
* **Session Persistence**: Saves prior decisions locally with timestamps[cite: 4].

---

## Design System & Calibration

The interface adheres to strict frontend anti-slop guidelines[cite: 4]:

| Dial | Value | Specification |
|---|---|---|
| `DESIGN_VARIANCE` | 7 | High-contrast kinetic layout constrained to mobile viewports (`max-w-md`)[cite: 4]. |
| `MOTION_INTENSITY` | 8 | Physics-driven deceleration ticker with spring feedback[cite: 4]. |
| `VISUAL_DENSITY` | 4 | Generous tap targets with clean separation of active cards[cite: 4]. |

* **Typography**: Slackey (Display headline) paired with Plus Jakarta Sans (Body and UI)[cite: 4].
* **Base Palette**: Off-black foundation (`#0f0f11`) with canary yellow (`#ffd02f`) interactive anchors[cite: 4].
* **Dynamic Palette**: Sequential vibrant accents (`#ff6b6b`, `#4ecdc4`, `#ffe66d`, `#a8e6cf`, `#ff8b94`, `#c7ecee`) assigned per option[cite: 4].
* **Refusals**: Zero em-dashes, no unvetted display fonts, no generic multi-column cards, no AI-purple button glows[cite: 4].

---

## Architecture

The entire client is contained within a single distribution file[cite: 4]:

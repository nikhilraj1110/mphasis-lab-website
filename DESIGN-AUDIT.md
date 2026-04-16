# Design Audit — Phase 1 Review
**Date:** Feb 27, 2026
**Status:** Noted — to be implemented in Phase 1 revision

---

## P0 — Critical (Contradicts user requirements)

### 1. Color Too Timid, No Warmth
- Page is 95% white/gray. Brand colors (Ashoka red, Mphasis blue) barely appear.
- Pillar colors only on tiny 4px bars and pill-sized tags.
- `section--alt` background (`gray-50`) is barely distinguishable from white.
- **Fix:** Bolder pillar color usage (tinted backgrounds, gradient touches). Warm-white base (`#FAFAF8`). Richer `section--alt` treatment.

### 2. No Visual Identity / Motif
- Site looks like a generic CSS framework template. Zero personality.
- Nothing says "research lab" or "Ashoka University."
- **Fix:** Extract geometric pattern from Ashoka logo as recurring motif — hero background, section dividers, footer decoration. Secondary motif: grid/node pattern (research connections).

---

## P1 — High Impact

### 3. Hero Lacks Visual Drama
- Just left-aligned text on blank white. No visual weight on right side. No energy.
- Badge is generic. No connection to brand identity.
- **Fix:** Background gradient/pattern. Visual element on right (geometric composition, research imagery). Make it feel alive.

### 4. No Entrance Animations
- Everything renders instantly. Page feels static and lifeless.
- **Fix:** Scroll-triggered fade-in-up animations with `IntersectionObserver`. Stagger grid items. 20-30px translateY, 400ms, ease-out. Subtle, not flashy.

### 5. Pillar Cards Too Uniform
- 4px color indicator barely registers. All 5 cards look identical.
- 5 cards in 3-column grid = awkward layout (3 + 2 with empty space).
- No icons per pillar — color alone fails for colorblind users.
- **Fix:** Tinted card backgrounds using pillar-bg colors. Add icon/symbol per pillar. Rethink layout for 5 items (3+2 centered, or featured card layout).

---

## P2 — Medium Impact

### 6. Stat Numbers — Static and Flat
- No visual emphasis beyond font size. No dividers, icons, or motion.
- **Fix:** Vertical dividers on desktop. Scroll-triggered count-up animation. Colored accent on numbers.

### 7. Inline Styles in HTML
- Multiple `style="..."` attributes, especially in dark section color overrides.
- **Fix:** Move to proper CSS rules (`.section--dark .stat-card__number`, etc.). Keep CSS custom property vars on components as acceptable API.

### 8. Header Nav Crowding
- 9 nav links in one row. Cramped at 1024-1200px. Active state (just bold) too subtle.
- Logo at 40px too small for detailed image.
- **Fix:** Consider grouping to 5-6 items, or two-line header. Add underline/dot for active state. Increase logo to 44-48px.

### 9. Section Rhythm Monotonous
- Every section uses identical padding. Same cadence throughout.
- Transitions between sections are just background color changes.
- **Fix:** Vary section padding. Consider subtle dividers (angled/curved SVG). Let elements break section boundaries for depth.

### 10. Card Accent-Top Border Clumsy
- 3px colored top border + 1px card border = looks like a rendering glitch.
- **Fix:** Remove card border and use bolder accent top (4-5px), or use left-side accent, or color-tint card background.

### 11. Card Placeholders Ugly
- Flat gray rectangles kill visual appeal. May be permanent for projects without photos.
- **Fix:** Gradient placeholders with pillar colors. Pattern/icon overlay. Faint watermark treatment.

---

## P3 — Polish

### 12. Footer Logo Treatment
- `filter: brightness(0) invert(1)` makes Mphasis logo lose its brand colors (blue/purple swoosh becomes white blob).
- **Fix:** Request white logo versions as separate assets, or use lighter strip within dark footer.

### 13. Mobile Refinements
- Stat grid jumps 4→1 columns (needs 2-column intermediate).
- Filter bar scrollability not visually indicated.
- Hero CTAs should stack on small screens.
- **Fix:** Add 2-column breakpoint. Fade edges on filter bar. Stack buttons vertically on mobile.

### 14. Accessibility Gaps
- Filter bar buttons need `aria-pressed` states.
- Pillar cards as `<a>` wrapping block content — semantically questionable.
- Color-only pillar identification needs secondary identifiers for colorblind users.
- Placeholder images need better aria treatment.
- **Fix:** Add ARIA states. Refactor pillar card markup. Add icons alongside colors. Fix alt text.

### 15. Missing Components
- No favicon
- No scroll-to-top button
- No announcement bar component
- No loading/skeleton treatment

---

## Interactivity & Immersion Plan

(See separate section below — full interactive experience audit)

---

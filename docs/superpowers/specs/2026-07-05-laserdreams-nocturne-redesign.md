# LASERDREAMS Cologne — "Nocturne" Redesign

Date: 2026-07-05 · Status: user delegated direction ("choose yourself"), v1
(porcelain/beige editorial) rejected as cheap/boring/basic.

## Why v1 failed
- Light greige palette read washed-out and template-like, not luxurious.
- Bodoni Moda + Jost read as default "elegant spa" typography.
- Video was framed in an arch panel — user wanted it as a true background.

## Direction: cinematic editorial noir ("Nocturne Cologne")
- **Theme:** dark. Clientele browses Instagram at night; luxury positioning.
- **Palette (OKLCH):** warm near-black canvas ~oklch(16% .012 60), elevated
  ~oklch(20% .015 60); warm ivory text; champagne accent ~oklch(78% .06 75)
  and deep gold ~oklch(65% .08 65); one fir-green panel (studio door).
  Neutrals tinted toward the warm brand hue. 60-30-10 weight.
- **Type:** Italiana display (huge, fashion-cover scale, single weight) +
  Hanken Grotesk 300/400/500 body. Reflex fonts (Playfair/Cormorant/Bodoni/
  Fraunces…) explicitly rejected per impeccable procedure.
- **Video usage (user requirement):** full-bleed background.
  - Mobile: the entire hero (100svh) is the walkthrough video under a noir
    gradient veil; content bottom-anchored.
  - Desktop: same video bleeds off the top/right/bottom edges of the hero
    (right ~46%), melted into the canvas with a long horizontal gradient.
  - One shared `<video>` element, repositioned by CSS. Audio track stripped
    at encode time (`-an`); `muted playsinline autoplay loop`.
- **Signature:** stacked giant "LASER / DREAMS" Italiana hero over the video,
  plus a champagne "laser line" that draws across the statement section.

## Page structure (single index.html, inline CSS/JS, German)
1. Header — transparent over hero → noir on scroll; logo_transparent.png
   recolored to warm ivory via CSS filter (dark logo invisible on noir).
2. Hero — as above; meta rule at bottom (ICE-Diodenlaser · 4 Wellenlängen ·
   Frauen & Männer).
3. Statement — "Natürlich schön. Dauerhaft glatt." huge, laser-line draw.
4. Vorteile — three asymmetric editorial rows (oversized Italiana keyword +
   copy), hairline separators; no equal card grid.
5. Technologie — treated Behandlungsraum photo, copy, wavelengths as large
   Italiana numerals 755 / 808 / 940 / 1064.
6. Preise — giant text toggle (Damen / Herren), hairline-leader rows, real
   flyer prices; Pakete as champagne-ruled feature rows.
7. Stimmen — three real quotes, alternating asymmetric blocks, not cards.
8. Kontakt — deep fir-green panel ("die grüne Tür"), Instagram CTA.
9. Footer — noir, ivory logo, Impressum/Datenschutz placeholders.

## Quality gates
- Screenshot iteration desktop + mobile until it passes the AI-slop test.
- No border-left stripes, no gradient text, no glassmorphism, no
  transition-all; focus-visible everywhere; reduced-motion honored.

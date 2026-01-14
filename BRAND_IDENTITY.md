# word and mouth* Brand Identity

> *Established: 2026-01-14*
> *Inspired by: Carl Sagan's Cosmos*

---

## The Logo

**word and mouth***

- Three words stacked vertically
- Lowercase throughout
- Clean, rounded sans-serif font (Space Grotesk)
- White text on dark backgrounds, or dark text on light backgrounds
- The asterisk is always in accent orange (#ff6b35)

### The Asterisk

The asterisk is not decoration. It is a **visual verb**.

**Meaning:** "There's more here"

The asterisk literally means "little star" in Latin. It signals:
- Deeper explanation available
- This point is essential — don't skip it
- A footnote to the surface story
- The hidden insight beneath the obvious

### Usage Guidelines

**Use the asterisk when:**
- Making a super important point that must sink in for skimmers
- Linking to additional information or resources
- Highlighting a moment of insight or revelation
- Marking CTAs that lead somewhere meaningful

**Don't use the asterisk:**
- For decoration or animation
- On every heading (it loses potency)
- Without purpose

---

## Colour Palette

| Colour | Hex | Usage |
|--------|-----|-------|
| **Accent Orange** | #ff6b35 | Asterisks, highlights, CTAs |
| **Background Dark** | #0a0a0a | Primary background |
| **Text White** | #fafafa | Primary text |
| **Muted Grey** | #888888 | Secondary text, notes |
| **Border** | #222222 | Dividers, subtle structure |

---

## Typography

- **Headlines:** Space Grotesk, 700 weight
- **Body:** Inter, 400/500 weight
- **Logo:** Space Grotesk, 700 weight, lowercase

---

## The Origin Story

The STAR Framework — Shift, Tension, Awe, Resolution — was synthesized from Carl Sagan's Cosmos. The asterisk connects directly to this origin:

> "We are made of star-stuff."

The asterisk is a star. word and mouth* helps organisations find their cosmic perspective — the deeper story beneath the surface that changes how everyone shows up.

---

## CSS Implementation

The website includes these utility classes for the visual verb:

```css
/* In Base.astro global styles */

.logo-star {
  color: var(--accent);
  font-weight: 700;
}

/* Visual verb asterisk — use when making important points or linking to more */
.vv {
  color: var(--accent);
  font-weight: 700;
  cursor: help;
}

.vv-link {
  color: var(--accent);
  font-weight: 700;
}

.vv-link:hover {
  text-decoration: underline;
}
```

### Usage in HTML

```html
<!-- Important point with asterisk -->
<p>Solutions grow your market<span class="vv">*</span></p>
<p class="asterisk-note"><span class="vv">*</span> This is the deeper explanation.</p>

<!-- Logo -->
<a href="/" class="logo">word and mouth<span class="logo-star">*</span></a>
```

---

## Assets

- **Logo (dark bg):** `/public/logo.png`
- **Favicon:** `/public/favicon.svg` (to be updated)

---

## The Philosophy

**Purposeful playfulness.** 

word and mouth* believes that serious results don't require a sombre attitude. The asterisk embodies this: it's playful (a tiny star!) but purposeful (there's more here). 

Joy is a multiplier. Curiosity is a strategy. If it's not fun, we're doing it wrong.

---

## Footer Tagline

> © 2026 word and mouth* — there's more here.

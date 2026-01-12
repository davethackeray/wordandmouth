# WordAndMouth.com Design System

## Principles

1. **Radical Simplicity** — Max 3 nav items. Whitespace as confidence.
2. **Depth on Demand** — Surface is simple, details expand in-place.
3. **Native Demos** — Projects keep their own visual identity. We don't force them into our design.

---

## Colour Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#0a0a0a` | Page background |
| `--text` | `#fafafa` | Primary text |
| `--accent` | `#ff6b35` | CTAs, highlights, tenets |
| `--muted` | `#888` | Secondary text |
| `--border` | `#222` | Dividers, cards |

---

## Typography

| Element | Font | Size | Weight |
|---------|------|------|--------|
| Headlines | Space Grotesk | clamp(2rem, 5vw, 3.5rem) | 700 |
| Body | Inter | 1rem-1.3rem | 400 |
| Labels | Space Grotesk | 0.85rem | 500 |
| Code/technical | System mono | 0.9rem | 400 |

---

## Component Patterns

### Tenet Tags
```css
.tenet {
  background: rgba(255, 107, 53, 0.15);
  color: var(--accent);
  padding: 0.25rem 0.6rem;
  font-size: 0.7rem;
  font-weight: 600;
  text-transform: uppercase;
}
```

### Section Structure
```astro
<section class="section">
  <h2 class="section-label">Label</h2>
  <!-- content -->
</section>
```

### CTAs
- **Primary**: `background: var(--accent)`, black text
- **Secondary**: Ghost button with border

---

## Demo Handling

Projects with distinct visual identity (The Stack, Zeitgeist, etc.) are handled as:

### Option A: External Link
```astro
<a href="/demos/the-stack/" target="_blank" class="demo-link">
  View Demo ↗
</a>
```

### Option B: Iframe Modal
```astro
<button onclick="openDemo('/demos/the-stack/')">View Demo</button>

<dialog id="demo-modal">
  <iframe src="" frameborder="0"></iframe>
  <button onclick="closeDemo()">Close</button>
</dialog>
```

### File Structure
```
wam-site/
├── public/
│   └── demos/
│       ├── the-stack/       ← Full project with own CSS
│       ├── zeitgeist/
│       └── freed-reads/
```

---

## Page Templates

| Page | Purpose |
|------|---------|
| `/` | Homepage — 5 tenets as scenarios |
| `/work` | Case studies grid (tagged by tenet) |
| `/about` | Superpowers + bio |
| `/testimonials` | Proof page |
| `/[tenet]` | Tenet hub (e.g., `/clarity`) with related content |

---

## User Flows

### New Visitor → Client
1. Land on homepage → Feel the problem
2. Click scenario that resonates
3. Read case study → See proof
4. View demo → Experience the work
5. CTA → Book a call

### Returning Visitor → Deep Content
1. Land on tenet page (e.g., `/ai`)
2. See related podcasts, research, case studies
3. Explore → Build trust
4. CTA → Engage

---

*Last updated: 2026-01-12*

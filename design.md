# Design System Inspired by www.thefa.com

> Auto-extracted from `https://www.thefa.com/` on 2026-06-04

## 1. Visual Theme & Atmosphere

Friendly, approachable design with rounded shapes and generous whitespace.

The hero section leads with "The FA" followed by "Close Modal".

**Key Characteristics:**
- Arial as the heading font
- Arial as the body font for all running text
- Heading weight 400
- Light/white background (#f0eced) as the primary canvas
- Primary accent `#0068b2` used for CTAs and brand highlights
- 7 shadow level(s) detected — tinted shadows
- Rounded corners (2px+) creating a friendly, approachable feel
- Tags: light, rounded, accented, sans-serif

## 2. Color Palette & Roles

### Primary
- **Primary Accent** (`#0068b2`) · `--color-primary`: Brand color, CTA backgrounds, link text, interactive highlights.
- **Secondary Accent** (`#3860be`) · `--color-secondary`: Secondary brand, hover states, complementary highlights.
- **Background** (`#f0eced`) · `--color-bg`: Page background, primary canvas.
- **Background Secondary** (`#011e41`) · `--color-bg-secondary`: Cards, surfaces, alternating sections.

### Text
- **Text Primary** (`#333333`) · `--color-text`: Headings and body text.
- **Text Secondary** (`#666666`) · `--color-text-secondary`: Muted text, captions, placeholders.

### Borders & Surfaces
- **Border** (`#f7f7f7`) · `--color-border`: Dividers, outlines, input borders.

### Full Extracted Palette

| # | Hex | CSS Variable | Role | Area | Contrast |
|---|---|---|---|---|---|
| 1 | `#ffffff` | `--palette-1` | block | large | text-dark |
| 2 | `#011e41` | `--palette-2` | text-accent | large | text-light |
| 3 | `#f7f7f7` | `--palette-3` | block | large | text-dark |
| 4 | `#f0eced` | `--palette-4` | section | large | text-dark |
| 5 | `#222222` | `--palette-5` | block | medium | text-light |
| 6 | `#0068b2` | `--palette-6` | text-accent | small | text-light |
| 7 | `#02264c` | `--palette-7` | text-accent | small | text-light |
| 8 | `#3860be` | `--palette-8` | text-accent | small | text-light |
| 9 | `#5d6f86` | `--palette-9` | text-accent | small | text-light |

## 3. Typography Rules

- **Heading Font:** `Arial`, sans-serif
- **Body Font:** `Arial`, sans-serif

### Type Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|---|---|---|---|---|---|
| H1 | Arial | 32px | 400 | 45.7142px | normal |
| H2 | FSJackPoster | 30px | 400 | 42.8571px | normal |
| H3 | Arial | 18px | 700 | 21.6px | normal |
| H4 | Arial | 14.08px | 600 | 21.12px | normal |
| Body | Arial | 12px | 400 | 17.1428px | normal |
| Small | Arial | 11px | 400 | 12px | normal |

### Type Scale

| Token | Size | Suggested Usage |
|---|---|---|
| Display | `32px` | headings |
| H1 | `30px` | headings |
| H2 | `29px` | headings |
| H3 | `24px` | headings |
| H4 | `18px` | headings |
| Body L | `16px` | body / supporting text |
| Body | `14.4px` | body / supporting text |
| Small | `14.08px` | body / supporting text |
| XS | `14px` | body / supporting text |
| Caption | `13.6px` | body / supporting text |

## 4. Component Stylings

### Primary Button

```css
.btn-primary {
  background: transparent;
  color: #333333;
  border-radius: 0px;
  padding: 0px 128px;
  font-size: 0px;
  font-weight: 400;
  border: none;
  cursor: pointer;
}
```

### Filled Button

```css
.btn-filled {
  background: #ffffff;
  color: #02264c;
  border-radius: 0px;
  padding: 12px 0px;
  font-size: 14px;
  font-weight: 400;
  border: none;
  cursor: pointer;
}
```

## 5. Layout Principles

- **Base spacing unit:** `8px` — use multiples (16px, 24px, 32px, etc.)

### Spacing Scale (extracted from real elements)

| Token | Value | Role |
|---|---|---|
| spacing-1 | `8px` | element |
| spacing-2 | `12px` | element |
| spacing-3 | `5px` | element |
| spacing-4 | `15px` | element |
| spacing-5 | `30px` | card |
| spacing-6 | `25px` | card |
| spacing-7 | `11px` | element |
| spacing-8 | `20px` | element |

### Border Radius Scale

| Token | Value | Element |
|---|---|---|
| radius-subtle | `2px` | subtle |
| radius-subtle | `1px` | subtle |
| radius-card | `20px` | card |
| radius-subtle | `3px` | subtle |
| radius-card | `17px` | card |
| radius-card | `50px` | card |

## 6. Depth & Elevation

| Level | Shadow | Usage |
|---|---|---|
| Low | `rgba(0, 0, 0, 0.6) 0px 2px 4px 0px` | Cards, subtle elevation |
| Low | `rgb(204, 210, 217) 0px 0px 0px 1px inset` | Cards, subtle elevation |
| Mid | `rgba(0, 0, 0, 0.6) 0px 4px 5px 0px` | Dropdowns, popovers |
| Mid | `rgba(0, 0, 0, 0.6) 0px 0px 5px 0px` | Dropdowns, popovers |
| Mid | `rgb(153, 153, 153) 0px 2px 10px -3px` | Dropdowns, popovers |


## 7. Do's and Don'ts

### Do
- Use `#f0eced` as the primary background color
- Use `Arial` for all headings and `Arial` for body text
- Use `#0068b2` as the single dominant accent/CTA color
- Maintain `8px` as the base spacing unit — all gaps should be multiples
- Use rounded corners (`2px`+) consistently for all interactive elements
- Apply the shadow system for elevation — use the extracted shadow values
- Use weight 400 for headings to match the brand's typographic voice

### Don't
- Don't use colors outside the extracted palette without justification
- Don't substitute Arial/Arial with generic alternatives
- Don't use irregular spacing — stick to 8px grid
- Don't use dark/black backgrounds — this is a light-themed design
- Don't use sharp corners — they feel hostile in this rounded design language
- Don't use pure black (#000000) for text — use `#333333` instead
- Don't add decorative elements not present in the original design — no badges, ribbons, banners, or ornaments unless the source site uses them
- Don't invent UI patterns the source site doesn't have — if the original has no NEW badge, don't add one just because a red is in the palette

## 8. Responsive Behavior

| Breakpoint | Width | Notes |
|---|---|---|
| Mobile | < 640px | Single column, stack sections, reduce font sizes ~80% |
| Tablet | 640–1024px | 2-column where appropriate, maintain spacing ratios |
| Desktop | 1024–1440px | Full layout as designed |
| Wide | > 1440px | Max-width container, center content |

- Touch targets: minimum 44×44px on mobile
- Maintain 8px base unit across breakpoints — only scale multipliers

## 9. Agent Prompt Guide

### Quick Color Reference

```
Background:  #f0eced
Text:        #333333
Accent:      #0068b2
Secondary:   #3860be
Border:      #f7f7f7
```

### Example Prompts

1. "Build a hero section with a `#f0eced` background, `Arial` heading in `#333333`, and a `#0068b2` CTA button with 0px radius."
2. "Create a pricing card using background `#011e41`, border `#f7f7f7`, `Arial` for text, and 24px padding."
3. "Design a navigation bar — `#f0eced` background, `#333333` links, `#0068b2` for active state."
4. "Build a feature grid with 3 columns, 24px gap, each card using the card component style."
5. "Create a footer with `#333333` background, `#f0eced` text, and 16px padding."

### Iteration Guide

1. Start with layout structure (sections, grid, spacing)
2. Apply colors from the palette — background first, then text, then accents
3. Set typography — font families, sizes from the type scale, weights
4. Add components — buttons, cards, inputs using the specs above
5. Apply border-radius consistently across all elements
6. Add shadows for depth — use the extracted shadow values, not defaults
7. Check responsive behavior — test mobile and tablet layouts
8. Final pass — verify all colors match, spacing is consistent, fonts are correct

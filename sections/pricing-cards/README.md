# Pricing Cards

A 4-card pricing/service grid with background images, color overlays, and per-card CTAs — built for showcasing packages, rituals, or service tiers. On mobile, switches to a swipeable snap-scroll slider with nav buttons.

## Features

- Section header (subtitle + title + rich-text description), fully optional
- 4 independent cards, each with its own:
  - Background image + overlay color/opacity
  - Title, description, price, button text/link
  - Content alignment (left / center / right)
  - Text color
  - Optional full-card click link
- Configurable `cards_per_row` (1–4) for desktop grid
- Hover effect: card lifts with a shadow
- Mobile: optional swipeable slider (CSS scroll-snap) with prev/next nav buttons, or falls back to a simple 1-column stack
- Extensive style controls — spacing, sizes, colors, border radius — all through the theme customizer

## How to Use

Standalone **section**. Drop `pricing-cards.liquid` into your theme's `sections/` folder, then add it via the theme customizer ("Add section" → "Pricing cards").

## Schema Settings (key ones)

| Setting | Type | Description |
|---|---|---|
| `section_title` / `section_subtitle` / `section_description` | richtext | Header content above the grid |
| `cards_per_row` | range | Desktop grid columns (1–4) |
| `card_spacing`, `card_min_height`, `card_padding`, `card_border_radius` | range | Card layout |
| `enable_mobile_slider` | checkbox | Toggle mobile slider vs. stacked layout |
| `show_nav_buttons` | checkbox | Show/hide slider prev/next arrows |
| `card_1_image` … `card_4_image` | image_picker | Background image per card |
| `card_1_overlay_color` / `_overlay_opacity` | color / range | Overlay per card |
| `card_1_title` / `_description` / `_price` / `_button_text` / `_button_link` | text/richtext/url | Card content (repeated for cards 1–4) |
| `card_1_alignment` | select | Content alignment per card |
| `card_1_text_color` | color | Text color per card |

Full settings list is in the `{% schema %}` block of the liquid file.

## Dependencies

- None (vanilla JS, no external libraries). Uses native CSS scroll-snap for the mobile slider — no swipe library needed.
- Uses `var(--font-heading-family)` for headings — assumes your theme defines this CSS variable (most Shopify Online Store 2.0 themes do). If yours doesn't, replace it with a fallback font-family or remove the line.

## Notes

- Card content loops over `card_1` … `card_4` via dynamically built setting keys (`'card_' | append: i | append: '_title'`), so adding a 5th card means extending the `{% for i in (1..4) %}` loop range **and** adding matching `card_5_*` settings in the schema (in two places — desktop grid and mobile slider both render the same loop).
- Card content sits above a colored overlay above a background image (3 stacked layers using `position: absolute`) — this is what makes the overlay + image + text combination work without extra image editing.
- French default copy in the schema ("RITUELS SIGNATURE", "Réserver", etc.) — this came from the original store context; replace with your own defaults if reusing on an English store.

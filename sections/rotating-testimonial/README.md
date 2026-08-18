# Rotating Testimonial Slider

A 3D coverflow-style testimonial carousel — center card full size and forward, side cards scaled down and rotated in 3D for a stacked-deck effect. Shows customer image, star rating, review text, and a verified-purchase badge. Falls back to a simple center-only view on smaller screens.

![preview](Rotating%20Testimonial.png)

## Features

- Up to 5 testimonials, each with:
  - Image (with placeholder fallback if none set)
  - Star rating (1–5, visually filled based on setting)
  - Review text (defaults provided, editable via textarea)
  - Optional "Verified Purchase" badge with custom label
- 3D coverflow effect on desktop — center card scaled up, left/right cards rotated and scaled down with `rotateY` + `scale`, active card cross-fades in with opacity + translateX
- Prev/next navigation buttons that cycle through testimonials (wraps around, no dead ends)
- Responsive breakpoints:
  - `≤1024px` — side cards hide, only center card shows (simplified, no rotation)
  - `≤768px` — smaller card size, smaller nav buttons, scaled-down heading sizes
- Optional heading + subheading above the slider

## How to Use

Standalone **section**. Drop `testimonial-slider.liquid` into your theme's `sections/` folder, then add it via the theme customizer ("Add section" → "Modern testimonial slider").

## Schema Settings (key ones)

| Setting | Type | Description |
|---|---|---|
| `heading` / `subheading` | inline_richtext | Optional header above the slider |
| `heading_size` / `subheading_size` | range | Header text sizes |
| `card_background`, `card_border_radius` | color / range | Card styling |
| `star_color` | color | Star rating icon color |
| `review_text_color` | color | Review body text color |
| `verified_color`, `verified_text` | color / inline_richtext | Verified badge styling and label |
| `nav_button_bg` / `nav_button_color` / `nav_button_hover_bg` | color | Prev/next button styling |
| `testimonial_1_image` … `testimonial_5_image` | image_picker | Customer photo per testimonial |
| `testimonial_1_review` … `testimonial_5_review` | textarea | Review text per testimonial |
| `testimonial_1_rating` … `testimonial_5_rating` | range (1–5) | Star rating per testimonial |
| `testimonial_1_verified` … `testimonial_5_verified` | checkbox | Show/hide verified badge per testimonial |

Full settings list is in the `{% schema %}` block of the liquid file.

## Dependencies

- None (vanilla JS, no external libraries). Uses a native Web Component (`customElements.define`) for slider navigation.

## Notes

- Testimonial content loops over `testimonial_1` … `testimonial_5` via dynamically built setting keys (`'testimonial_' | append: i | append: '_review'`, etc.). Adding a 6th testimonial means extending the `{% for i in (1..5) %}` loop range **and** adding matching `testimonial_6_*` settings in the schema.
- The 3D coverflow effect (`rotateY`, layered `z-index`, `translateX` offsets) only applies above 1024px — below that it degrades gracefully to a plain single-card view, so there's no broken/clipped 3D rendering on mobile.
- Card height is `auto` (not fixed), so review text length will affect card height — very long reviews will make the center card taller than the side cards, which is expected with this layout.
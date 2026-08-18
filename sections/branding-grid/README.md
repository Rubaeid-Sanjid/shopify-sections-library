# Branding Grid

An asymmetrical 5-image brand/lifestyle grid — four corner images (offset up/down in two columns) with a floating arched portrait image centered on top. On mobile, switches to either a vertical stack or a swipeable touch slider with nav arrows and pagination dots.

![preview](preview.png)

## Features

- 4-image grid (top-left, bottom-left, top-right, bottom-right) with independent image + link per slot
- Floating center "portrait" image with an arched top (rounded corners on top only) and drop shadow, layered above the grid
- Asymmetrical layout — left column shifts up, right column shifts down, controlled independently via sliders
- Fully responsive with two selectable mobile modes:
  - **Stack** — all 5 images stacked vertically, center image first
  - **Slider** — swipeable horizontal slider (touch + mouse drag) with prev/next buttons and pagination dots
- Every image is optional — falls back to a placeholder SVG if not set
- Every image slot supports an optional link
- Extensive style controls: colors, padding, gaps, corner radius, arch radius, nav button styling, pagination styling — all through the theme customizer, no code editing needed

## How to Use

This is a standalone **section**. Drop `branding-grid.liquid` into your theme's `sections/` folder, then add it to any template/JSON template via the theme customizer ("Add section" → "Branding grid").

## Schema Settings (key ones)

| Setting | Type | Description |
|---|---|---|
| `background_color` | color | Section background |
| `max_width`, `section_padding`, `grid_gap` | range | Layout sizing |
| `left_column_offset` / `right_column_offset` | range | Vertical shift for the asymmetrical look |
| `image_top_left` / `image_bottom_left` / `image_top_right` / `image_bottom_right` | image_picker | The 4 grid images |
| `top_left_link` / `bottom_left_link` / `top_right_link` / `bottom_right_link` | url | Optional link per image |
| `center_image` | image_picker | The floating arched portrait image |
| `center_image_width`, `center_border_radius` | range | Size and arch shape of the center image |
| `mobile_layout` | select | `stack` or `slider` |
| `show_nav_buttons`, `show_pagination` | checkbox | Slider mode controls (mobile only) |

Full settings list (colors, sizes, spacing for nav buttons and pagination dots) is in the `{% schema %}` block of the liquid file.

## Dependencies

- None (vanilla JS, no external libraries)
- Uses a native Web Component (`customElements.define`) for the mobile slider — no jQuery or frameworks needed

## Notes

- The mobile slider has exactly 5 slides hardcoded (`this.totalSlides = 5`) matching the 5 image slots. If you fork this to add/remove image slots, update `totalSlides` in the script accordingly.
- Supports both touch swipe and mouse-drag swipe on the slider (useful for testing in a desktop browser via device toolbar).
- `section_id` is derived from `section.id`, so multiple instances of this section on the same page won't have CSS class collisions.

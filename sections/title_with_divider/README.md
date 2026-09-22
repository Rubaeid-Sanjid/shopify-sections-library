# Ornamental Divider Title (Title with Divider)

An elegant, customizable **Title with Divider Lines & Ornamental Icons** section for Shopify Online Store 2.0 themes. Perfect for boutique brands, beauty, luxury apparel, lifestyle, and editorial stores to separate page content with sophisticated heading dividers.

Features a central title flanked by decorative divider lines in multiple styles (solid, dashed, dotted, or gradient fade) and optional left/right ornamental icons or custom brand marks.

![Title with Divider Preview](title_with_divider.png)

---

## ✨ Features

- **Multi-Style Divider Lines**: Choose between 4 distinct divider line appearances:
  - `solid`: Classic clean hairline.
  - `dashed`: Subtle repeating dashed stroke.
  - `dotted`: Elegant repeating dotted line.
  - `gradient`: Soft gradient fading out smoothly towards outer container edges.
- **Flanking Ornamental Icons**: Display left and right decorative icons (default SVG heart icon or upload custom brand logos, crests, or icons via Theme Customizer).
- **Comprehensive Typography Controls**:
  - Font families: `Sans-serif`, `Serif`, or `Custom` (input any Google Font or theme custom font name like *Playfair Display*, *Cinzel*, *Cormorant*).
  - Configurable font weight (`300`, `400`, `500`, `600`, `700`).
  - Independent desktop and mobile font sizes.
  - Tracking / letter-spacing slider.
- **Granular Layout & Color Settings**:
  - Adjustable line thickness, gap between icons and text, and section background color.
  - Customizable container maximum width and desktop/mobile vertical padding.
- **Encapsulated Custom Element**: Scoped via `<ornamental-divider-{{ section_id }}>` to prevent style leaks across themes.
- **Zero Heavy Dependencies**: Pure semantic Liquid, HTML5, and scoped CSS with no external libraries.

---

## 🚀 How to Use

1. Copy [`title_with_divider.liquid`](title_with_divider.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template.
3. Click **Add section** and select **Ornamental divider title**.
4. Set your heading text, choose your divider line style, pick your icon styling, and position it between sections.

---

## ⚙️ Schema Settings

### Title & Typography

| Setting | Type | Default | Description |
|---|---|---|---|
| `title_text` | `text` | `FEATURED COLLECTION` | Heading text |
| `title_color` | `color` | `#222222` | Heading text color |
| `font_family` | `select` | `sans-serif` | `Sans-serif`, `Serif`, or `Custom` |
| `custom_font_family` | `text` | *empty* | Custom font family name (e.g. `Playfair Display`) |
| `font_weight` | `select` | `500` | Light (`300`), Regular (`400`), Medium (`500`), Semi-bold (`600`), Bold (`700`) |
| `font_size_desktop` / `_mobile` | `range` | `28px` / `20px` | Responsive font sizes |
| `letter_spacing` | `range` | `1px` | Letter spacing tracking (0px to 5px) |

### Ornamental Icons

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_left_icon` / `show_right_icon` | `checkbox` | `true` | Toggle left and right icons |
| `left_icon` / `right_icon` | `image_picker` | — | Upload custom icon image (leaves default SVG if empty) |
| `icon_size_desktop` / `_mobile` | `range` | `24px` / `18px` | Responsive icon dimensions |
| `icon_color` | `color` | `#E0006C` | Fill color for default SVG icons |
| `icon_text_gap` | `range` | `15px` | Spacing gap between icon and title text |

### Divider Lines

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_lines` | `checkbox` | `true` | Show or hide divider lines |
| `line_color` | `color` | `#E0006C` | Line stroke / gradient color |
| `line_thickness` | `range` | `2px` | Line height/thickness (1px to 10px) |
| `line_style` | `select` | `solid` | `Solid`, `Dashed`, `Dotted`, or `Gradient fade` |

### Layout & Spacing

| Setting | Type | Default | Description |
|---|---|---|---|
| `max_width` | `range` | `800px` | Maximum content width (400px to 1600px) |
| `section_bg_color` | `color` | `#FFEFF4` | Section background color |
| `padding_top` / `padding_bottom` | `range` | `40px` / `40px` | Vertical padding |
| `desktop_width_percent` | `range` | `100%` | Section width percentage (50% to 100%) |

---

## 💻 Tech & Compatibility

- **Shopify Compatibility**: Online Store 2.0 (OS 2.0)
- **Zero Dependencies**: Pure Liquid, HTML5, and CSS
- **Performance**: Extremely lightweight with instantaneous render time
- **License**: MIT

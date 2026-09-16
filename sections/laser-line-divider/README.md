# Laser Line Divider

A cyberpunk / dark tech styled laser beam divider section for Shopify Online Store 2.0 themes. Designed to demarcate page sections with a futuristic glowing laser beam, tracking-spaced monospace label, and optional breathing pulse animation.

![Laser Line Divider Preview](preview.png)

---

## ✨ Features

- **Futuristic Laser Beam Effect**: Horizontal lines with gradient fade-out towards outer edges and soft neon laser glow (`box-shadow`).
- **Cyber Monospace Typography**: Uppercase tracked label (`01 — THE PROBLEM`, `02 — FEATURES`, etc.) with customizable letter spacing and font family (Monospace, Sans-serif, Heading, or Body).
- **Flexible Alignment**: Align content to `Center`, `Left`, or `Right` (with auto-balanced beam lengths).
- **Optional Laser Pulse**: Toggleable breathing laser animation for an electric cyber vibe.
- **Optional Link / Anchor**: Set an optional URL or in-page anchor ID (e.g. `#problem`) to turn the label into a clickable link.
- **Full Customizer Controls**: Control laser color, glow blur radius, opacity, line thickness, text size (desktop & mobile), gap, and container padding.
- **Zero Dependencies**: 100% pure CSS, no external libraries or heavy scripts.

---

## 🚀 How to Use

1. Copy [`laser-line-divider.liquid`](laser-line-divider.liquid) into your Shopify theme's `sections/` folder.
2. In the Shopify theme customizer, navigate to any page template.
3. Click **Add section** and search for **Laser Line Divider**.
4. Set your section step/title (e.g., `01 — THE PROBLEM`), choose your accent/laser color, and position it between sections.

---

## ⚙️ Schema Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `tag_text` | `text` | `01 — THE PROBLEM` | Divider text / label |
| `tag_link` | `url` | *empty* | Optional link or anchor jump (e.g. `#problem`) |
| `content_alignment` | `select` | `center` | `center`, `left`, or `right` |
| `text_transform` | `select` | `uppercase` | Uppercase, Lowercase, Capitalize, None |
| `tag_color` | `color` | `#ef4444` | Label text color |
| `tag_font_size_desktop` / `_mobile` | `range` | `11px` / `10px` | Responsive font sizes |
| `tag_letter_spacing` | `range` | `3.5px` | Tracking / letter spacing |
| `font_weight` | `select` | `600` | Regular (400), Medium (500), Semi Bold (600), Bold (700) |
| `tag_font_family` | `select` | `monospace` | Monospace, Sans-serif, Heading, Body |
| `gap_size` | `range` | `16px` | Gap between label and laser beams |
| `show_laser_lines` | `checkbox` | `true` | Show/hide laser lines |
| `laser_color` | `color` | `#ef4444` | Laser beam color |
| `laser_glow_color` | `color` | `rgba(239, 68, 68, 0.45)` | Laser neon glow shadow color |
| `laser_thickness` | `range` | `1px` | Line thickness (1px to 5px) |
| `laser_glow_blur` | `range` | `10px` | Neon glow blur radius |
| `laser_opacity` | `range` | `85%` | Overall beam opacity |
| `enable_pulse` | `checkbox` | `false` | Enable breathing laser pulse animation |
| `pulse_speed` | `range` | `3s` | Pulse cycle duration |
| `section_bg` | `color` | `#000000` | Background color |
| `container_max_width` | `range` | `1280px` | Container maximum width |
| `padding_top_desktop` / `padding_bottom_desktop` | `range` | `48px` | Vertical padding on desktop |
| `padding_top_mobile` / `padding_bottom_mobile` | `range` | `32px` | Vertical padding on mobile |

---

## 💻 Tech & Compatibility

- **Shopify Compatibility**: Online Store 2.0 (OS 2.0)
- **Zero Dependencies**: Pure HTML and CSS
- **Performance**: Lightweight, hardware-accelerated CSS animations
- **License**: MIT

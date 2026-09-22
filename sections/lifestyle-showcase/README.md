# Lifestyle Showcase (The Bond)

An atmospheric, editorial **Lifestyle & Storytelling Showcase Grid** section for Shopify Online Store 2.0 themes. Designed for lifestyle, DTC, fashion, pet tech, and premium storytelling brands to showcase rich photography with captions, ambient glows, and interactive card overlays.

Features an editorial header with gradient text highlights, customizable ambient background glow, card rim lighting effects, configurable aspect ratios, and an optional bottom CTA banner with arrow or video play button styles.

![Lifestyle Showcase Preview](lifestyle-showcase-the-bond.png)

---

## ✨ Features

- **Editorial Storytelling Grid**: Flexible multi-column grid layout (2, 3, or 4 columns on desktop, 1 or 2 on mobile) to showcase brand moments and product lifestyles.
- **Atmospheric Ambient Glow**: Radial gradient background light effect with fully customizable coordinates (`X` and `Y` percentages), blur radius, size, and opacity.
- **Gradient Text Highlights**: Automatically highlights words in headlines with a smooth multi-stop gradient (`gradient_start` &rarr; `gradient_end`).
- **Card Rim Glow & Glassmorphism**: Cards feature subtle translucent borders and optional illuminated rim glows (`enable_rim_glow`) for a modern dark-mode aesthetic.
- **Configurable Aspect Ratios**: Choose between `4:5` (Portrait), `9:16` (Tall Portrait), `1:1` (Square), or `3:4` (Standard).
- **Rich Card Overlays**: Cards support uppercase tags, descriptive editorial sentences, and optional click-through URLs.
- **Dual Bottom CTA Banner Styles**:
  - **Pill Button with Arrow**: Classic high-converting pill CTA button.
  - **Circular Play Button**: Icon button ideal for launching brand video modals or stories.
- **Independent Desktop & Mobile Typography**: Full customizer control over font sizes, line heights, letter spacing, and paddings for all screen widths.
- **Zero Heavy Dependencies**: Pure semantic Liquid, HTML5, and scoped CSS with no external frameworks.

---

## 🚀 How to Use

1. Copy [`lifestyle_showcase.liquid`](lifestyle_showcase.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template.
3. Click **Add section** and select **Lifestyle Showcase (The Bond)**.
4. Add lifestyle cards, upload your photography (or supply external image URLs), and configure your headlines and CTAs.

---

## ⚙️ Schema Settings

### Header Text Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `tagline` | `text` | `THE BOND` | Uppercase tracking tagline above headline |
| `tagline_size` | `range` | `11px` | Tagline font size |
| `tagline_spacing` | `range` | `3px` | Tagline letter spacing |
| `heading` | `textarea` | `It was always there.` | Main section heading |
| `highlight_text` | `text` | `Now, you can hear it.` | Word(s) in heading to render with gradient text |
| `highlight_new_line` | `checkbox` | `true` | Place gradient text on its own line |
| `description` | `textarea` | *Description copy* | Editorial narrative text below heading |
| `heading_size_desktop` / `_mobile` | `range` | `56px` / `32px` | Responsive heading font sizes |
| `heading_weight` | `select` | `800` | Font weight: `600`, `700`, `800`, or `900` |
| `heading_align` | `select` | `left` | Alignment: `left`, `center`, or `right` |

### Color & Gradient Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `bg_color` | `color` | `#000000` | Section background color |
| `gradient_start` | `color` | `#2e5bff` | Primary gradient color (Cyan / Blue) |
| `gradient_end` | `color` | `#a855f7` | Secondary gradient color (Purple / Magenta) |
| `heading_color` | `color` | `#ffffff` | Primary heading color |
| `subheading_color` | `color` | `#8a8f98` | Tagline text color |
| `card_border_color` | `color` | `rgba(255, 255, 255, 0.08)` | Card border stroke color |

### Ambient Background Glow

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_glow` | `checkbox` | `true` | Enable ambient background blur glow |
| `glow_opacity` | `range` | `15%` | Glow intensity (0% to 100%) |
| `glow_size` | `range` | `650px` | Glow blur diameter (200px to 1000px) |
| `glow_blur` | `range` | `120px` | Gaussian blur filter radius |
| `glow_right` / `glow_top` | `range` | `20%` / `0%` | Horizontal and vertical glow position |

### Card Style & Aspect Ratio

| Setting | Type | Default | Description |
|---|---|---|---|
| `enable_rim_glow` | `checkbox` | `true` | Enable glowing rim highlight on card borders |
| `rim_glow_color` | `color` | `rgba(46, 91, 255, 0.2)` | Rim glow color |
| `card_radius` | `range` | `24px` | Card corner radius |
| `img_aspect_ratio` | `select` | `4 / 5` | `4:5` (Portrait), `9:16` (Tall), `1:1` (Square), or `3:4` (Standard) |
| `card_title_color` | `color` | `#ffffff` | Card overlay tag color |
| `card_desc_color` | `color` | `rgba(255, 255, 255, 0.78)` | Card overlay description color |

### Layout & Spacing

| Setting | Type | Default | Description |
|---|---|---|---|
| `container_max_width` | `range` | `1280px` | Container maximum width |
| `cols_desktop` | `select` | `3` | Columns on desktop (`2`, `3`, or `4`) |
| `cols_mobile` | `select` | `1` | Columns on mobile (`1` or `2`) |
| `grid_gap` | `range` | `24px` | Space between cards in grid |
| `padding_top_desktop` / `_mobile` | `range` | `120px` / `80px` | Section top padding |
| `padding_bottom_desktop` / `_mobile` | `range` | `120px` / `80px` | Section bottom padding |

### Bottom CTA Banner

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_bottom_cta` | `checkbox` | `true` | Toggle bottom CTA banner |
| `bottom_tagline` | `text` | `A NEW WAY TO EXPERIENCE` | Banner eyebrow text |
| `bottom_heading` | `textarea` | `THE BOND YOU ALREADY SHARE.` | Banner headline |
| `bottom_btn_style` | `select` | `arrow` | `Pill Button with Arrow` or `Circular Play Icon Button` |
| `button_text` | `text` | `DISCOVER PETRIX` | Button label |
| `button_link` | `url` | *empty* | Button destination URL |

---

## 🧱 Blocks (`lifestyle_card`)

| Setting | Type | Default | Description |
|---|---|---|---|
| `image` | `image_picker` | — | Upload card image from Shopify Theme |
| `image_url` | `text` | *fallback url* | Direct image URL fallback |
| `title` | `text` | `FAMILY, REIMAGINED` | Uppercase card tag/title |
| `description` | `textarea` | *copy* | Card narrative caption |
| `card_link` | `url` | *empty* | Optional click-through link for the entire card |

---

## 💻 Tech & Compatibility

- **Shopify Compatibility**: Online Store 2.0 (OS 2.0)
- **Zero Dependencies**: Pure Liquid, HTML5, and modern CSS (Flexbox / CSS Grid)
- **Performance**: High performance with responsive image sizes and lazy-loading
- **License**: MIT

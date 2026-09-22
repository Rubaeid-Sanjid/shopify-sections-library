# Image with Text (Gradient BG / Product Spotlight)

A sleek, modern **Product Spotlight & Feature Showcase** section with an ambient radial gradient glow background for Shopify Online Store 2.0 themes. Designed specifically for tech gadgets, smart pet devices, wearable hardware, and premium DTC products to highlight product imagery alongside feature pill badges.

Features a split 2-column layout, glowing ambient backdrop, interactive feature pill cards with vector icons, gradient-highlighted headline copy, and subtle corner overlay badges on the product visual.

![Product Spotlight Preview](image_with_text_gradient_BG.png)

---

## ✨ Features

- **Atmospheric Radial Gradient Glow**: Beautiful glowing radial backdrop behind the product image, customizable in color and intensity.
- **Gradient Heading Text Highlight**: Highlight specific words in your headline with a vibrant gradient color simply by typing the word into the customizer.
- **Top Category / Status Tag**: Uppercase pill tag with a glowing status dot to demarcate device models or product series.
- **Interactive Feature Pills**: Grid of block-based benefit pills with subtle hover lift, border glow, and built-in vector icons:
  - 🪶 `feather` (Lightweight & durable)
  - 💧 `droplet` (Water resistant / Splash-proof)
  - 🔋 `battery` (Long battery life)
  - 🛡️ `shield` (Protection / All-day comfort)
  - ⚡ `zap` (Fast / Power / Quick charge)
  - ✔️ `check` (Checkmark / Verified)
  - ⭐ `star` (Top rated / Premium)
  - ❤️ `heart` (Health & care)
- **Product Visual Frame**: Rounded product image container with ambient shadow glow and futuristic corner overlay labels (`IP-RATED • WATER RESISTANT`, `PETRIX™`).
- **Accent CTA Link**: Arrow link button with smooth hover transition.
- **Responsive Layout**: Adapts cleanly from a 2-column desktop split to a single-column stacked mobile flow with customizable padding.
- **Zero Heavy Dependencies**: Pure semantic Liquid, modern CSS, and Vanilla JS custom element without third-party frameworks.

---

## 🚀 How to Use

1. Copy [`image_with_text_gradient_BG.liquid`](image_with_text_gradient_BG.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template (Homepage, Product page, Landing page, etc.).
3. Click **Add section** and search for **Product spotlight**.
4. Upload your product photo, adjust the gradient glow color, and configure feature blocks as needed.

---

## ⚙️ Schema Settings

### Layout & Background

| Setting | Type | Default | Description |
|---|---|---|---|
| `section_padding_desktop` | `range` | `80px` | Section top and bottom padding on desktop |
| `section_padding_mobile` | `range` | `40px` | Section top and bottom padding on mobile |
| `background_color` | `color` | `#000000` | Section background color |
| `glow_color` | `color` | `#7033ff` | Radial ambient glow backdrop color |

### Header & Copy

| Setting | Type | Default | Description |
|---|---|---|---|
| `top_tag` | `text` | `THE PETRIX DEVICE` | Top pill badge text |
| `tag_color` | `color` | `#a78bfa` | Top pill badge text color |
| `tag_dot_color` | `color` | `#8b5cf6` | Pulsing dot color next to tag text |
| `heading` | `text` | `Premium design. Made for every adventure.` | Main section heading |
| `heading_highlight` | `text` | *empty* | Exact word(s) in heading to receive gradient highlight |
| `heading_size` | `range` | `48px` | Desktop heading font size |
| `heading_color` | `color` | `#ffffff` | Primary heading text color |
| `description` | `textarea` | *Description text* | Editorial description below heading |
| `description_size` | `range` | `16px` | Desktop description font size |
| `description_color` | `color` | `#c4b5fd` | Description text color |

### Feature Pills Styling

| Setting | Type | Default | Description |
|---|---|---|---|
| `feature_pill_bg` | `color` | `rgba(255, 255, 255, 0.05)` | Feature pill background |
| `feature_pill_hover_bg` | `color` | `rgba(255, 255, 255, 0.08)` | Feature pill background on hover |
| `feature_pill_border` | `color` | `rgba(255, 255, 255, 0.1)` | Pill border color |
| `feature_pill_hover_border` | `color` | `rgba(255, 255, 255, 0.2)` | Pill border color on hover |
| `feature_pill_radius` | `range` | `12px` | Pill corner radius |
| `feature_icon_color` | `color` | `#a78bfa` | Icon color inside feature pills |
| `feature_text_color` | `color` | `#ffffff` | Feature pill title text color |
| `feature_desc_color` | `color` | `#c4b5fd` | Feature pill description text color |

### Product Image & Overlays

| Setting | Type | Default | Description |
|---|---|---|---|
| `product_image` | `image_picker` | — | Product or device photograph |
| `image_border_radius` | `range` | `24px` | Border radius for the product image |
| `image_glow_color` | `color` | `#7033ff` | Soft ambient glow behind the image |
| `overlay_left_text` | `text` | `IP-RATED • WATER RESISTANT` | Bottom left overlay tag text |
| `overlay_right_text` | `text` | `PETRIX™` | Bottom right overlay badge text |
| `overlay_text_color` | `color` | `#ffffff` | Text color for image overlay tags |

### Call to Action (CTA)

| Setting | Type | Default | Description |
|---|---|---|---|
| `cta_text` | `text` | `EXPLORE THE DEVICE` | Button / link text |
| `cta_link` | `url` | *empty* | Target URL for CTA |
| `cta_color` | `color` | `#a78bfa` | Link color |
| `cta_hover_color` | `color` | `#ffffff` | Link hover color |

---

## 🧱 Blocks (`feature`)

Merchants can add, remove, and reorder feature blocks:

| Setting | Type | Default | Description |
|---|---|---|---|
| `icon` | `select` | `feather` | Icon choice (`feather`, `droplet`, `battery`, `shield`, `zap`, `check`, `star`, `heart`, or `none`) |
| `title` | `text` | `Lightweight & durable` | Feature title |
| `description` | `text` | *Short description* | Concise supporting sentence |

---

## 💻 Tech & Compatibility

- **Shopify Compatibility**: Online Store 2.0 (OS 2.0)
- **Zero Dependencies**: Pure Liquid, HTML5, CSS, and lightweight Vanilla JS
- **Performance**: High performance with CSS hardware acceleration and responsive image sizing
- **License**: MIT

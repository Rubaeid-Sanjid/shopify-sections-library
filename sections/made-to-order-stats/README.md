# Made to Order Stats / Production Process Showcase

A high-converting, modern **"Made to Order" Brand Narrative & Production Stats Banner** section for Shopify Online Store 2.0 themes. Designed specifically for custom merchandise, DTC athletic brands, made-to-order apparel, bespoke goods, and specialized manufacturers.

Features bold athletic italic display typography, custom metrics grid with vertical blue-accented dividers, pill call-to-action button, smooth animated counter effect, and an atmospheric dark workshop background with customizable gradient overlays.

![Made to Order Stats Preview](preview.png)

---

## ✨ Features

- **Bold Athletic Design System**:
  - High-impact italicized uppercase headlines and tracked cyan/blue eyebrow label.
  - Matches DTC athletic brands, custom merchandise shops, and modern apparel stores.
- **Key Production Metrics & Stat Grid**:
  - Showcase lead times, minimum order quantities (MOQ), color variants, and manufacturing origins (e.g. `4–5 weeks`, `25 pieces MOQ`, `11 terry colours`, `100% EU produced`).
  - Seamless horizontal desktop alignment with automatic 2-column or stacked mobile fallback.
- **Segmented Vertical Dividers**:
  - Sleek vertical dividers separating each metric.
  - Features an eye-catching electric blue accent bar at the top with a subtle translucent line body, precisely matching the reference aesthetic.
- **Optional Number Counter Animation**:
  - Smooth JavaScript counter effect powered by `IntersectionObserver` that counts up when scrolled into view, with support for percentages (`100%`), discrete values (`25`), and graceful fallback for date ranges (`4–5`).
- **Atmospheric Dark Backdrop & Gradient Overlay**:
  - Configurable desktop and mobile background image picker.
  - Directional gradient overlay ensuring ultra-crisp white text readability on the left while revealing ambient workshop depth on the right.
  - Built-in, high-fidelity SVG illustration fallback so the section looks stunning right out of the box even before custom imagery is uploaded.
- **Call-to-Action Pill Button**:
  - Prominent pill-shaped CTA button with smooth lift hover animation and vibrant glowing shadow.
- **Fully Modular Blocks**:
  - Add, remove, or reorder stat metric blocks dynamically through the Shopify Theme Editor.
- **Zero Heavy Dependencies**:
  - Pure semantic HTML5, scoped CSS variables, and lightweight Vanilla JavaScript. No jQuery, Tailwind, or external libraries required.

---

## 🚀 How to Install & Use

1. Copy [`made-to-order-stats.liquid`](made-to-order-stats.liquid) into your Shopify theme's `sections/` directory.
2. In your Shopify Admin, navigate to **Online Store > Themes > Customize**.
3. Go to any page template (Homepage, Product page, Custom Merch Landing page, About Us, etc.).
4. Click **Add section** and choose **Made to Order Stats**.
5. Customize the headline, lead times, stat metrics, CTA button, and background image to fit your brand.
6. Click **Save**.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `eyebrow` | `text` | `MADE TO ORDER, MADE IN EUROPE` | Tracking label above the heading |
| `eyebrow_color` | `color` | `#0084ff` | Eyebrow label color |
| `eyebrow_size` | `range` | `13px` | Font size of the eyebrow label |
| `heading` | `text` | `CUSTOM WORK TAKES A FEW WEEKS. THAT IS THE POINT.` | Main section headline |
| `heading_tag` | `select` | `h2` | HTML heading tag (`h1`, `h2`, `h3`, `div`) |
| `heading_color` | `color` | `#ffffff` | Color of the main heading |
| `heading_size_desktop` | `range` | `46px` | Desktop heading font size |
| `heading_size_mobile` | `range` | `30px` | Mobile heading font size |
| `description` | `richtext` | *(copy)* | Supporting brand narrative copy |
| `description_color` | `color` | `#cbd5e1` | Description text color |
| `description_size_desktop` | `range` | `16px` | Desktop description font size |
| `description_size_mobile` | `range` | `15px` | Mobile description font size |
| `content_max_width` | `range` | `640px` | Maximum width of the text column |
| `stat_number_color` | `color` | `#ffffff` | Color of the metric numbers |
| `stat_number_size_desktop` | `range` | `52px` | Metric number font size on desktop |
| `stat_number_size_mobile` | `range` | `36px` | Metric number font size on mobile |
| `stat_label_color` | `color` | `#cbd5e1` | Color of the metric labels |
| `stat_label_size` | `range` | `13px` | Font size of the metric labels |
| `divider_color` | `color` | `rgba(255, 255, 255, 0.16)` | Base line color for vertical dividers |
| `divider_accent_color` | `color` | `#0084ff` | Electric top accent bar color for dividers |
| `enable_counter_animation` | `checkbox` | `true` | Animate numbers counting up on scroll |
| `button_label` | `text` | `SEE THE FULL PROCESS` | Primary CTA button text |
| `button_link` | `url` | — | Destination link for the CTA button |
| `button_bg_color` | `color` | `#0084ff` | Button background color |
| `button_text_color` | `color` | `#ffffff` | Button label text color |
| `button_bg_hover` | `color` | `#006ed6` | Button background color on hover |
| `background_image` | `image_picker` | — | High-res desktop background photo |
| `background_image_mobile` | `image_picker` | — | Optional mobile background photo override |
| `show_fallback_backdrop` | `checkbox` | `true` | Show realistic atelier illustration when no photo is uploaded |
| `bg_color` | `color` | `#080d16` | Background color fallback |
| `overlay_color_left` | `color` | `#080d16` | Left side gradient overlay color |
| `overlay_color_right` | `color` | `#080d16` | Right side gradient overlay color |
| `overlay_opacity_left` | `range` | `94%` | Left gradient opacity (ensures text readability) |
| `overlay_opacity_right` | `range` | `55%` | Right gradient opacity (reveals workshop background) |
| `min_height_desktop` | `range` | `540px` | Minimum banner height on desktop |
| `container_max_width` | `range` | `1320px` | Maximum container width |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `90px` | Top & bottom vertical padding on desktop |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `56px` | Top & bottom vertical padding on mobile |

---

### Block Settings (`stat_item`)

| Setting | Type | Default | Description |
|---|---|---|---|
| `stat_value` | `text` | `25` | The metric value (e.g. `4–5`, `25`, `11`, `100%`) |
| `stat_label` | `text` | `pieces minimum order...` | The metric description or explanation |
| `custom_accent_color` | `color` | *(empty)* | Optional override for the divider accent color on this specific item |

---

## 🎨 Design Customization Tips

- **Match Your Brand Palette**:
  - For high-energy athletic brands, pair electric blue (`#0084ff`), safety orange (`#ff5722`), or neon lime (`#10b981`) with pure white headlines.
- **Custom Workshop Photography**:
  - Upload a photo of your factory floor, design desk, sewing stations, or textile rolls. The built-in left-to-right gradient overlay automatically balances high readability for text while showcasing authentic craft photography.
- **Complementary Pairing**:
  - Pairs perfectly with [`how-it-works-steps`](../how-it-works-steps) and [`custom-product-cards`](../custom-product-cards) to create an end-to-end custom merchandise or made-to-order landing page.

---

## 📄 License

MIT — Free to use and modify in personal and commercial Shopify projects.

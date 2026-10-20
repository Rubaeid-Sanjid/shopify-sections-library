# Custom Product Cards

A high-converting, modern **Custom Product Cards & Collection Showcase** section for Shopify Online Store 2.0 themes. Designed specifically for custom merchandise, athletic gear, fitness accessories, promotional products, and direct-to-consumer (DTC) brands offering customized or made-to-order collections.

Features bold athletic condensed typography, floating pill badges, accent divider bars, dynamic pricing notes, interactive color swatches with live color name labels, and a built-in interactive **Logo Upload & Mockup Preview Modal**.

![Custom Product Cards Preview](preview.png)

---

## ✨ Features

- **Shopify Product Integration or Custom Override**: Select an existing Shopify catalog product via the native product picker, or use the custom fields to specify titles, prices, descriptions, and swatches.
- **Interactive Color Swatches**:
  - Displays dynamic swatch count (e.g. `11 COLOURS`) and live active color label (`Green`, `White`, etc.).
  - Clicking any swatch moves the checkmark indicator with smooth micro-animation.
  - Updates the active color label in real time.
  - Automatically morphs the color of the realistic vector fallback illustration or swaps variant images.
- **High-Fidelity Realistic Fallback Illustrations**:
  - Automatically renders studio-quality, realistic vector SVG artwork for the **Wrist Sweatband** (with woven terry cloth texture, depth shading, cast ground shadow, and embroidered chevron logo) and the **Terry Headband**.
  - No empty placeholders if product photography is still in progress!
- **Interactive "Upload Your Logo" Modal**:
  - Clicking **UPLOAD YOUR LOGO** can trigger an accessible modal dialog.
  - Customers can drag & drop or upload their logo file (`PNG`, `SVG`, `JPG`, `WebP`).
  - **Live Mockup Preview**: The customer's logo is rendered on the product card in real time!
  - Branding method selector (`3D / Direct Embroidery`, `Woven Damask Patch`, `Screen Print`).
  - Order quantity input with dynamic volume pricing tier breakdown.
- **Volume Pricing & Price Notes**:
  - Highlights starting price (`From €2.45`) alongside subtle volume discount notes (`per piece · volume pricing available`).
- **Accent Divider Bar**:
  - Customizable horizontal accent bar (color, width, height) separating the product media from the product description.
- **Floating Pill Badges**:
  - Customizable pill badge (`Made to order · 4–5 weeks`) with custom background, text, and border colors.
- **Flexible Section Header**:
  - Eyebrow text (`THE COLLECTION`).
  - High-impact italicized uppercase headline (`TWO BANDS. EVERY COLOUR. YOUR LOGO.`).
  - Editorial description and top-right **SHOP ALL →** link with hover arrow animation.
- **Responsive Layout Modes**:
  - **Desktop**: Configurable 1 to 4 columns (defaults to 2 columns matching reference design).
  - **Mobile**: Select between clean **Vertical Stack** or touch-friendly **Swipeable Slider** with peek preview.
- **Zero Heavy Dependencies**:
  - Pure semantic HTML5, scoped CSS variables, and lightweight Vanilla JavaScript. No external libraries or framework dependencies required.

---

## 🚀 How to Use

1. Copy [`custom-product-cards.liquid`](custom-product-cards.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template (Homepage, Collection page, Landing page, Product page, etc.).
3. Click **Add section** and choose **Custom Product Cards**.
4. Configure your section header, layout preferences, and customize each product card block with your catalog products or custom promotional details.
5. Save and publish your changes.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_header` | `checkbox` | `true` | Toggle display of the section header |
| `eyebrow` | `text` | `THE COLLECTION` | Tracking label above the headline |
| `eyebrow_color` | `color` | `#0284c7` | Eyebrow text color |
| `eyebrow_size` | `range` | `13px` | Eyebrow font size (`10px` to `18px`) |
| `heading` | `text` | `TWO BANDS. EVERY COLOUR. YOUR LOGO.` | Main section heading |
| `heading_tag` | `select` | `h2` | Semantic HTML heading tag (`h1`, `h2`, `h3`, `div`) |
| `heading_italic` | `checkbox` | `true` | Apply athletic italic styling to heading |
| `heading_color` | `color` | `#0b1320` | Heading color |
| `heading_size` | `range` | `44px` | Desktop heading font size (`24px` to `64px`) |
| `description` | `textarea` | *(copy)* | Supporting description copy |
| `description_color` | `color` | `#64748b` | Description text color |
| `show_shop_all` | `checkbox` | `true` | Toggle display of "Shop All" link |
| `shop_all_text` | `text` | `SHOP ALL` | Link text |
| `shop_all_url` | `url` | — | Destination collection or page URL |
| `shop_all_color` | `color` | `#0b1320` | Link color |
| `container_max_width` | `range` | `1280px` | Maximum container width (`900px` to `1600px`) |
| `desktop_columns` | `range` | `2` | Number of columns on desktop (`1` to `4`) |
| `mobile_layout` | `select` | `stacked` | Mobile layout style (`Vertical Stack` or `Touch Swipeable Slider`) |
| `card_gap_desktop` | `range` | `28px` | Space between cards on desktop |
| `card_gap_mobile` | `range` | `16px` | Space between cards on mobile |
| `section_bg` | `color` | `#ffffff` | Background color for the entire section |
| `accent_color` | `color` | `#0284c7` | Global accent color for links, buttons, and active rings |
| `card_bg_color` | `color` | `#ffffff` | Background color of each card |
| `card_border_color` | `color` | `#e2e8f0` | Card border stroke color |
| `card_border_radius` | `range` | `24px` | Corner radius for cards (`8px` to `40px`) |
| `card_hover_lift` | `checkbox` | `true` | Lift card and add soft elevation shadow on hover |
| `enable_upload_modal` | `checkbox` | `true` | Enables interactive logo upload modal on button click |
| `modal_heading` | `text` | `Upload Your Brand Logo` | Heading inside customizer modal |
| `modal_subheading` | `text` | *(copy)* | Subheading instructions in modal |
| `volume_pricing_tiers` | `textarea` | *(tiers)* | Bulk discount tiers shown inside the modal |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `64px` | Vertical section padding on desktop |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `40px` | Vertical section padding on mobile |

---

### Block Settings (`product_card`)

Each product card block represents an individual item in the collection:

| Setting | Type | Default | Description |
|---|---|---|---|
| `product` | `product` | — | Optional Shopify product picker |
| `override_product` | `checkbox` | `false` | Override product title, description, and pricing with custom text below |
| `show_badge` | `checkbox` | `true` | Toggle pill badge display |
| `badge_text` | `text` | `Made to order · 4–5 weeks` | Badge copy |
| `badge_bg` | `color` | `#f8fafc` | Badge background color |
| `badge_text_color` | `color` | `#334155` | Badge text color |
| `badge_border_color` | `color` | `#e2e8f0` | Badge border outline color |
| `enable_custom_image` | `checkbox` | `false` | Enable to use the custom image below instead of the Shopify product image (keeps product title & price) |
| `image` | `image_picker` | — | Custom product image upload (renders fallback vector if empty) |
| `fallback_art_type` | `select` | `wristband` | Fallback vector style (`Wrist Sweatband` or `Terry Headband`) |
| `show_accent_bar` | `checkbox` | `true` | Toggle accent divider bar |
| `accent_bar_color` | `color` | `#0284c7` | Accent bar color |
| `accent_bar_width` | `range` | `80px` | Accent bar width (`40px` to `160px`) |
| `accent_bar_height` | `range` | `4px` | Accent bar thickness (`2px` to `8px`) |
| `title` | `text` | `CUSTOM WRIST SWEATBAND` | Product title |
| `title_tag` | `select` | `h3` | Semantic HTML tag (`h2`, `h3`, `h4`, `div`) |
| `title_color` | `color` | `#0b1320` | Title text color |
| `subtitle` | `textarea` | *(copy)* | Supporting subtitle / tagline |
| `subtitle_color` | `color` | `#64748b` | Subtitle text color |
| `price_prefix` | `text` | `From` | Price prefix text |
| `price` | `text` | `€2.45` | Main price display |
| `price_color` | `color` | `#0b1320` | Main price color |
| `price_subtext` | `text` | *(note)* | Secondary note (e.g. `per piece · volume pricing available`) |
| `price_subtext_color` | `color` | `#64748b` | Secondary note text color |
| `show_swatches` | `checkbox` | `true` | Toggle color swatches row |
| `swatches_label` | `text` | `11 COLOURS` | Swatches counter header label |
| `active_color_name` | `text` | `Green` | Initial active color label |
| `colors_list` | `textarea` | *(11 colors)* | Comma-separated list of colors in `Name:HexCode` format |
| `btn1_text` | `text` | `UPLOAD YOUR LOGO` | Primary CTA button label |
| `btn1_action` | `select` | `open_modal` | Action (`Open Logo Upload Modal` or `Navigate to Custom URL`) |
| `btn1_link` | `url` | — | Destination URL if action is set to link |
| `btn1_bg` | `color` | `#0284c7` | Primary button background |
| `btn1_text_color` | `color` | `#ffffff` | Primary button text color |
| `btn2_text` | `text` | `DETAILS` | Secondary CTA button label |
| `btn2_link` | `url` | — | Secondary button link URL |
| `btn2_bg` | `color` | `#ffffff` | Secondary button background |
| `btn2_border_color` | `color` | `#cbd5e1` | Secondary button outline border color |
| `btn2_text_color` | `color` | `#0b1320` | Secondary button text color |

---

## 🎨 Swatches Format

Colors can be configured in the `colors_list` setting using a simple comma-separated `Name:HexCode` format:

```text
Black:#111827, White:#ffffff, Red:#dc2626, Pink:#ec4899, Yellow:#eab308, Green:#059669, Navy:#1e3a8a, Gray:#94a3af, Purple:#7c3aed, Orange:#ea580c, Light Blue:#38bdf8
```

Each button renders the exact hex color, includes an accessible `aria-label`, and features an animated checkmark indicator when selected.

---

## 📦 Presets Included

The section comes pre-configured with a default preset matching the reference design:

1. **Card 1 (Custom Wrist Sweatband)**:
   - Badge: `Made to order · 4–5 weeks`
   - Title: `CUSTOM WRIST SWEATBAND`
   - Subtitle: `The classic terry wristband, printed with your logo`
   - Price: `From €2.45 per piece · volume pricing available`
   - Swatches: 11 colors, default active `Green`
   - CTAs: `UPLOAD YOUR LOGO` + `DETAILS →`

2. **Card 2 (Custom Terry Headband)**:
   - Badge: `Made to order · 4–5 weeks`
   - Title: `CUSTOM TERRY HEADBAND`
   - Subtitle: `Keep hair and sweat out of the way, with your logo front and centre`
   - Price: `From €3.20 per piece · volume pricing available`
   - Swatches: 11 colors, default active `White`
   - CTAs: `UPLOAD YOUR LOGO` + `DETAILS →`

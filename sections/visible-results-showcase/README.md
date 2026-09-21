# Visible Results Showcase

A modern, high-converting **Before & After Visual Proof & Results Showcase** section for Shopify Online Store 2.0 themes. Designed specifically for beauty, skincare, cosmetic tech, wellness, dental, and personal care brands to display clinical or real-customer transformation proof.

Features an elevated floating comparison card with side-by-side visual proof pairs, floating circular arrow indicators, uppercase tracking eyebrow, prominent headline, and pill-shaped benefit callouts with custom icons.

![Visible Results Showcase Preview](preview.png)

---

## ✨ Features

- **Elevated Visual Proof Card**: Floating card with customizable rounded corners (`border-radius: 24px`), soft elevation drop shadow, and clean card padding.
- **Dual Visual Proof Pairs**: Displays side-by-side comparison images with centered circular arrow indicators (`width: 32px; height: 32px; background: rgba(30, 41, 59, 0.65)` with backdrop blur and white chevron) connecting before and after states.
- **Interactive Drag Slider Mode**: In addition to the side-by-side layout, merchants can toggle an interactive before/after drag slider mode with touch and mouse dragging.
- **Pill-Shaped Benefit Badges**: Soft mint/pale-teal pill containers (`border-radius: 9999px`) with circular icon badges highlighting key product benefits and customer transformations.
- **Built-in SVG Icon Library**: Includes 8 pre-configured SVG icons (Sparkles, Checkmark, Shield, Heart, Droplet, Sun, Feather, Star) plus a custom SVG code override field.
- **Dual Block Architecture**:
  - `comparison_item`: Add, reorder, or customize before/after photo pairs with custom captions and optional corner tags.
  - `benefit_pill`: Add, reorder, or customize highlighted benefit callout pills with title, subtitle, and icons.
- **Flexible Column Ordering**: Configurable desktop layout (Card Left / Content Right vs. Content Left / Card Right) and mobile display order.
- **Zero Heavy Dependencies**: Pure semantic HTML, responsive modern CSS, and lightweight Vanilla JS only when interactive slider mode is enabled.
- **Built-in SVG Placeholders**: Automatically displays clean SVG illustrations when images are not yet selected, ensuring the theme editor looks polished immediately.

---

## 🚀 How to Use

1. Copy [`visible-results-showcase.liquid`](visible-results-showcase.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, open any page template (Product page, Landing page, Homepage, etc.).
3. Click **Add section** and select **Visible Results Showcase**.
4. Customize your section heading, eyebrow, description, and upload your before-and-after imagery.
5. Add or reorder **Comparison Pair** and **Benefit Pill** blocks as needed.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `section_bg` | `color` | `#f8fafc` | Background color for the whole section |
| `container_max_width` | `range` | `1180px` | Maximum container width |
| `desktop_layout` | `select` | `card_first` | Column layout on desktop (`Card Left / Text Right` or `Text Left / Card Right`) |
| `mobile_card_order` | `select` | `first` | Display order on mobile (`Card First` or `Text First`) |
| `padding_top_desktop` / `padding_bottom_desktop` | `range` | `80px` | Vertical padding on desktop screens |
| `padding_top_mobile` / `padding_bottom_mobile` | `range` | `48px` | Vertical padding on mobile screens |
| `card_bg_color` | `color` | `#ffffff` | Background color of the floating comparison card |
| `card_border_radius` | `range` | `24px` | Border radius of the card |
| `card_border_color` | `color` | `rgba(0, 0, 0, 0.04)` | Subtle border around the card |
| `card_shadow` | `text` | *(CSS shadow)* | Box shadow string for the floating card |
| `card_padding_desktop` / `_mobile` | `range` | `36px` / `20px` | Inner padding of the comparison card |
| `comparison_mode` | `select` | `side_by_side` | Presentation style: `Side by Side with Arrow Badge` or `Interactive Drag Before/After Slider` |
| `image_aspect_ratio` | `select` | `1 / 1` | Aspect ratio for photos (`Square 1:1`, `Landscape 4:3`, `Portrait 3:4`) |
| `image_border_radius` | `range` | `12px` | Corner radius for before/after photos |
| `show_arrow_badge` | `checkbox` | `true` | Toggle floating center circular arrow indicator |
| `arrow_badge_bg` | `color` | `rgba(30, 41, 59, 0.65)` | Background color of the circular arrow badge |
| `arrow_badge_icon_color` | `color` | `#ffffff` | Icon color for the arrow chevron |
| `arrow_badge_size` | `range` | `32px` | Diameter of the arrow badge |
| `show_before_after_tags` | `checkbox` | `false` | Optional floating "Before" & "After" text chips |
| `caption_color` | `color` | `#1e293b` | Color of the comparison caption under image pairs |
| `caption_font_size` | `range` | `14px` | Font size of comparison caption |
| `eyebrow` | `text` | `VISIBLE RESULTS` | Small tracking tag above main heading |
| `eyebrow_color` | `color` | `#0f766e` | Color of eyebrow text |
| `eyebrow_font_size` | `range` | `13px` | Font size of eyebrow text |
| `eyebrow_letter_spacing` | `range` | `1.5px` | Letter spacing / tracking for eyebrow |
| `heading` | `text` | `Lighten lines. Lift the jawline.` | Main section heading |
| `heading_tag` | `select` | `h2` | HTML tag for heading (`h1`, `h2`, `h3`, `div`) |
| `heading_color` | `color` | `#0f172a` | Color of the main heading |
| `heading_font_size_desktop` / `_mobile` | `range` | `40px` / `28px` | Responsive heading font size |
| `heading_margin_bottom` | `range` | `16px` | Spacing beneath heading |
| `description` | `textarea` | *(copy)* | Editorial narrative / benefit paragraph |
| `description_color` | `color` | `#475569` | Color of narrative paragraph |
| `description_font_size` | `range` | `16px` | Font size of description |
| `description_line_height` | `select` | `1.6` | Line height of description (`1.4`, `1.6`, `1.75`) |
| `description_margin_bottom` | `range` | `32px` | Spacing below description |
| `pill_bg_color` | `color` | `#eaf7f4` | Background color for benefit pills |
| `pill_hover_bg_color` | `color` | `#e2f5f1` | Hover background color for benefit pills |
| `pill_border_radius` | `range` | `9999px` | Border radius for benefit pills |
| `pill_icon_bg` | `color` | `#93e8c9` | Circular badge background for pill icon |
| `pill_icon_color` | `color` | `#065f46` | Fill color for pill icon |
| `pill_title_color` | `color` | `#0f172a` | Font color of benefit title |
| `pill_desc_color` | `color` | `#475569` | Font color of benefit description |
| `pill_spacing` | `range` | `16px` | Vertical gap between benefit pills |

---

### Block Settings

#### 1. `comparison_item` (Comparison Pair)
Add multiple before/after transformation pairs inside the card container.

| Setting | Type | Default | Description |
|---|---|---|---|
| `before_image` | `image_picker` | — | "Before" state image |
| `after_image` | `image_picker` | — | "After" state image |
| `caption` | `text` | `Lightens neck lines Skin becomes smooth` | Caption text rendered directly beneath the photo pair |
| `before_label` | `text` | `Before` | Label shown if corner tags are enabled |
| `after_label` | `text` | `After` | Label shown if corner tags are enabled |

#### 2. `benefit_pill` (Benefit Pill)
Highlight individual claims, clinical results, or customer perks with rounded pill callouts.

| Setting | Type | Default | Description |
|---|---|---|---|
| `icon` | `select` | `sparkles` | Preset SVG icon (`sparkles`, `check`, `shield`, `heart`, `droplet`, `sun`, `feather`, `star`) |
| `custom_icon_svg` | `html` | — | Custom inline SVG code (overrides preset icon) |
| `title` | `text` | `Lightens neck lines` | Bold title for the benefit item |
| `description` | `text` | `Skin becomes visibly smoother.` | Supporting copy / explanation |

---

## 🎨 Presets Included

The section includes a complete ready-to-use preset matching the reference design:

1. **Comparison Pair 1**:
   - Caption: `Lightens neck lines Skin becomes smooth`
2. **Comparison Pair 2**:
   - Caption: `Relieve sagging skin on face and jaw`
3. **Benefit Pill 1**:
   - Icon: `sparkles`
   - Title: `Lightens neck lines`
   - Description: `Skin becomes visibly smoother.`
4. **Benefit Pill 2**:
   - Icon: `sparkles`
   - Title: `Relieves sagging skin`
   - Description: `Face and jaw feel firmer and more lifted.`

---

## 💡 Best Practices & Tips

- **Image Dimensions**: Square images (`600x600px` to `800x800px`) work best for consistency between before and after shots.
- **Lighting & Angle**: For maximum conversion impact, ensure before and after photos share identical lighting and angle.
- **Color Customization**: If your brand uses a different accent color (e.g. rose gold, lavender, or medical blue), adjust `eyebrow_color`, `pill_bg_color`, and `pill_icon_bg` to match your store's palette seamlessly.

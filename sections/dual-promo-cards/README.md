# Dual Promo Cards

A modern, high-converting **2-Column Promotional Banner Cards** section for Shopify Online Store 2.0 themes. Designed specifically for lifestyle, travel, wellness, fashion, gifting, and DTC brands to feature curated collections, gift guides, travel essentials, or seasonal campaigns.

Features wide rounded promo tiles (`border-radius: 24px`), built-in pill badges with icons, atmospheric dark vignette gradient overlays for optimal text legibility, bold headlines, concise copy, and hover-animated arrow CTA links.

![Dual Promo Cards Preview](preview.png)

---

## ✨ Features

- **Dual-Card Promo Grid**: 2-column responsive layout showcasing complementary campaigns (e.g. *Travel Essentials* alongside *Gift Ideas*).
- **Floating Pill Badges**: Soft mint/pastel rounded badges (`border-radius: 9999px`) with customizable icons and text.
- **Built-in SVG Icon Library**: Includes 10 pre-configured vector icons:
  - ✈️ `airplane` (Travel / Jetsetter / Holiday)
  - 🎁 `gift` (Gift Ideas / Holiday Guide)
  - ✨ `sparkles` (Featured / New)
  - ⭐ `star` (Bestsellers / Top Rated)
  - ❤️ `heart` (Staff Picks / Favorites)
  - 🛍️ `bag` (Shopping / Collection)
  - 🏷️ `tag` (Special Offers / Sale)
  - 🧭 `compass` (Adventure / Outdoor)
  - 🔥 `fire` (Trending / Hot)
  - 🚚 `truck` (Express Shipping)
  - Custom inline SVG support via `custom` option.
- **Deep Vignette Gradient Overlay**: Smooth gradient overlay ensuring high contrast and effortless legibility for white text over any photography.
- **Responsive Mobile Modes**:
  - **Vertical Stack**: Clean single-column stack on mobile devices.
  - **Swipeable Carousel**: Touch-friendly scroll-snap track where the next card peeks into view, encouraging swiping.
- **Hover Micro-Interactions**:
  - Smooth image zoom (`transform: scale(1.05)`) with ease-out curve.
  - Card lift with soft elevation shadow.
  - Arrow CTA translates horizontally on hover (`transform: translateX(5px)`).
- **Built-in Fallback Vector Artwork**: Automatically displays clean, vector flatlay and lifestyle illustrations when photos are not yet uploaded in the theme customizer.
- **Full-Card Click Option**: Merchants can make the entire card clickable or keep it as an inline text link.
- **Zero Heavy Dependencies**: Pure semantic HTML5, modern scoped CSS variables, and lightweight Vanilla liquid — no external scripts or stylesheets required.

---

## 🚀 How to Use

1. Copy [`dual-promo-cards.liquid`](dual-promo-cards.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template (Homepage, Collection page, Landing page, etc.).
3. Click **Add section** and select **Dual Promo Cards**.
4. Upload your card imagery, customize badge text and icons, and configure your headlines and links.
5. Add up to 6 promo card blocks if you wish to showcase a larger campaign grid.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `section_bg` | `color` | `#ffffff` | Background color for the whole section |
| `container_max_width` | `range` | `1280px` | Maximum container width (`900px` to `1600px`) |
| `desktop_columns` | `range` | `2` | Number of columns on desktop (`1` to `3`) |
| `mobile_layout` | `select` | `stacked` | Mobile layout style (`Vertical Stack` or `Swipeable Carousel`) |
| `card_border_radius` | `range` | `24px` | Corner radius for the promo cards |
| `card_min_height_desktop` | `range` | `440px` | Minimum card height on desktop |
| `card_min_height_mobile` | `range` | `360px` | Minimum card height on mobile |
| `card_gap_desktop` / `_mobile` | `range` | `24px` / `16px` | Gap between cards |
| `card_padding_desktop` / `_mobile` | `range` | `36px` / `24px` | Inner content padding |
| `enable_image_zoom` | `checkbox` | `true` | Image zoom animation on desktop hover |
| `enable_hover_lift` | `checkbox` | `true` | Card lift and elevation shadow on hover |
| `eyebrow` | `text` | — | Optional tracking label above the section |
| `heading` | `text` | — | Optional section heading |
| `description` | `textarea` | — | Optional editorial description above the cards |
| `header_alignment` | `select` | `left` | Alignment of optional section header (`Left` or `Center`) |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `64px` | Vertical section padding on desktop |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `40px` | Vertical section padding on mobile |

---

### Block Settings (`promo_card`)

Each promo card can be independently customized:

| Setting | Type | Default | Description |
|---|---|---|---|
| `image` | `image_picker` | — | Primary background image (desktop) |
| `image_mobile` | `image_picker` | — | Optional portrait/square image for mobile screens |
| `overlay_color` | `color` | `#0b151b` | Base color for bottom vignette gradient |
| `overlay_opacity` | `range` | `75%` | Overall opacity of the gradient overlay |
| `overlay_gradient_mid` | `range` | `45%` | Midpoint height where gradient darkens |
| `show_badge` | `checkbox` | `true` | Toggle display of the pill badge |
| `badge_text` | `text` | `Travel Essentials` | Label rendered inside the pill badge |
| `badge_icon` | `select` | `airplane` | Preset SVG icon (`airplane`, `gift`, `sparkles`, `star`, `heart`, etc.) |
| `custom_badge_svg` | `html` | — | Custom SVG markup (used if icon is set to `Custom`) |
| `badge_bg_color` | `color` | `#bbf7d0` | Background color of pill badge |
| `badge_text_color` | `color` | `#064e3b` | Text and icon color of pill badge |
| `title` | `text` | `Perfect for travel` | Main headline of the card |
| `title_tag` | `select` | `h3` | Semantic HTML heading tag (`h2`, `h3`, `h4`, `div`) |
| `title_color` | `color` | `#ffffff` | Color of the card headline |
| `description` | `textarea` | *(copy)* | Supporting description copy |
| `description_color` | `color` | `#f3f4f6` | Color of the description copy |
| `content_vertical_align` | `select` | `bottom` | Vertical alignment (`Bottom`, `Center`, `Top`) |
| `link_text` | `text` | `Shop travel picks` | Text for the call-to-action link |
| `link_url` | `url` | — | Destination URL for the CTA |
| `link_style` | `select` | `arrow` | Presentation (`Text Link with Arrow` or `Rounded Pill Button`) |
| `show_arrow` | `checkbox` | `true` | Display right chevron arrow on link |
| `link_color` | `color` | `#76e5b5` | Accent color for link and arrow |
| `link_hover_color` | `color` | `#a7f3d0` | Hover color for link and arrow |
| `enable_full_card_link` | `checkbox` | `false` | Makes the entire card surface clickable |
| `open_in_new_tab` | `checkbox` | `false` | Opens link in a new browser tab |

---

## 🎨 Presets Included

The section includes a complete ready-to-use preset matching the reference design:

1. **Card 1 (Travel Essentials)**:
   - Badge: `Travel Essentials` (with Airplane icon)
   - Title: `Perfect for travel`
   - Description: `Fold it into your carry-on and arrive restored — not wrecked.`
   - CTA: `Shop travel picks →`
2. **Card 2 (Gift Ideas)**:
   - Badge: `Gift Ideas` (with Gift Box icon)
   - Title: `The perfect gift`
   - Description: `Give the people you love the gift of genuine relief.`
   - CTA: `Shop gifts →`

---

## 💡 Best Practices & Tips

- **Image Dimensions**: High-resolution landscape or 4:3 images (`1200x900px` or `1400x1000px`) deliver razor-sharp results on Retina and 4K displays.
- **Focal Points**: Position primary visual subjects in the upper-center or upper-right of your photos so they remain unobstructed by the text placed at the bottom-left.
- **Overlay Customization**: If your imagery is naturally brighter or darker, adjust `overlay_opacity` and `overlay_gradient_mid` to balance subject visibility and text contrast.
- **Full Card Click**: For mobile users, turning on `enable_full_card_link` makes it easier to tap anywhere on the banner without needing to hit the text link specifically.

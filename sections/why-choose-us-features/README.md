# Why Choose Us (Center Image Features)

A high-converting, 3-column feature section designed for Shopify Online Store 2.0 themes. It showcases a central product or pet hero image flanked by 3 customizable feature/benefit cards on each side.

Built with pure Vanilla CSS and semantic Liquid with zero external JavaScript dependencies, complete mobile responsiveness, and granular customization controls for both desktop and mobile views.

---

## 🌟 Key Features

- **3-Column Center-Focus Layout**: Perfectly balances a central hero image (dog, pet, product, or lifestyle photo) with feature items on the left and right.
- **Block-Based Architecture (`feature_item`)**: Add, delete, reorder, or position items on the Left or Right column easily through Shopify Theme Customizer.
- **12+ Built-in SVG Icons**: Includes handcrafted, lightweight vector icons ready out of the box (Smart Feeder, Safe Walks Leash, Grooming Tools, Travel Carrier, Healthy Pet Bowl, Free Shipping Truck, Paw Print, Heart Care, Shield, Star, 24/7 Clock, Organic Leaf).
- **Custom Icon Support**: Upload your own image icons (PNG/SVG/WebP) or paste raw inline SVG code directly in block settings.
- **Granular Desktop & Mobile Customization**:
  - Independent font sizes for headings, subheadings, titles, and descriptions.
  - Independent section padding (top & bottom) for mobile and desktop.
  - Independent icon and image dimensions for mobile and desktop.
- **Flexible Mobile Modes**:
  - **Stacked (Middle Image)**: Features flow naturally (Left items &rarr; Center Image &rarr; Right items).
  - **Image Top**: Center Image appears first on mobile, followed by items below.
  - **Image Bottom**: Features appear first, image at the bottom.
  - **Compact 2-Column Grid**: Items arranged in a clean 2-column grid on mobile screens.
  - **Horizontal Slider**: Swipeable scroll-snap carousel on mobile.
- **Smooth Micro-Interactions**: Subtle hover lift effects on cards, icon zoom, ambient background glow, and optional gentle floating animation on the center image.
- **Optional Bottom CTA Button**: Configurable pill button with arrow icon linking to any page or collection.

---

## 🚀 How to Install & Use

1. In your Shopify Admin, go to **Online Store** &rarr; **Themes** &rarr; **Edit code**.
2. Under the **Sections** directory, click **Add a new section**.
3. Name the file `why-choose-us-features.liquid`.
4. Copy the entire contents of [`why-choose-us-features.liquid`](file:///c:/Users/Rubaeid%20Sanjid/Downloads/Sanjid/shopify_theme_sections/shopify-sections-library/sections/why-choose-us-features/why-choose-us-features.liquid) and paste it into the new file.
5. Click **Save**.
6. Open the **Theme Customizer** (Customize), navigate to any page (e.g., Homepage or Product page), click **Add section**, and select **Why Choose Us (Features)**.

---

## ⚙️ Schema Settings Reference

### 🎨 Section Layout & Background

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `bg_color` | `color` | `#FFF6E5` | Section background color |
| `enable_bg_gradient` | `checkbox` | `false` | Enable gradient background |
| `bg_gradient` | `color_background` | *Warm cream gradient* | Custom gradient CSS |
| `container_max_width` | `range` | `1360px` | Maximum width of section container |
| `enable_ambient_glow` | `checkbox` | `true` | Soft radial ambient light behind center image |
| `ambient_glow_color` | `color` | `#FFE4BA` | Glow light color |
| `ambient_glow_opacity` | `range` | `55%` | Glow opacity |

### 📝 Section Header

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `show_header` | `checkbox` | `true` | Show/hide entire header |
| `eyebrow_text` | `text` | `WHY CHOOSE US` | Tagline / subtitle text |
| `show_eyebrow_icon` | `checkbox` | `true` | Show icon next to eyebrow |
| `custom_eyebrow_icon` | `html` | *Blank* | Optional custom SVG icon |
| `eyebrow_style` | `select` | `plain` | `plain` or `badge` (pill background) |
| `eyebrow_color` | `color` | `#D97736` | Eyebrow text & icon color |
| `eyebrow_size_desktop` | `range` | `13px` | Eyebrow font size on desktop |
| `eyebrow_size_mobile` | `range` | `12px` | Eyebrow font size on mobile |
| `heading` | `inline_richtext` | `BECAUSE YOUR PET DESERVES THE BEST` | Main section heading |
| `heading_tag` | `select` | `h2` | HTML semantic tag (`h1`, `h2`, `h3`, `p`) |
| `heading_color` | `color` | `#1E1E1E` | Heading text color |
| `heading_size_desktop` | `range` | `36px` | Heading font size on desktop |
| `heading_size_mobile` | `range` | `26px` | Heading font size on mobile |
| `heading_weight` | `select` | `800` | Font weight (600, 700, 800, 900) |
| `header_align` | `select` | `center` | Text alignment (`left`, `center`, `right`) |

### 🖼️ Center Featured Image

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `center_image` | `image_picker` | *None* | Featured pet/product image |
| `fallback_image_url` | `url` | *None* | External image URL fallback |
| `image_width_desktop` | `range` | `420px` | Maximum width of image on desktop |
| `image_width_mobile` | `range` | `280px` | Maximum width of image on mobile |
| `image_max_height_desktop` | `range` | `520px` | Max height on desktop |
| `image_max_height_mobile` | `range` | `320px` | Max height on mobile |
| `image_object_fit` | `select` | `contain` | `contain` or `cover` |
| `image_radius` | `range` | `0px` | Image corner radius |
| `enable_pedestal_shadow` | `checkbox` | `true` | Soft ground shadow under subject |
| `enable_floating_animation` | `checkbox` | `false` | Gentle floating breathing animation |

### 📐 Column & Item Layout

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `vertical_alignment` | `select` | `center` | Desktop column alignment (`center`, `start`, `space-between`) |
| `left_col_align` | `select` | `center` | Left column text alignment (`right`, `center`, `left`) |
| `right_col_align` | `select` | `center` | Right column text alignment (`left`, `center`, `right`) |
| `column_gap_desktop` | `range` | `50px` | Horizontal space between columns |
| `item_gap_desktop` | `range` | `45px` | Vertical space between feature cards (Desktop) |
| `item_gap_mobile` | `range` | `25px` | Vertical space between feature cards (Mobile) |
| `item_max_width` | `range` | `280px` | Maximum width of each feature item |

### ✨ Icons & Feature Typography

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `icon_box_size` / `_mobile` | `range` | `64px` / `56px` | Circular badge container size |
| `icon_inner_size` / `_mobile`| `range` | `32px` / `26px` | Inner icon SVG size |
| `icon_bg_color` | `color` | `#FFFFFF` | Icon circle background |
| `icon_color` | `color` | `#4A5568` | Icon color |
| `icon_border_color` | `color` | `rgba(0,0,0,0.06)` | Icon border color |
| `enable_icon_shadow` | `checkbox` | `true` | Soft shadow under icon |
| `item_title_color` | `color` | `#1E1E1E` | Title color |
| `item_title_size_desktop` / `_mobile` | `range` | `18px` / `16px` | Title font size |
| `item_desc_color` | `color` | `#555555` | Description text color |
| `item_desc_size_desktop` / `_mobile` | `range` | `14px` / `13px` | Description font size |
| `enable_card_hover` | `checkbox` | `true` | Subtle lift animation on hover |

### 📱 Mobile Settings

| Setting ID | Type | Default | Description |
|---|---|---|---|
| `mobile_layout_mode` | `select` | `stacked` | `stacked`, `grid_2_col`, or `slider` |
| `mobile_image_position` | `select` | `middle` | `top` (Image first), `middle`, or `bottom` |
| `mobile_item_align` | `select` | `center` | Text alignment on mobile (`center`, `flex-start`, `flex-end`) |

---

## 📦 Block Settings (`feature_item`)

| Setting ID | Type | Options / Default | Description |
|---|---|---|---|
| `column_position` | `select` | `left`, `right`, `auto` | Choose which side the item displays on |
| `icon_type` | `select` | `preset`, `image`, `custom_svg` | Choose icon source |
| `icon_preset` | `select` | 12 presets available | Select built-in SVG icon |
| `icon_image` | `image_picker` | *None* | Upload custom image icon |
| `custom_svg_code` | `html` | *None* | Raw SVG code snippet |
| `custom_icon_bg` | `color` | *Optional* | Per-item icon background override |
| `custom_icon_color` | `color` | *Optional* | Per-item icon color override |
| `badge_text` | `text` | *Optional* | Pill tag above title (e.g. `NEW`, `POPULAR`) |
| `title` | `text` | `Feature Title` | Item title |
| `description` | `textarea` | Feature description | Multi-line description text |
| `card_link` | `url` | *Optional* | Clickable link for the entire feature card |

---

## 🎯 Out-of-the-box Preset

The section comes pre-configured with default content matching the original design:

1. **Left Column**:
   - 🛰️ **Smart Feeding Tech**: Automatic feeders with camera & voice control — feed your pet anytime, anywhere.
   - 🦮 **Safe & Stylish Walks**: LED retractable leashes and breathable harnesses for safe, comfortable outdoor adventures.
   - ✂️ **Expert Grooming Tools**: Self-cleaning brushes and steam grooming tools for a clean, healthy coat every day.
2. **Right Column**:
   - 🎒 **Travel Ready**: Bubble carrier backpacks and GPS trackers to keep your pet safe on every journey.
   - 🥣 **Healthy Food**: Premium, nutritionally balanced meals with natural ingredients — keeping your pet healthy and happy.
   - 🚚 **Free Shipping**: Enjoy free delivery on all orders. Fast, reliable shipping straight to your door — no minimum order required.

---

## 💡 Best Practices & Tips

- **Transparent PNG / WebP Cutout**: For the center image, use a cutout image with a transparent background (such as a pet or product isolated on transparent background) for a clean look with the warm cream background.
- **Alignment Match**: On desktop, setting `left_col_align` to `center` or `right` and `right_col_align` to `center` or `left` creates balanced visual harmony framing the center subject.
- **Theme Color Pairing**: You can change `bg_color` and `eyebrow_color` to match any brand color scheme effortlessly.

# How It Works - Process Steps

A high-converting, modern **Step-by-Step "How It Works" / Process Guide** section for Shopify Online Store 2.0 themes. Tailored specifically for custom merchandise, DTC brands, made-to-order collections, personalized apparel, and services.

Designed with bold athletic italic typography, customizable circular number badges, responsive grid layouts, a touch-friendly mobile swipeable slider, high-fidelity built-in fallback illustrations, and an estimated delivery subtext note.

![How It Works Steps Preview](preview.png)

---

## ✨ Features

- **Bold Athletic Design System**:
  - High-impact italicized uppercase headlines and eyebrow tracking labels.
  - Matches DTC athletic brands, custom merchandise shops, and modern apparel stores.
- **Top Header with Flexible Navigation**:
  - Eyebrow text (`HOW IT WORKS`).
  - Athletic headline (`FROM YOUR LOGO TO YOUR DOOR IN FOUR STEPS`).
  - Supporting description copy.
  - Optional header link (`SEE THE FULL PROCESS →`) with smooth hover arrow animation.
- **Flexible 4-Step Card Grid**:
  - Desktop: Configurable 2 to 4 equal columns (defaults to 4 columns matching the reference layout).
  - Tablet: Automatic 2-column layout.
  - Mobile: Select between a clean **Vertical Stack** or a smooth, touch-friendly **Swipeable Slider** with peek preview and interactive pagination dots.
- **Floating Step Number Badges**:
  - Circular badges (`01`, `02`, `03`, `04`) positioned over each step image.
  - Auto-increments (`01`, `02`, etc.) if left blank, or allows custom overrides.
  - Fully customizable badge background, text color, size, and font size.
- **Studio-Quality Fallback Vector Illustrations**:
  - Built-in, high-fidelity SVG artwork for all 4 default steps:
    1. **Choose your sweatband**: Studio presentation of terry wristbands with knitted cloth texture and embroidered logos.
    2. **Upload your logo**: Designer desk with laptop canvas displaying vector artwork and digital proof sheets.
    3. **We print and produce it**: Workshop conveyor with industrial screen-printing press squeegee.
    4. **Delivered to your door**: Open kraft delivery parcel packed neatly with rolled colorful sweatbands.
  - Never leaves an ugly empty placeholder when product photography is still in progress!
- **Interactive Card Animations**:
  - Smooth hover zoom on step imagery and optional card hover lift elevation.
- **Footer Delivery & Policy Note**:
  - Centered subtext under the cards (e.g. `Estimated delivery: 4 to 5 weeks from proof approval · Minimum order 25 pieces`).
  - Customizable colors, background pill, and font sizes.
- **Zero Heavy Dependencies**:
  - Pure semantic HTML5, scoped CSS variables, and lightweight Vanilla JavaScript. No external libraries, jQuery, or framework dependencies required.

---

## 🚀 How to Install & Use

1. Copy [`how-it-works-steps.liquid`](how-it-works-steps.liquid) into your Shopify theme's `sections/` directory.
2. In your Shopify Admin, navigate to **Online Store > Themes > Customize**.
3. Go to any page template (Homepage, Product page, Landing page, Collection page, etc.).
4. Click **Add section** and choose **How It Works Steps**.
5. Customize the heading, cards, images, colors, and badge styling to match your brand.
6. Click **Save**.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_header` | `checkbox` | `true` | Toggle display of the section header |
| `eyebrow` | `text` | `HOW IT WORKS` | Eyebrow label text above the heading |
| `eyebrow_color` | `color` | `#0284c7` | Eyebrow text color |
| `eyebrow_size` | `range` | `13px` | Eyebrow font size (`10px` to `20px`) |
| `heading` | `text` | `FROM YOUR LOGO TO YOUR DOOR IN FOUR STEPS` | Main section headline |
| `heading_tag` | `select` | `h2` | HTML heading tag (`h1`, `h2`, `h3`, `div`) |
| `heading_italic` | `checkbox` | `true` | Apply athletic italic styling to headline |
| `heading_color` | `color` | `#0b1320` | Headline text color |
| `heading_size_desktop` | `range` | `42px` | Desktop heading font size (`24px` to `64px`) |
| `heading_size_mobile` | `range` | `28px` | Mobile heading font size (`20px` to `40px`) |
| `description` | `textarea` | *(copy)* | Supporting description copy |
| `description_color` | `color` | `#64748b` | Description text color |
| `description_size` | `range` | `16px` | Description font size (`13px` to `22px`) |
| `show_header_link` | `checkbox` | `true` | Toggle "See the full process" header link |
| `header_link_text` | `text` | `SEE THE FULL PROCESS` | Header link text |
| `header_link_url` | `url` | — | Destination URL for the header link |
| `header_link_color` | `color` | `#0284c7` | Header link color |
| `container_max_width` | `range` | `1280px` | Maximum container width (`900px` to `1600px`) |
| `columns_desktop` | `range` | `4` | Number of columns on desktop (`2` to `4`) |
| `mobile_layout` | `select` | `stacked` | Mobile layout style (`Vertical Stack` or `Touch Swipeable Slider`) |
| `card_gap_desktop` | `range` | `24px` | Space between cards on desktop (`16px` to `48px`) |
| `card_gap_mobile` | `range` | `16px` | Space between cards on mobile (`12px` to `32px`) |
| `section_bg` | `color` | `#ffffff` | Background color for the section |
| `card_bg` | `color` | `transparent` | Background color for each card |
| `accent_color` | `color` | `#0284c7` | Global accent color for links, badges, and indicators |
| `image_aspect_ratio` | `select` | `4/3` | Image aspect ratio (`4/3`, `1/1`, `16/9`, `3/2`, `auto`) |
| `image_border_radius` | `range` | `20px` | Corner radius for card images (`4px` to `36px`) |
| `enable_image_zoom` | `checkbox` | `true` | Subtle zoom effect on card hover |
| `card_hover_lift` | `checkbox` | `false` | Subtle card elevation lift on hover |
| `show_step_badge` | `checkbox` | `true` | Toggle floating step number badges |
| `badge_bg_color` | `color` | `#0284c7` | Number badge background circle color |
| `badge_text_color` | `color` | `#ffffff` | Number badge text color |
| `badge_size` | `range` | `34px` | Badge circle diameter (`26px` to `48px`) |
| `badge_font_size` | `range` | `13px` | Badge number font size (`10px` to `20px`) |
| `step_title_color` | `color` | `#0b1320` | Step title text color |
| `step_title_size_desktop` | `range` | `19px` | Step title desktop font size (`15px` to `26px`) |
| `step_title_size_mobile` | `range` | `17px` | Step title mobile font size (`14px` to `22px`) |
| `step_title_italic` | `checkbox` | `true` | Italicize step titles |
| `text_muted_color` | `color` | `#64748b` | Step description copy color |
| `step_desc_size` | `range` | `14px` | Step description font size (`12px` to `18px`) |
| `show_footer_note` | `checkbox` | `true` | Toggle bottom delivery note |
| `footer_note_text` | `text` | *(note)* | Bottom delivery and order requirement note |
| `footer_note_color` | `color` | `#64748b` | Footer note text color |
| `footer_note_size` | `range` | `13px` | Footer note font size (`11px` to `18px`) |
| `footer_note_bg` | `color` | `transparent` | Optional background pill color for footer note |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `64px` | Vertical section padding on desktop |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `40px` | Vertical section padding on mobile |

---

### Block Settings (`step`)

Each step block represents a milestone in the order process:

| Setting | Type | Default | Description |
|---|---|---|---|
| `step_number` | `text` | — | Step number override (e.g. `01`). Leave empty to auto-number |
| `image` | `image_picker` | — | Custom step photography upload |
| `fallback_art_type` | `select` | `sweatband` | Fallback vector style if no image is uploaded (`Choose Sweatband`, `Upload Logo`, `Screen Printing`, `Delivery Box`) |
| `title` | `text` | `Choose your sweatband` | Step title |
| `title_tag` | `select` | `h3` | HTML heading tag (`h3`, `h4`, `h5`, `div`) |
| `description` | `textarea` | *(copy)* | Detailed instructions and expectations for this step |
| `step_link` | `url` | — | Optional URL destination if step is clickable |
| `link_text` | `text` | — | Optional call-to-action link text (e.g. `Learn more →`) |

---

## 📱 Mobile Layout Modes

This section includes two distinct mobile experiences:

1. **Vertical Stack (`stacked`)**:
   - Displays steps cleanly in a single vertical column.
   - Ideal for short, concise step descriptions and effortless one-thumb scrolling.

2. **Touch Swipeable Slider (`slider`)**:
   - Enables a horizontal touch carousel with native CSS scroll-snap.
   - Includes peek preview of upcoming cards (`flex: 0 0 82%`).
   - Automatically renders interactive pagination dots at the bottom with real-time active state synchronization.

---

## 🎨 Presets

The section comes pre-configured with the complete 4-step custom merchandise order workflow out of the box:

- **Step 01**: `Choose your sweatband`
- **Step 02**: `Upload your logo`
- **Step 03**: `We print and produce it`
- **Step 04**: `Delivered to your door`
- **Footer**: `Estimated delivery: 4 to 5 weeks from proof approval · Minimum order 25 pieces`

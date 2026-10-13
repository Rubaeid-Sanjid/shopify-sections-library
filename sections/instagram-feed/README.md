# Instagram Feed & Slider Showcase

A modern, highly customizable responsive Instagram Feed and Showcase section for Shopify Online Store 2.0 themes. Built with an editorial urban DTC aesthetic, featuring smooth hover interactions with a centered Instagram icon micro-animation, optional direct links, and a touch-friendly carousel/slider mode.

![Instagram Feed Preview](preview.png)

---

## ✨ Features

- **Responsive Grid & Slider Modes**:
  - **All Devices Slider**: Smooth horizontal touch-swipe and drag carousel on both desktop and mobile.
  - **Mobile Only Slider**: High-density grid on desktop (e.g. 5 columns), automatically converts to a swipeable carousel on mobile.
  - **Static Grid**: Pure CSS responsive grid layout.
- **Center Instagram Icon Hover Micro-animation**:
  - Smooth spring-scale entrance animation (`cubic-bezier(0.34, 1.56, 0.64, 1)`) with customizable frosted glass or solid badge styling.
  - Subtle dark overlay fade and image zoom effect on hover.
  - Optional username/tag preview (e.g. `@redlaneclub`).
- **Flexible Image & Card Dimensions**:
  - Customizable aspect ratios: **Square (1:1)**, **Portrait (4:5)**, **Story/Tall (9:16)**, or **Landscape (16:9)**.
  - Configurable card corner border radius (0–32px).
- **Interactive Navigation & Controls**:
  - Multiple arrow positions: **Header Right** (aligned beside title), **Side Floating**, or **Bottom Center**.
  - Pagination dots with active progress indicator.
  - Optional smooth **Autoplay** with auto-pause on mouse hover and touch.
- **Clickable Posts / Links**:
  - Link any card directly to an Instagram post, Instagram profile, or Shopify product page.
  - Option to open links in a new tab (`target="_blank" rel="noopener noreferrer"`).
- **Dual Image Source Support**:
  - Native Shopify `image_picker` upload support.
  - Direct external URL fallback field for quick staging, CDN hosting, or mockups.
- **Zero External Dependencies**:
  - 100% vanilla CSS & lightweight vanilla JavaScript. No Slick, Swiper, jQuery, or third-party libraries needed.
  - Uses native CSS scroll-snap for ultra-smooth 60fps/120fps mobile swiping.
  - Scoped CSS variables and unique IDs prevent styling conflicts with any theme.

---

## 🚀 How to Use

1. Copy [`instagram-feed.liquid`](instagram-feed.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify Admin, navigate to **Online Store → Themes → Customize**.
3. In any template (Home page, Product page, About page, etc.), click **Add section**.
4. Search for and select **Instagram Feed**.
5. Customize your heading, subheading, colors, columns, and add or rearrange Instagram post blocks.

---

## ⚙️ Schema Settings

### Header Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_header` | checkbox | `true` | Show or hide the section header |
| `eyebrow` | text | `""` | Eyebrow tag above heading (e.g. `INSTAGRAM`) |
| `show_eyebrow_icon` | checkbox | `false` | Displays a mini Instagram glyph in the eyebrow |
| `eyebrow_size` | range | `13px` | Eyebrow font size |
| `eyebrow_color` | color | `#767676` | Eyebrow text color |
| `heading` | text | `"FOLLOW THE ROUTE"` | Main headline text |
| `heading_size_desktop` | range | `36px` | Headline size on desktop |
| `heading_size_mobile` | range | `24px` | Headline size on mobile |
| `heading_weight` | select | `"700"` | Font weight (Regular to Extra Bold) |
| `heading_transform` | select | `"uppercase"` | Text case (None, Uppercase, Capitalize) |
| `heading_color` | color | `#111111` | Headline color |
| `subheading` | richtext | `"Tag us @redlaneclub to be featured"` | Subheading / social handle description with HTML link support |
| `subheading_size` | range | `15px` | Subheading font size |
| `subheading_color` | color | `#333333` | Subheading text color |
| `header_alignment` | select | `"left"` | Content alignment (`left`, `center`, `right`) |
| `header_margin_bottom` | range | `28px` | Space between header and image cards |

### Layout & Sizing

| Setting | Type | Default | Description |
|---|---|---|---|
| `full_width` | checkbox | `false` | Expand section edge-to-edge |
| `container_max_width` | range | `1400px` | Maximum content width if not full-width |
| `section_bg` | color | `#ffffff` | Background color of section |
| `gap_desktop` | range | `16px` | Gap between cards on desktop |
| `gap_mobile` | range | `12px` | Gap between cards on mobile |
| `columns_desktop` | range | `5` | Visible cards per row on desktop (2–6) |
| `columns_tablet` | range | `3` | Visible cards per row on tablet (2–4) |
| `columns_mobile` | select | `"2"` | Columns on mobile when in static grid mode |
| `columns_mobile_slider`| select | `"1.3"` | Visible slides on mobile in slider mode (allows peeking next card) |

### Slider / Carousel Controls

| Setting | Type | Default | Description |
|---|---|---|---|
| `slider_mode` | select | `"all"` | Mode: `all` (desktop & mobile), `mobile_only`, `desktop_only`, or `none` |
| `enable_autoplay` | checkbox | `false` | Automatically advance slides |
| `autoplay_speed` | range | `4s` | Slide change duration in seconds |
| `show_arrows` | checkbox | `true` | Show prev/next navigation arrow buttons |
| `arrow_position` | select | `"header"` | Arrow placement: `header`, `sides`, or `bottom` |
| `arrow_size` | range | `42px` | Diameter/size of arrow buttons |
| `arrow_bg_color` | color | `#ffffff` | Arrow button background color |
| `arrow_color` | color | `#111111` | Arrow chevron icon color |
| `arrow_hover_bg` | color | `#111111` | Arrow button hover background |
| `arrow_hover_color` | color | `#ffffff` | Arrow chevron hover color |
| `show_dots` | checkbox | `false` | Display pagination indicator dots |
| `dot_color` | color | `#dddddd` | Inactive dot color |
| `dot_active_color` | color | `#111111` | Active dot color |

### Card Styling & Hover Effects

| Setting | Type | Default | Description |
|---|---|---|---|
| `aspect_ratio` | select | `"square"` | `square` (1:1), `portrait` (4:5), `tall` (9:16), or `landscape` (16:9) |
| `card_border_radius` | range | `14px` | Rounded corner radius for images |
| `enable_hover_zoom` | checkbox | `true` | Subtle scale zoom on card hover |
| `zoom_scale` | select | `"1.08"` | Scale magnitude on hover (`1.04`, `1.08`, `1.12`) |
| `overlay_color` | color | `#000000` | Backdrop color on hover |
| `overlay_opacity` | range | `35%` | Overlay opacity on hover (0–90%) |
| `show_center_instagram_icon` | checkbox | `true` | Show center Instagram icon on hover |
| `icon_size` | range | `28px` | Center Instagram glyph size |
| `icon_color` | color | `#ffffff` | Center Instagram glyph color |
| `icon_bg_style` | select | `"circle_glass"` | `circle_glass`, `circle_solid`, `square_rounded`, or `none` |
| `icon_bg_color` | color | `rgba(255, 255, 255, 0.2)` | Background badge tint behind icon |
| `open_in_new_tab` | checkbox | `true` | Open post links in a new browser tab |

---

## 🧩 Block Settings (`instagram_post`)

Each image card is added as a block:

| Setting | Type | Description |
|---|---|---|
| `image` | `image_picker` | Primary Shopify image file |
| `image_url` | `text` | External image URL fallback (useful for testing or CDN assets) |
| `link` | `url` | Destination URL (Instagram post, profile, or product link) |
| `caption` | `text` | Accessible alt text & image description |
| `username` | `text` | Optional hover handle tag (e.g. `@redlaneclub`) |

---

## 💡 Pro Tips

- **Connecting to Instagram**: Simply copy the share link of your top performing Instagram posts (e.g. `https://www.instagram.com/p/xxxxxx/`) into the block's `link` field.
- **Peek-Next Mobile Slider**: Setting `columns_mobile_slider` to `1.3` gives users a visual affordance that the list is swipeable by showing the edge of the next photo.
- **Custom Fonts**: The section inherits your theme's body and heading typography rules seamlessly while providing independent weight and letter-spacing sliders.

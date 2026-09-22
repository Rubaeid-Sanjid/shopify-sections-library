# Community Stats / Counter

An engaging, animated **Community Statistics Counter** section for Shopify Online Store 2.0 themes. Designed to showcase social proof, subscriber counts, total community members, or happy customer milestones with smooth rolling number animations and optional CTA.

Built with semantic Shopify Liquid, performant Vanilla JS (utilizing `IntersectionObserver` and cubic ease-out `requestAnimationFrame`), and pure CSS with zero external library dependencies.

![Community Stats Preview](Community_count_section.png)

---

## ✨ Features

- **Animated Number Counter**: Numbers smoothly roll up from `0` to the target value when the section scrolls into view using `IntersectionObserver` with a buttery smooth cubic ease-out curve (`1 - (1 - p)^3`).
- **Automatic Number Formatting**: Formats large numbers with localized thousand separators (e.g. `1,000,000`) via native `Intl.NumberFormat`.
- **3 Configurable Milestone Stats**: Set individual values, custom suffixes (such as `+`, `k`, `M`, `%`), and descriptive labels for each stat item.
- **Header & Editorial Copy**: Centered headline and rich text description with customizable widths and font sizing.
- **Optional CTA Button**: Link to community channels, Discord, YouTube, or product collections with customizable background, text color, padding, and corner radius.
- **Granular Responsive Controls**:
  - Independent desktop and mobile padding (top and bottom).
  - 1-column or 2-column mobile grid toggle.
  - Independent font size controls for headings, body descriptions, numbers, and labels.
  - Adjustable column gaps and vertical spacing.
- **Encapsulated Custom Element**: Scoped via `<community-stats-{{ section_id }}>` to prevent CSS/JS pollution across themes.
- **Zero Dependencies**: Lightweight and fast, no external libraries (no jQuery, no CountUp.js).

---

## 🚀 How to Use

1. Copy [`custom_community_count.liquid`](custom_community_count.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify theme customizer, navigate to any page template (Homepage, About page, Landing page, etc.).
3. Click **Add section** and search for **Community stats**.
4. Configure your statistics numbers, suffixes, labels, colors, and optional community button.

---

## ⚙️ Schema Settings

### Content & Numbers

| Setting | Type | Default | Description |
|---|---|---|---|
| `heading` | `text` | `Backed by a Community of Millions` | Main section heading |
| `description` | `richtext` | *Rich text copy* | Descriptive body text below the heading |
| `stat_1_count` | `text` | `1000000` | Target number for Stat 1 (raw integer) |
| `stat_1_suffix` | `text` | `+` | Suffix for Stat 1 (e.g., `+`, `k`, `M`, `%`) |
| `stat_1_label` | `text` | `YouTube Subscribers` | Label description for Stat 1 |
| `stat_2_count` | `text` | `300000` | Target number for Stat 2 |
| `stat_2_suffix` | `text` | `+` | Suffix for Stat 2 |
| `stat_2_label` | `text` | `Community Members` | Label description for Stat 2 |
| `stat_3_count` | `text` | `100000` | Target number for Stat 3 |
| `stat_3_suffix` | `text` | `+` | Suffix for Stat 3 |
| `stat_3_label` | `text` | `Happy Customers` | Label description for Stat 3 |
| `button_label` | `text` | `Join the community` | Optional CTA button label |
| `button_link` | `url` | *empty* | Optional CTA button link |

### Layout & Spacing

| Setting | Type | Default | Description |
|---|---|---|---|
| `desktop_width` | `range` | `100%` | Inner content width percentage on desktop (50% to 100%) |
| `max_width` | `range` | `1200px` | Maximum content width in pixels (800px to 2000px) |
| `desktop_top` / `_bottom` | `range` | `90px` / `90px` | Section top and bottom padding on desktop |
| `mobile_top` / `_bottom` | `range` | `60px` / `60px` | Section top and bottom padding on mobile |
| `mobile_columns` | `select` | `1` | Mobile grid layout: `1` or `2` columns |
| `gap` | `range` | `25px` | Spacing gap between stats columns on desktop |
| `mobile_gap` | `range` | `35px` | Spacing gap between stats columns on mobile |
| `stats_top` / `_bottom` | `range` | `60px` / `50px` | Top and bottom spacing around the stats grid |
| `heading_gap` | `range` | `20px` | Spacing gap below the main heading |
| `body_width` | `range` | `700px` | Maximum width of the description text |

### Typography

| Setting | Type | Default | Description |
|---|---|---|---|
| `heading_size` / `mobile_heading_size` | `range` | `52px` / `32px` | Responsive font sizes for the main heading |
| `body_size` / `mobile_body_size` | `range` | `17px` / `16px` | Responsive font sizes for description copy |
| `number_size` / `mobile_number_size` | `range` | `70px` / `44px` | Responsive font sizes for statistic numbers |
| `label_size` / `mobile_label_size` | `range` | `15px` / `14px` | Responsive font sizes for statistic labels |
| `button_size` | `range` | `14px` | Button text font size |
| `button_v` / `button_h` | `range` | `14px` / `30px` | Vertical and horizontal button padding |
| `button_radius` | `range` | `0px` | Corner border-radius for button |

### Colors

| Setting | Type | Default | Description |
|---|---|---|---|
| `bg` | `color` | `#0D0D0D` | Section background color |
| `text` | `color` | `#FFFFFF` | Default text color |
| `heading_color` | `color` | `#FFFFFF` | Heading text color |
| `subtext` | `color` | `#D6D6D6` | Description text color |
| `number_color` | `color` | `#FFFFFF` | Statistic numbers color |
| `label_color` | `color` | `#BDBDBD` | Statistic labels color |
| `button_bg` | `color` | `#E44E03` | CTA button background color |
| `button_text` | `color` | `#FFFFFF` | CTA button text color |

---

## 💻 Tech & Compatibility

- **Shopify Compatibility**: Online Store 2.0 (OS 2.0)
- **Zero Dependencies**: Pure HTML5, Vanilla JavaScript (`IntersectionObserver`), and CSS
- **Performance**: Runs animation only when visible in the viewport and automatically disconnects the observer
- **License**: MIT

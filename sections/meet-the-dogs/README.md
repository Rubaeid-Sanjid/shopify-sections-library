# Meet the Dogs Behind Petrix

A premium, compact storytelling section designed for Shopify themes (e.g. Petrix) to introduce the real dogs and personalities behind the brand. Displays matching cards in a responsive grid layout with portrait photography, badges (Breed & Age), and personality bio copy.

## Features

- **Dynamic Header**: Tagline with glowing dot, main heading (with gradient highlight word effect), and customizable subtitle.
- **3-Card Matching Grid**: Obsidian glassmorphic cards with rim glow effect on hover, smooth image zoom, and subtle gradient vignette.
- **Block-based Architecture**: Add, reorder, or edit dogs via Shopify blocks (`dog_card`).
- **Structured Metadata**: Dedicated fields for Dog Name, Breed, Age, and Personality Description.
- **Image Flexibility**: Supports Shopify Theme Image Picker + direct External Image URL fallback.
- **Bottom CTA Action**: Optional pill button ("Meet the Dogs →") linking to the About Us page.
- **Complete Schema Customization**: Full control over background colors, glowing radial ambient lights, card backgrounds, borders, typography sizes (desktop and mobile), aspect ratios, and padding.
- **Pure CSS / Vanilla Liquid**: Lightweight, zero external JS dependencies, fully mobile-responsive.

## How to Use

1. Copy `meet_the_dogs.liquid` into your Shopify theme's `sections/` directory.
2. In the Shopify Theme Customizer, click **Add section** and select **Meet the Dogs**.
3. Place it near the bottom of the homepage (e.g., between "Built to Keep Evolving" and the Preorder section).
4. Customize the content, dog photos, breed/age badges, and CTA button.

## Schema Settings

| Setting Group | Key Settings | Description |
|---|---|---|
| **Header Text** | `tagline`, `heading`, `heading_highlight`, `subtitle`, `heading_align` | Header titles, gradient highlight, and alignment |
| **Colors & Gradients** | `bg_color`, `gradient_start`, `gradient_end`, `card_bg`, `card_border`, `dog_name_color`, `dog_meta_color`, `dog_bio_color` | Color palette and glassmorphism styling |
| **Ambient Glow** | `enable_glow`, `glow_opacity`, `glow_size`, `glow_blur`, `glow_pos_x`, `glow_pos_y` | Background glow orb effect |
| **Card Style** | `card_radius`, `img_aspect_ratio`, `enable_card_glow`, `card_glow_color` | Card geometry and hover effects |
| **Bottom Button** | `show_button`, `button_text`, `button_link`, `btn_margin_top` | CTA button linking to About page |
| **Layout** | `container_max_width`, `cols_desktop`, `cols_mobile`, `grid_gap`, padding settings | Responsive grid sizing |

## Preset Content

Includes default block settings for:
1. **WILLIE** (French Bulldog • Age 3)
2. **POPPY** (Cockapoo • Age 4)
3. **PRINCE** (Miniature Dachshund • 5 Months)

# Featured Product

A modern, high-converting **Featured Product Section** for Shopify Online Store 2.0 themes. Designed with a clean, minimalist DTC streetwear aesthetic (inspired by premium apparel brands like *Beyond Myth*, *Fear of God Essentials*, and *Represent*).

Features a multi-angle vertical thumbnail rail, a generous rounded product hero card (`border-radius: 24px`), dynamic price display, 5-star social proof reviews, pill button variant swatches (Size S / M / L / XL), an accessible quantity stepper, a full-width high-converting Add-to-Cart CTA with AJAX cart drawer dispatch, and customizable trust badges.

![Featured Product Preview](preview.png)

---

## ✨ Features

- **Split 2-Column DTC Layout**: Optimal visual balance with an interactive media gallery on the left and a streamlined purchase form on the right.
- **Vertical Thumbnail Rail**:
  - Desktop vertical thumbnail strip on the left with prominent active border indicators (`2px solid #111111`).
  - Smooth slide switching with fade transitions and hover states.
  - Automatically switches to a touch-friendly horizontal swipe strip on mobile screens.
- **Hero Media Card**:
  - Subtle neutral background (`#f0f0f2`) that makes product silhouettes and colors pop.
  - Generous modern rounded corners (`border-radius: 24px`).
  - Smooth hover zoom interaction (`transform: scale(1.05)`).
- **Product Information Hierarchy**:
  - **Vendor / Eyebrow**: Uppercase tracking label (`BEYOND MYTH`).
  - **Product Headline**: Bold, modern typography (`The Essential Tee`).
  - **Price & Compare Price**: High-visibility price formatting with strikethrough discount support.
  - **Star Rating & Social Proof**: 5 golden stars with review score and count (`4.8 (120 reviews)`).
  - **Editorial Description**: Clean typography for product narrative and fabric details.
- **Interactive Option Swatches (Size Pills)**:
  - Accessible button swatches for sizes (`S`, `M`, `L`, `XL`) or any product option.
  - Full variant mapping: clicking a size updates the master variant ID, live price, compare-at price, inventory availability, and switches to the variant's featured photo.
  - Sold-out state handling: automatically disables button and displays "Sold Out" if variant is out of stock.
- **Quantity Stepper Box**:
  - Clean boxed stepper (`−`, numeric input, `+`) with boundary checks (minimum 1).
- **High-Converting Add to Cart CTA**:
  - Solid high-contrast button with smooth hover lift and loading state.
  - Native AJAX submission to `/cart/add.js`.
  - Dispatches standard Shopify events (`cart:updated`, `cart:refresh`) to automatically open cart drawers and slide-outs on themes like Dawn, Impulse, Prestige, Warehouse, etc.
  - Dynamic checkout button support (`{{ form | payment_button }}`).
- **3 Built-in Trust Badges**:
  - 🚚 **Free Shipping** `(US Orders)`
  - 🔄 **30-Day Returns**
  - 🛡️ **Secure Checkout**
  - Fully customizable icons (Truck, Return Arrow, Shield) and copy in the theme customizer.
- **100% Self-Contained & Zero Dependencies**:
  - Pure Shopify Liquid, modern scoped CSS variables, and Vanilla JavaScript.
  - No snippet dependencies or external libraries.
  - Includes built-in high-fidelity vector artwork so the section renders a ready-to-use demo even before a product is selected in the theme editor!

---

## 🚀 How to Use

1. Copy [`featured-product.liquid`](featured-product.liquid) into your Shopify theme's `sections/` directory via the Shopify Code Editor or Shopify CLI.
2. In the Shopify theme customizer, navigate to any page template (Homepage, Product Landing Page, Campaign page, etc.).
3. Click **Add section** and select **Featured Product**.
4. In the section settings sidebar, select your desired **Product** from your Shopify catalog.
5. *(Optional)* If you wish to use custom marketing headlines or launch a promotional teaser, toggle **Override Product Content** or upload custom gallery photos.

---

## ⚙️ Schema Settings

### Product Selection & Content Overrides

| Setting | Type | Default | Description |
|---|---|---|---|
| `product` | `product` | — | Select the product to feature. Leave blank to display the built-in demo |
| `override_content` | `checkbox` | `false` | When enabled, overrides product title/price/description with the custom copy below |
| `vendor` | `text` | `BEYOND MYTH` | Eyebrow brand or vendor name |
| `title` | `text` | `The Essential Tee` | Main product headline |
| `price` | `text` | `$38.00` | Custom price display |
| `compare_at_price` | `text` | — | Optional original strikethrough price |
| `description` | `textarea` | *(copy)* | Editorial product description copy |

---

### Reviews & Social Proof

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_rating` | `checkbox` | `true` | Toggle display of star rating row |
| `rating_text` | `text` | `4.8 (120 reviews)` | Rating score and review count copy |
| `star_color` | `color` | `#f59e0b` | Fill color for the 5 rating stars |

---

### Media & Gallery Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `media_bg_color` | `color` | `#f0f0f2` | Background color for the hero product card |
| `media_border_radius` | `range` | `24px` | Corner radius for the main product card (`0px` to `40px`) |
| `thumbnail_position_desktop` | `select` | `left` | Desktop thumbnail rail position (`Left (Vertical)` or `Bottom (Horizontal)`) |
| `thumbnail_border_radius` | `range` | `6px` | Corner radius for thumbnail buttons (`0px` to `16px`) |
| `enable_image_zoom` | `checkbox` | `true` | Micro-scale zoom effect on desktop hover |
| `custom_image_1` - `5` | `image_picker` | — | Optional custom image overrides for the 5 gallery slides |

---

### Variant & Form Controls

| Setting | Type | Default | Description |
|---|---|---|---|
| `size_option_name` | `text` | `Size` | Label for the swatch options (demo mode) |
| `custom_sizes` | `text` | `S, M, L, XL` | Comma-separated sizes shown when no product is linked |
| `show_quantity_selector` | `checkbox` | `true` | Toggle numeric stepper box |
| `button_text` | `text` | `Add to Cart` | Call-to-action button text |
| `button_bg_color` | `color` | `#111111` | Primary CTA background color |
| `button_text_color` | `color` | `#ffffff` | Primary CTA text color |
| `button_hover_bg_color` | `color` | `#262626` | Primary CTA hover background color |
| `button_border_radius` | `range` | `8px` | CTA button corner radius (`0px` to `20px`) |
| `show_dynamic_checkout` | `checkbox` | `false` | Enable Shopify Dynamic Checkout (Apple Pay, Google Pay, PayPal) |

---

### Trust Badges & Value Props

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_trust_badges` | `checkbox` | `true` | Toggle display of trust badges row |
| `badge_1_icon` | `select` | `truck` | SVG icon for badge 1 (`truck`, `return`, `shield`) |
| `badge_1_title` | `text` | `Free Shipping` | Title for badge 1 |
| `badge_1_subtitle` | `text` | `(US Orders)` | Optional subtitle for badge 1 |
| `badge_2_icon` | `select` | `return` | SVG icon for badge 2 (`truck`, `return`, `shield`) |
| `badge_2_title` | `text` | `30-Day Returns` | Title for badge 2 |
| `badge_2_subtitle` | `text` | — | Optional subtitle for badge 2 |
| `badge_3_icon` | `select` | `shield` | SVG icon for badge 3 (`truck`, `return`, `shield`) |
| `badge_3_title` | `text` | `Secure Checkout` | Title for badge 3 |
| `badge_3_subtitle` | `text` | — | Optional subtitle for badge 3 |

---

### Section Layout & Spacing

| Setting | Type | Default | Description |
|---|---|---|---|
| `section_bg` | `color` | `#ffffff` | Overall section background color |
| `container_max_width` | `range` | `1200px` | Maximum content width (`900px` to `1440px`) |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `64px` | Desktop vertical padding |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `36px` | Mobile vertical padding |

---

## 🎨 Presets Included

The section includes a ready-to-use preset replicating the reference showcase:

- **Vendor**: `BEYOND MYTH`
- **Product Title**: `The Essential Tee`
- **Price**: `$38.00`
- **Rating**: `★ ★ ★ ★ ★` `4.8 (120 reviews)`
- **Description**: `A premium everyday tee designed for a higher standard. Minimal, versatile, and made to move with you.`
- **Media**: 5 interactive slides (Front Flat Lay, Model Front View, Model Back Graphic, Collar Detail, Fabric Drape)
- **Options**: `S`, `M`, `L`, `XL`
- **Badges**: Free Shipping (US Orders), 30-Day Returns, Secure Checkout

---

## 💡 Best Practices & Customization Tips

- **Transparent PNGs**: For apparel, accessories, or packaged goods, using images with transparent backgrounds allows them to sit cleanly inside the rounded card (`#f0f0f2`).
- **Cart Drawer Compatibility**: The section dispatches both `cart:refresh` and `cart:updated` DOM events upon adding items to the cart. If your theme uses an AJAX side cart (like Dawn or Impulse), the drawer will slide open automatically.
- **Drop-in Flexibility**: Perfect for the Homepage hero, a dedicated landing page for an ad campaign, or as an upsell module on a blog post.

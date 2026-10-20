# FAQ Accordion / Questions & Answers Grid

A clean, modern, high-converting **FAQ Accordion & Questions Grid** section for Shopify Online Store 2.0 themes. Designed specifically for custom merchandise stores, DTC brands, eCommerce product pages, and service providers.

Features an elegant 2-column rounded card grid, smooth CSS grid expand/collapse transitions, rotating chevron indicators, built-in Google FAQPage JSON-LD structured data for search engine rich snippets, accessible ARIA attributes, and complete customization controls.

![FAQ Accordion Preview](preview.png)

---

## ✨ Features

- **2-Column Responsive Grid Layout**:
  - Displays questions side-by-side in a modern 2-column card grid on desktop (or switchable to single-column centered or 3-column layouts).
  - Automatically stacks gracefully into a clean, easy-to-read vertical column on mobile screens.
- **Card-Based UI with Subtle Styling**:
  - Clean white cards with configurable border stroke (`1px` to `4px`), corner radius (`6px` to `32px`), internal padding, and hover elevation shadow.
- **Smooth Accordion Transitions**:
  - Built with modern CSS grid-template transitions (`grid-template-rows: 0fr` to `1fr`) for seamless animation without glitchy height calculations.
  - Rotating chevron arrows (`180deg`) smoothly indicate open and closed states.
- **Flexible Accordion Behaviors**:
  - **Initial State Modes**: Choose between `all_open` (all cards open by default, as shown in the reference design), `all_closed` (clean collapsed view), or `first_open` (only the first card open).
  - **Single or Multi-Open**: Toggle whether opening one card automatically closes other cards (`allow_multiple_open`).
  - **Per-Block Override**: Option on individual questions to stay open by default.
- **Google FAQPage Structured Data (JSON-LD)**:
  - Automatically generates Google-compliant `FAQPage` schema markup.
  - Helps your store qualify for expandable question-and-answer rich snippets directly on Google Search result pages, driving higher organic CTR!
- **Rich Text Answers**:
  - Supports formatted paragraphs, links, bold text, bullet points, and numbered lists in answers.
- **Optional Contact Support Bar**:
  - Built-in bottom call-to-action bar (e.g. *"Still have questions? Our custom branding specialists are here to help"*) with a button link to your contact page.
- **Zero Heavy Dependencies**:
  - Pure semantic HTML5, scoped CSS variables, and lightweight Vanilla JavaScript. No jQuery, Bootstrap, or external libraries required.

---

## 🚀 How to Install & Use

1. Copy [`faq-accordion.liquid`](faq-accordion.liquid) into your Shopify theme's `sections/` directory.
2. In the Shopify Admin, navigate to **Online Store > Themes > Customize**.
3. Choose the page template where you want the FAQ section (Homepage, Product page, FAQ page, Contact page, etc.).
4. Click **Add section** and search for **FAQ Accordion**.
5. Add or reorder your questions and answers in the theme editor.
6. Customize the card colors, typography, borders, and accordion behavior to match your store's branding.
7. Click **Save**.

---

## ⚙️ Schema Settings

### Section Settings

| Setting | Type | Default | Description |
|---|---|---|---|
| `show_header` | `checkbox` | `true` | Toggle display of the section header |
| `header_alignment` | `select` | `left` | Header text alignment (`Left Aligned` or `Centered`) |
| `eyebrow` | `text` | — | Optional tracking label above the heading |
| `eyebrow_color` | `color` | `#0284c7` | Eyebrow text color |
| `heading` | `text` | `Frequently Asked Questions` | Main section heading |
| `heading_tag` | `select` | `h2` | HTML heading tag (`h1`, `h2`, `h3`, `div`) |
| `heading_color` | `color` | `#0b1320` | Section heading color |
| `heading_size_desktop` | `range` | `36px` | Desktop heading font size (`24px` to `56px`) |
| `heading_size_mobile` | `range` | `26px` | Mobile heading font size (`20px` to `36px`) |
| `subheading` | `textarea` | *(copy)* | Supporting subheading copy |
| `subheading_color` | `color` | `#64748b` | Subheading text color |
| `subheading_size` | `range` | `16px` | Subheading font size (`13px` to `20px`) |
| `container_max_width` | `range` | `1280px` | Maximum container width (`800px` to `1600px`) |
| `columns_desktop` | `select` | `2` | Number of columns on desktop (`1`, `2`, `3`) |
| `grid_gap_desktop` | `range` | `20px` | Space between cards on desktop (`12px` to `40px`) |
| `grid_gap_mobile` | `range` | `14px` | Space between cards on mobile (`10px` to `24px`) |
| `section_bg` | `color` | `#ffffff` | Background color of the entire section |
| `card_bg_color` | `color` | `#ffffff` | Background color for each FAQ card |
| `card_border_color` | `color` | `#e2e8f0` | Border stroke color for FAQ cards |
| `card_border_width` | `range` | `1px` | Card border stroke width (`0px` to `4px`) |
| `card_border_radius` | `range` | `16px` | Card corner radius (`6px` to `32px`) |
| `card_padding_desktop` | `range` | `22px` | Internal card padding on desktop (`14px` to `36px`) |
| `card_padding_mobile` | `range` | `18px` | Internal card padding on mobile (`12px` to `28px`) |
| `card_hover_shadow` | `checkbox` | `true` | Subtle elevation shadow on card hover |
| `initial_state` | `select` | `all_open` | Default state on load (`All Items Open`, `All Items Collapsed`, `First Item Open Only`) |
| `allow_multiple_open` | `checkbox` | `true` | Allow multiple questions open simultaneously |
| `chevron_color` | `color` | `#0b1320` | Chevron arrow icon color |
| `accent_color` | `color` | `#0284c7` | Active/hover accent color for links and icons |
| `question_color` | `color` | `#0b1320` | Question text color |
| `question_size_desktop` | `range` | `16px` | Question desktop font size (`14px` to `22px`) |
| `question_size_mobile` | `range` | `15px` | Question mobile font size (`13px` to `18px`) |
| `answer_color` | `color` | `#64748b` | Answer text color |
| `answer_size` | `range` | `14px` | Answer font size (`12px` to `18px`) |
| `answer_line_height` | `range` | `1.6` | Answer line height (`1.3` to `2.0`) |
| `enable_faq_schema` | `checkbox` | `true` | Generates Google FAQPage structured data (JSON-LD) |
| `show_contact_footer` | `checkbox` | `false` | Show bottom contact CTA bar |
| `contact_text` | `text` | *(copy)* | Text prompt in the contact CTA bar |
| `contact_btn_label` | `text` | `Contact Support` | Button label in contact bar |
| `contact_btn_url` | `url` | — | Destination URL for the contact button |
| `padding_top_desktop` / `_bottom_desktop` | `range` | `64px` | Vertical section padding on desktop |
| `padding_top_mobile` / `_bottom_mobile` | `range` | `40px` | Vertical section padding on mobile |

---

### Block Settings (`faq_item`)

Each block represents an individual question and expandable answer:

| Setting | Type | Default | Description |
|---|---|---|---|
| `question` | `text` | `Can I upload my own logo?` | Question text displayed in card header |
| `question_tag` | `select` | `h3` | Semantic HTML tag (`h2`, `h3`, `h4`, `h5`, `div`) |
| `answer` | `richtext` | *(answer)* | Rich text answer supporting formatting and links |
| `is_open_default` | `checkbox` | `false` | Force this specific card open on load regardless of section setting |

---

## 🎨 Presets

The section comes pre-configured with the complete 4-item custom sweatband FAQ from the reference design:

1. **Can I upload my own logo?**
   > *Yes! You can easily upload your logo or artwork on the product page. We'll make sure it's perfectly embroidered.*
2. **Which colours are available?**
   > *We offer a wide range of colours for both wristbands and headbands. You can see all available options on the product pages.*
3. **How long does delivery take?**
   > *For customized orders, the approximate delivery time is 4–5 weeks across Europe.*
4. **Do you offer custom orders for companies or teams?**
   > *Yes! We specialize in custom orders for sports clubs, companies, events and promotional use. Contact us for larger quantities.*

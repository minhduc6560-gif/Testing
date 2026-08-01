# Design System Inspired by Leandigi

## 1. Visual Theme & Atmosphere

Leandigi's design system embodies a modern, professional digital marketing agency aesthetic with bold contrasts and purposeful hierarchy. The visual language combines a dark, sophisticated color palette with striking golden-yellow accents that command attention and drive conversion. This creates an energetic yet trustworthy atmosphere—appropriate for a B2B SaaS platform focused on sales funnels and digital transformation. The design prioritizes clarity and bold calls-to-action, using generous whitespace and clean typography to guide users through complex business solutions. The dark backgrounds with luminous accents create visual depth while maintaining accessibility and contemporary appeal.

**Key Characteristics**
- Dark-dominant color strategy with golden-yellow CTAs
- High-contrast typography for readability and hierarchy
- Generous spacing and whitespace for breathing room
- Bold, square-edged components with minimal ornamentation
- Focused on conversion-oriented UI patterns
- Professional yet approachable visual tone
- Strong emphasis on primary yellow action buttons

## 2. Color Palette & Roles

### Primary
- **Primary CTA Yellow** (`#FFBC01`): Primary action buttons, high-importance CTAs, hero section buttons
- **Secondary Yellow** (`#F0C334`): Supporting yellow elements, alternative action states

### Accent Colors
- **Link Blue** (`#0000EE`): Hyperlinks, secondary navigation, emphasized text (used 158 times across site)
- **Sky Blue** (`#188BF6`): Alternative accent, complementary interactive states
- **Cyan** (`#81E6D9`): Accent highlights, tertiary interactive elements
- **Sage Green** (`#9AE6B4`): Success indicators, positive reinforcement elements
- **Orange Accent** (`#F6AD55`): Tertiary accent, supporting visual elements

### Interactive
- **Success Green** (`#37CA37`): Success states, positive confirmations, checkmarks
- **Error Red** (`#E93D3D`): Error states, warnings, destructive actions

### Neutral Scale
- **Pure Black** (`#000000`): Primary text, backgrounds, strong contrasts (700 uses)
- **Pure White** (`#FFFFFF`): Text on dark backgrounds, primary backgrounds (162 uses)
- **Dark Gray** (`#222222`): Secondary text, reduced contrast backgrounds
- **Mid Gray** (`#3B3B3B`): Tertiary text, disabled states
- **Light Gray** (`#CBD5E0`): Borders, dividers, subtle separators
- **Off-White** (`#FAFAFA`): Light backgrounds, subtle surface differentiation
- **Very Light Gray** (`#F5F5F5`): Alternative light background
- **Pale Blue Gray** (`#EBEEF2`): Subtle background tint

### Surface & Borders
- **Border Light** (`#CBD5E0`): Standard borders, dividers, outlines
- **Surface Light** (`#FAFAFA`): Secondary background surfaces, cards
- **Surface Very Light** (`#F5F5F5`): Alternative light surfaces

### Semantic / Status
- **Warning Primary** (`#FFBC01`): Warning messages, important alerts (19 uses)
- **Warning Secondary** (`#F0C334`): Supporting warning context (15 uses)
- **Success** (`#37CA37`): Positive confirmations, completed states
- **Error** (`#E93D3D`): Error messages, destructive actions

## 3. Typography Rules

### Font Family
**Primary:** Roboto (`https://fonts.googleapis.com/css?family=Roboto:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i&display=swap`) with fallback: `-apple-system, BlinkMacSystemFont, Segoe UI, Arial, sans-serif`

**Secondary:** Times New Roman with fallback: `Georgia, serif` (for specific span typography)

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| **Display / H1** | Roboto | 60px | 700 | 78px | normal | Hero headlines, page titles, major sections |
| **Heading / H2** | Roboto | 24px | 200 | 31.2px | normal | Section headings, subsection titles |
| **Body Text** | Roboto | 16px | 500 | 20.8px | normal | Standard paragraph text, descriptions |
| **Button / CTA** | Roboto | 16px | 400 | normal | normal | Action button labels, call-to-action text |
| **Link** | Roboto | 16px | 500 | 20.8px | normal | Navigation links, hyperlinks |
| **Caption / Meta** | Roboto | 14px | 400 | 18px | normal | Small supporting text, annotations (inferred) |
| **Code / Monospace** | `Courier New` | 14px | 400 | 18px | normal | Code blocks, technical snippets (inferred) |

### Principles
- **Contrast-driven hierarchy:** Weight and size work together to establish visual priority without relying on color alone
- **Generous line heights:** All text uses 1.3x+ line height for improved readability and breathing room
- **Weight stratification:** Use 200, 400, 500, and 700 weights to create clear distinctions without excessive variety
- **Dark-mode readiness:** All typography leverages sufficient contrast ratios against both light and dark backgrounds
- **Accessibility first:** Font sizes never drop below 14px for body content; headings use semantic weight to reinforce structure
- **Professional restraint:** Only Roboto and Times New Roman are used; consistent fallback stacks ensure compatibility

## 4. Component Stylings

### Buttons

#### Primary CTA Button
- **Background Color:** `#FFBC01`
- **Text Color:** `#000000`
- **Font:** Roboto, 16px, weight 400
- **Padding:** `15px 20px`
- **Height:** `51px`
- **Border:** `0px none`
- **Border Radius:** `0px`
- **Box Shadow:** `none`
- **Line Height:** `normal`
- **Hover State:** Background `#F0C334` (darker yellow), text remains `#000000`
- **Active State:** Background `#E6B800` (pressed yellow), slight inset effect
- **Disabled State:** Background `#CBD5E0`, text `#3B3B3B`, cursor `not-allowed`

#### Secondary Button
- **Background Color:** `#FFFFFF`
- **Text Color:** `#000000`
- **Font:** Roboto, 16px, weight 400
- **Padding:** `15px 20px`
- **Height:** `51px`
- **Border:** `2px solid #000000`
- **Border Radius:** `0px`
- **Box Shadow:** `none`
- **Hover State:** Background `#F5F5F5`, border remains `#000000`
- **Active State:** Background `#EBEEF2`, inset border

#### Ghost Button (Text Only)
- **Background Color:** `transparent`
- **Text Color:** `#0000EE`
- **Font:** Roboto, 16px, weight 400
- **Padding:** `15px 20px`
- **Height:** `51px`
- **Border:** `0px none`
- **Border Radius:** `0px`
- **Box Shadow:** `none`
- **Hover State:** Text color `#188BF6`, background `rgba(0, 0, 238, 0.08)`
- **Active State:** Text color `#0000CC`, background `rgba(0, 0, 238, 0.15)`

### Cards & Containers

#### Standard Card
- **Background Color:** `#FFFFFF`
- **Border:** `1px solid #CBD5E0`
- **Border Radius:** `0px`
- **Padding:** `32px`
- **Box Shadow:** `none`
- **Text Color:** `#000000`
- **Hover State:** Border `#188BF6`, background remains `#FFFFFF`

#### Dark Card (Over Dark Background)
- **Background Color:** `#222222`
- **Border:** `1px solid #3B3B3B`
- **Border Radius:** `0px`
- **Padding:** `32px`
- **Box Shadow:** `none`
- **Text Color:** `#FFFFFF`
- **Heading Text Color:** `#FFBC01` (if emphasizing)

### Inputs & Forms

#### Text Input
- **Background Color:** `#FFFFFF`
- **Border:** `1px solid #CBD5E0`
- **Border Radius:** `0px`
- **Padding:** `12px 16px`
- **Font:** Roboto, 16px, weight 400
- **Text Color:** `#000000`
- **Placeholder Color:** `#CBD5E0`
- **Focus State:** Border `#0000EE`, box-shadow `inset 0 0 0 2px rgba(0, 0, 238, 0.1)`
- **Error State:** Border `#E93D3D`, background `rgba(233, 61, 61, 0.05)`

#### Select Dropdown
- **Background Color:** `#FFFFFF`
- **Border:** `1px solid #CBD5E0`
- **Border Radius:** `0px`
- **Padding:** `12px 16px`
- **Font:** Roboto, 16px, weight 400
- **Text Color:** `#000000`
- **Focus State:** Border `#0000EE`
- **Disabled State:** Background `#F5F5F5`, border `#EBEEF2`, text `#3B3B3B`

#### Checkbox / Radio
- **Border:** `2px solid #CBD5E0`
- **Border Radius:** `2px` (checkbox) / `50%` (radio)
- **Checked Background:** `#0000EE`
- **Checked Border:** `2px solid #0000EE`
- **Focus State:** Box-shadow `0 0 0 3px rgba(0, 0, 238, 0.1)`

### Navigation

#### Primary Navigation (Header)
- **Background Color:** `#000000`
- **Height:** `60px`
- **Padding:** `0px 40px`
- **Link Color:** `#FFFFFF`
- **Link Font:** Roboto, 16px, weight 500
- **Active Link Color:** `#FFBC01`
- **Hover Link Color:** `#81E6D9`
- **Z-index:** `100`

#### Navigation Links
- **Font:** Roboto, 16px, weight 500
- **Color:** `#FFFFFF`
- **Text Decoration:** `none`
- **Padding:** `12px 0px`
- **Border Bottom:** `2px solid transparent`
- **Hover State:** Border bottom `#FFBC01`, color remains `#FFFFFF`
- **Active State:** Border bottom `#FFBC01`, color `#FFBC01`

#### Dropdown Menu
- **Background Color:** `#000000`
- **Border:** `1px solid #3B3B3B`
- **Padding:** `8px 0px`
- **Min Width:** `200px`
- **Item Padding:** `12px 16px`
- **Item Hover Background:** `#222222`
- **Item Text Color:** `#FFFFFF`
- **Z-index:** `200`

### Badges

#### Success Badge
- **Background Color:** `rgba(55, 202, 55, 0.1)`
- **Text Color:** `#37CA37`
- **Border:** `1px solid #37CA37`
- **Padding:** `4px 8px`
- **Border Radius:** `0px`
- **Font:** Roboto, 12px, weight 500

#### Warning Badge
- **Background Color:** `rgba(255, 188, 1, 0.1)`
- **Text Color:** `#FFBC01`
- **Border:** `1px solid #FFBC01`
- **Padding:** `4px 8px`
- **Border Radius:** `0px`
- **Font:** Roboto, 12px, weight 500

#### Error Badge
- **Background Color:** `rgba(233, 61, 61, 0.1)`
- **Text Color:** `#E93D3D`
- **Border:** `1px solid #E93D3D`
- **Padding:** `4px 8px`
- **Border Radius:** `0px`
- **Font:** Roboto, 12px, weight 500

## 5. Layout Principles

### Spacing System

**Base Unit:** `4px`

**Scale:**
- `4px`: Minimal spacing between inline elements
- `8px`: Tight spacing between related components
- `12px`: Standard spacing within components (input padding)
- `16px`: Comfortable spacing between form fields, inline padding
- `20px`: Standard margin between sections
- `32px`: Generous spacing within cards and containers
- `40px`: Major section margins, header padding
- `44px`: Large padding for hero sections (inferred)
- `72px`: Large gap between major sections
- `100px`: Hero section vertical margins
- `136px`: Extra-large spacing between sections (inferred)
- `140px`: Maximum padding for full-bleed sections

**Usage Context:**
- **4–8px:** Icon spacing, micro interactions, dense layouts
- **12–16px:** Form field padding, button internal spacing, component density
- **20–32px:** Section spacing, card margins, comfortable reading distance
- **40–100px:** Major layout transitions, hero sections, breathing room
- **136–140px:** Full-screen sections, maximum-width padding equivalents

### Grid & Container

- **Max Width Container:** `1200px` (inferred from typical web standards)
- **Gutter Width:** `20px` (half-gutter on each side of grid items)
- **Column Strategy:** 12-column grid system (inferred from modern standards)
- **Breakpoint Strategy:**
  - Desktop (1024px+): Full container width
  - Tablet (768px–1023px): 90% width with increased gutters
  - Mobile (320px–767px): Full width with edge padding `16px`

**Section Patterns:**
- **Hero sections:** Full bleed with `140px` vertical padding, centered content
- **Content sections:** Max-width container, symmetric horizontal margins
- **Cards grid:** 3–4 columns on desktop, 2 on tablet, 1 on mobile
- **Alternating layouts:** Content left/image right (and vice versa) with `72px` gap

### Whitespace Philosophy

Leandigi employs **generous whitespace** as a strategic tool for visual hierarchy and comprehension. Large vertical gaps (`72px–136px`) separate distinct sections, preventing information overload. Horizontal padding (`40px–140px`) creates breathing room around content blocks, especially critical in hero sections. Component-level spacing (`12px–32px`) maintains clear relationships between related elements. This approach elevates the visual tone, reinforces professionalism, and guides user focus toward primary CTAs.

### Border Radius Scale

- **0px:** All components (buttons, cards, inputs, navigation)—sharp, square edges reinforce modern, tech-forward aesthetic
- **2px:** Subtle radius for checkboxes only, minimal softness where needed

### Border Widths

- **1px:** Standard borders on cards, inputs, form elements, light dividers
- **2px:** Focus states on form inputs, radio button/checkbox outlines, prominent borders on secondary buttons

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| **Base** | `box-shadow: none` | Flat buttons, primary cards, base surfaces |
| **Hover** | `box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1)` | Card hover, button lift on interaction |
| **Overlay / Modal** | `box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3)` | Modals, dropdowns, popovers |
| **Sticky / Fixed** | `box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15)` | Navigation header, sticky sidebars |

**Shadow Philosophy:**
Leandigi embraces a **minimal shadow strategy**, avoiding drop shadows for most base components to maintain a flat, modern appearance. Shadows are reserved for interactive states (hover cards, modals, overlays) where they communicate depth and elevation. The primary shadow uses a soft black at 10% opacity, creating subtle lift without visual clutter. This approach supports the bold, design-forward aesthetic while maintaining clarity on dark backgrounds.

### Opacity Levels
- **80% (0.80):** Primary opacity for semi-transparent overlays, disabled states
- **10% (0.10):** Subtle background tints, soft shadow overlays, hover backgrounds
- **5% (0.05):** Extremely subtle backgrounds, focus states on light elements

### Z-index / Layering

- **Base:** `z-index: 2`—Standard document flow elements
- **Sticky Navigation:** `z-index: 100`—Header, top navigation bar
- **Dropdown / Submenu:** `z-index: 200`—Menu overlays, secondary navigation
- **Modal / Dialog:** `z-index: 9999`—Full-screen overlays, modal windows
- **Tooltip / Popovers:** `z-index: 999` (inferred)—Floating information, contextual help

## 7. Do's and Don'ts

### Do
- **Use `#FFBC01` yellow for primary CTAs**—It's the dominant conversion color across the site and commands attention
- **Maintain sharp `0px` border radius**—Reinforces the modern, tech-forward brand identity
- **Leverage generous spacing (`20px–72px` between sections)**—Creates visual breathing room and aids comprehension
- **Enforce high contrast typography**—Weight 700 for headlines, weight 500 for body ensure readability on both light and dark backgrounds
- **Deploy dark backgrounds (`#000000` or `#222222`) with white text**—Establishes professionalism and supports nighttime usage
- **Apply icons and visual accents in cyan (`#81E6D9`), sage green (`#9AE6B4`), or secondary yellow (`#F0C334`)**—Extends the accent palette while maintaining hierarchy
- **Use link blue (`#0000EE`) consistently for all hyperlinks**—Reinforces navigation clarity
- **Test all form inputs with focus states** (blue `#0000EE` border + light inset shadow)—Ensures accessibility compliance

### Don't
- **Avoid rounded corners (`border-radius > 0px`)** on primary components—The sharp aesthetic is core to the brand
- **Don't mix too many accent colors in a single section**—Stick to one primary accent + max one secondary accent per layout
- **Never use light text on `#FFBC01` backgrounds**—Creates insufficient contrast; always use black text on yellow CTAs
- **Avoid using red (`#E93D3D`) for general messaging**—Reserve it strictly for errors and destructive actions
- **Don't reduce opacity below `0.80` for disabled states**—Maintain visual distinction without ghosting elements
- **Never set line-height below `1.3x` font size**—Readability suffers on both desktop and mobile
- **Avoid inline color emphasis in body text**—Use weight changes instead (400 → 500 → 600)
- **Don't apply shadows to flat background components**—Reserve shadows for interactive and elevated elements only
- **Never exceed a `40px` font size for body copy**—Hierarchy is established through weight and sizing strategy, not excessive scale

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Key Changes | Column Count |
|------------|-------|-------------|--------------|
| **Mobile** | 320px–767px | Single column, full width, `16px` edge padding, `20px` section gaps, button width 100% | 1 |
| **Tablet** | 768px–1023px | 2–3 columns, 90% container width, `24px` gutters, `40px` section margins, font sizes reduced 10% | 2–3 |
| **Desktop** | 1024px+ | 3–4 columns, 1200px max-width, `20px` gutters, `72px` section spacing, full typography | 4 |
| **Large Desktop** | 1440px+ | Max-width bumped to 1400px, increased padding symmetry | 4 |

### Touch Targets
- **Minimum touch target size:** `44px × 44px` (buttons, interactive elements)
- **Recommended:** `56px × 56px` on mobile for high usability
- **Spacing between targets:** Minimum `8px` to prevent accidental activation
- **Form input height:** `51px` (exceeds minimum, enhances comfort)
- **Navigation link padding:** `12px` vertical, `16px` horizontal minimum

### Collapsing Strategy
- **Navigation:** Desktop horizontal nav → Tablet sticky header with dropdown menu → Mobile hamburger icon with full-screen slide-out menu
- **Cards:** Desktop 3–4 column grid → Tablet 2 column → Mobile single column, stacked vertically
- **Hero heading:** Desktop `60px` H1 → Tablet `40px` (inferred) → Mobile `28px` (inferred) with adjusted line-height
- **Sections:** Desktop `72px` gaps → Tablet `40px` gaps → Mobile `20px` gaps
- **Padding:** Desktop `40px` → Tablet `24px` → Mobile `16px` (edge margins)
- **Button width:** Desktop auto / `192px–405px` → Tablet `100%` → Mobile `100%` with max-width `400px`

## 9. Agent Prompt Guide

### Quick Color Reference
- **Primary CTA:** Yellow (`#FFBC01`) on black backgrounds, black text
- **Link Text:** Blue (`#0000EE`) for standard hyperlinks, white (`#FFFFFF`) on dark backgrounds
- **Heading Text:** Black (`#000000`) on light, white (`#FFFFFF`) on dark, optional golden accent (`#FFBC01`)
- **Body Text:** Black (`#000000`) primary, `#222222` secondary on light; white (`#FFFFFF`) on dark
- **Backgrounds:** `#FFFFFF` light, `#000000` or `#222222` dark, `#FAFAFA` subtle alternative light
- **Borders:** `#CBD5E0` standard, `#3B3B3B` dark mode
- **Success:** `#37CA37` (green)
- **Error:** `#E93D3D` (red)
- **Warning:** `#FFBC01` primary, `#F0C334` secondary

### Iteration Guide

1. **Every primary button is `#FFBC01` with black text, `15px 20px` padding, `51px` height, `0px` radius, Roboto 16px weight 400**—Zero exceptions; this is the conversion driver.

2. **All headings use Roboto: H1 is `60px` weight 700 line-height `78px`, H2 is `24px` weight 200 line-height `31.2px`**—Never invert weights or sizes; maintain the precise hierarchy.

3. **Body text is always `16px` Roboto weight 500 with line-height `20.8px`**—Ensures readability across all backgrounds and screen sizes.

4. **Form inputs and buttons use `51px` height with `12px–16px` padding**—Exceeds touch targets; prioritizes usability.

5. **Apply `#0000EE` to all hyperlinks with weight 500**—Reinforces navigation clarity; never use other colors for standard links.

6. **Spacing between major sections is `72px` on desktop, `40px` on tablet, `20px` on mobile**—Scale proportionally with viewport size.

7. **All component borders are `0px` radius with `1px` stroke in `#CBD5E0`**—Maintains the sharp, modern aesthetic; never round corners except where explicitly required (radio buttons = `50%`).

8. **Dark backgrounds are `#000000` or `#222222`; light backgrounds are `#FFFFFF` or `#FAFAFA`**—No gradients unless explicitly specified; maintain flat design language.

9. **Focus states on form inputs deploy `#0000EE` `2px` border + `inset 0 0 0 2px rgba(0, 0, 238, 0.1)` shadow**—Ensures keyboard navigation is visible and accessible.

10. **Navigation header is `60px` height with `#000000` background, white text, yellow (`#FFBC01`) active state, `z-index: 100`**—Sticky and prominent for all pages.

11. **Modal and overlay z-index is `9999`; dropdown menus are `200`; sticky elements are `100`**—Layer elements predictably to prevent stacking conflicts.

12. **Use opacity `0.80` for disabled states, `0.10` for hover overlays, `0.05` for subtle background tints**—Never exceed `0.80` opacity in disabled states; always maintain visual clarity.

13. **All buttons and cards have `box-shadow: none` by default; add `0 2px 8px rgba(0, 0, 0, 0.1)` only on hover or elevated states**—Preserve flat aesthetic; reserve shadows for interaction feedback.

14. **Responsive design: Mobile single column (`16px` edge padding), Tablet 2–3 columns (`24px` gutters), Desktop 3–4 columns (`20px` gutters, max-width `1200px`)**—Scale layout proportionally without redesigning components.

15. **Every interactive element has a clear hover state: buttons change yellow shade, cards get blue border, links change color**—Provide obvious visual feedback for all interactions; never leave hover states undefined.
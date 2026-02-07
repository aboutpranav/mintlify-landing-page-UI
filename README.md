# Mintlify Landing Page Recreation

A desktop-first documentation-style website inspired by the [Mintlify website](https://mintlify.com). This assignment focuses on **content structure, readability, and layout accuracy**, recreating the design of the Mintlify landing page.

## 🎯 Project Goal

The goal of this assignment is to achieve content structure, readability, and layout accuracy in recreating the Mintlify landing page, prioritizing faithful reproduction of the information architecture and visual hierarchy.

## 📋 Sections Recreated

This landing page includes the following sections from the original Mintlify website:

### 1. **Header/Navigation**

- Sticky navigation bar with Mintlify logo (SVG)
- Navigation links: Resources, Documentation, Customers, Blog, Pricing
- Two action buttons: "Contact sales" and "Start for free"
- Backdrop blur effect for modern aesthetic

### 2. **Hero Section**

- Main headline: "The Intelligent Knowledge Platform"
- Subheading: "Helping teams create and maintain world-class documentation built for both humans and AI"
- Email input field with integrated CTA button
- Large hero image showcasing the platform interface

### 3. **Logo Section (Social Proof)**

Company logos grid displaying trusted brands:

- Row 1: Anthropic, Coinbase, Microsoft, Perplexity
- Row 2: HubSpot, Twitter, PayPal, Lovable
- 4x2 grid layout for visual balance

### 4. **Features Section**

Main heading: "Built for the intelligence age"

Three feature highlights with detailed descriptions:

**Feature 1: LLMs.txt & MCP**

- Title: "Built for both people and AI"
- Description: Integration with AI workflows through llms.txt and MCP
- Visual: Platform integration showcase

**Feature 2: Agent**

- Title: "Self-updating knowledge management"
- Description: Context-aware content drafting and maintenance
- Visual: Agent interface demonstration

**Feature 3: Assistant**

- Title: "Intelligent assistance for your users"
- Description: AI-powered guided documentation experience
- Visual: Assistant interface (full-width layout)

### 5. **Enterprise Section**

Background: Dark theme (#191a1a)

**Enterprise Header:**

- Badge: "Enterprise-reinvention"
- Main heading: "Bring intelligence to enterprise knowledge"
- Description: Modernization without rebuilding
- CTA: "Explore for enterprise"

**Enterprise Content (Two columns):**

1. **Build with partnership**
   - White-glove documentation expertise
   - Migration support and elevated SLAs

2. **Compliance and access control**
   - SOC 2, ISO/27001, GDPR compliance
   - SAML-based SSO

**Enterprise Image:**

- Full-width product screenshot with rounded corners

**Enterprise Logos:**
Five company logos in a single row:

- Anthropic, Coinbase, HubSpot, Zapier, AT&T

### 6. **Customers Section**

- Badge: "Customers"
- Main heading: "Unlock knowledge for any industry"
- Subheading: Industry leaders scaling with Mintlify

**Customer Stories (Carousel layout):**

1. **Perplexity Case Study**
   - Image with rounded corners
   - Teaser text about AI-native developer experience
   - "Read story" link

2. **X (Twitter) Case Study**
   - Image with rounded corners
   - Teaser about global town square developer experience
   - "Read story" link

**Navigation Controls:**

- Previous/Next circular buttons
- Left button faded (start of carousel)

### 7. **Secondary Hero Section (CTA)**

- Main heading: "Make documentation your winning advantage"
- Subheading: Future-proofing documentation
- Two CTAs: "Get Started for free" and "Get a demo"

**Two-column Info Cards:**

**Card 1: Pricing on your terms**

- Icon: Pricing symbol
- Description: Pick the best plan
- Link: "Pricing details"
- Border divider on right

**Card 2: Start building**

- Icon: Building symbol
- Description: Deploy in minutes
- Link: "Quickstart"

### 8. **Footer**

**Footer Navigation:**

- Mintlify logo
- Social media icons: LinkedIn, Twitter, GitHub
- Border separation design

**Footer Links (5-column grid):**

1. **EXPLORE**
   - Startups, Enterprise, Switch
   - OSS Program, Customers, Pricing

2. **RESOURCES**
   - Blog, Guides, Feature Requests
   - Changelog, Getting Started

3. **DOCUMENTATION**
   - Documentation, API Reference, Components

4. **COMPANY**
   - Careers, Wall of Love

5. **LEGAL**
   - Privacy Policy, Responsible Disclosure
   - Terms of Service, Security, DSR/DSAR

**Security Badge:**

- Text: "Backed by enterprise-grade security"
- Security certification logo

**Copyright:**

- "© 2026 Mintlify, Inc."
- Centered text with muted styling

## 📸 Screenshot

### Full Page View

![Full Minflify Landing Page](screenshots/full-page.png)

## 🎨 Fonts and Colors Used

### Fonts

The project uses a **system font stack** for maximum compatibility and performance:

```css
font-family: Arial, Helvetica, sans-serif;
```

**Font Weights Used:**

- **Regular (400)**: Default body text
- **Light (100)**: Subheadings and secondary text
- **Light-Medium (200)**: Navigation links and tertiary headings
- **Medium (300)**: Feature headings

### Colors

The color scheme uses a dark theme with vibrant green accents:

#### CSS Custom Properties:

```css
:root {
  --primary-color: #08090b; /* Main background - almost black */
  --secondary-color: #18e299; /* Accent green - Mintlify brand */
  --third-color: #90ecc5; /* Light green - secondary accent */
}
```

#### Color Palette Breakdown:

**Background Colors:**

- **Primary Background**: `#08090b` - Deep black with subtle blue undertone
- **Secondary Background**: `#191a1a` - Dark gray (Enterprise & Footer sections)
- **Card Background**: `#080a0a` - Slightly darker than primary for feature cards
- **Semi-transparent Overlays**:
  - `rgba(47, 50, 57, 0.5)` - Secondary buttons
  - `rgba(98, 101, 108, 0.5)` - Input fields

**Text Colors:**

- **Primary Text**: `#ffffff` - Pure white for headings
- **Secondary Text**: `#bebebe` - Light gray for descriptions and body text
- **Muted Text**: `rgb(169, 163, 163)` - Placeholder text

**Accent Colors:**

- **Primary Accent**: `#18e299` - Vibrant mint green (badges, links, highlights)
- **Secondary Accent**: `#90ecc5` - Lighter mint green (alternative uses)

**Border Colors:**

- **Primary Borders**: `#333131` / `0.1px solid #333131` - Feature cards
- **Secondary Borders**: `#393737` / `1px solid #393737` - Footer sections
- **Tertiary Borders**: `#2d2c2c` / `1px solid #2d2c2c` - Info card dividers

**Button Colors:**

- **Primary Button**:
  - Background: `#ffffff` (white)
  - Text: `var(--primary-color)` (#08090b)
- **Secondary Button**:
  - Background: `rgba(47, 50, 57, 0.5)` (semi-transparent gray)
  - Text: `#ffffff` (white)
- **Faded State**: `#bebebe` (light gray for inactive buttons)

#### Color Usage Patterns:

**Navigation:**

- Background: Transparent with `backdrop-filter: blur(8px)`
- Text: `#ffffff`
- Font weight: `200` (Light)

**Hero Section:**

- Background: Custom image with fallback to `var(--primary-color)`
- Headings: `#ffffff`
- Subheadings: `#ffffff` with font-weight `100`

**Feature Section:**

- Badges: `#18e299` (secondary-color)
- Card backgrounds: `#080a0a`
- Card borders: `#333131`
- Body text: `#bebebe`

**Enterprise Section:**

- Section background: `#191a1a`
- Text colors maintain primary/secondary pattern
- Badge: `#18e299`

**Links:**

- Default: `#bebebe`
- Accent links: `#18e299` (var(--secondary-color))
- Text decoration: `none`

## 🖼️ Visual Design Elements

### Border Radius Usage

- Buttons: `25px` (pill-shaped)
- Feature cards: `10px`
- Enterprise image: `25px`
- Customer images: `60px` (extreme rounding)
- Info card icons: `15px`

### Grid Layouts

- **Logos**: `repeat(4, 270px)` × `repeat(2, 100px)`
- **Features**: `repeat(2, 1fr)` with 16px gap
- **Enterprise logos**: `repeat(5, 1fr)`
- **Footer links**: `repeat(5, 1fr)`

## 🚀 Getting Started

### Prerequisites

- A modern web browser
- All image assets in the `./assets/` directory

### Installation

1. Clone or download this repository
2. Ensure all assets are in the `./assets/` directory:

3. Open `index.html` in your web browser

## 🎯 Key Features

- **Sticky Navigation**: Fixed header with backdrop blur effect
- **Responsive Grid Layouts**: Modern CSS Grid for flexible layouts
- **SVG Logo Integration**: Scalable Mintlify branding
- **Custom Input Styling**: All-unset reset for clean form design
- **Strategic Color Usage**: Mint green accents against dark backgrounds
- **Semantic HTML**: Proper use of semantic elements (nav, main, section, footer)
- **Consistent Spacing**: Systematic padding (72px, 32px, 144px pattern)
- **Visual Hierarchy**: Font weights and sizes create clear information hierarchy

## 📐 Layout Specifications

### Container Widths

- **Navigation**: 80% of viewport
- **Hero Header**: 50% width, centered
- **Hero Input**: 80% of hero-header width
- **Hero Image**: 1080px × 656px
- **Content Containers**: 1080px standard width
- **Feature Grid**: 1080px with 60px padding

### Spacing System

- **Section Padding**: `72px 32px 144px 32px` (standard pattern)
- **Grid Gaps**:
  - Features: `16px`
  - Customers: `30px`
  - Footer: Varies by subsection
- **Element Gaps**: `10px`, `15px`, `20px` based on context

### Typography Scale

- **H1 (Main)**: 60px
- **H1 (Section)**: 36px
- **H1 (Subsection)**: 18-24px
- **H2 (Description)**: 15-20px
- **H3 (Badges)**: 12px
- **Body/Links**: 15px

## 🎨 Design Patterns

### Card Design Pattern

```css
border: 0.1px solid #333131;
padding: 30px;
border-radius: 10px;
background-color: #080a0a;
```

### Button Pattern

```css
/* Primary */
background-color: #ffffff;
color: var(--primary-color);
padding: 10px 15px;
border-radius: 25px;

/* Secondary */
background-color: rgba(47, 50, 57, 0.5);
color: #ffffff;
```

### Section Pattern

```css
padding: 72px 32px 144px 32px;
text-align: center;
```

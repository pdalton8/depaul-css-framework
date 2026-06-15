# DePaul Bootstrap Theme

A custom Bootstrap 5-inspired CSS framework built from scratch using DePaul University's official brand guidelines. Features responsive components, a 12-column grid system, and DePaul's signature design patterns.

## Features

- **Brand-Aligned Design**: Built using official DePaul colors, typography, and design patterns
- **Fully Responsive**: Mobile-first design with breakpoints at 576px, 768px, 992px, 1200px, and 1400px
- **Token-Based Theming**: CSS custom properties for easy customization
- **Production-Ready Components**: Buttons, cards, navigation, forms, and more
- **Portal Containers**: Pre-built section patterns for rapid page composition
- **Lightweight**: ~35KB CSS with minimal JavaScript (Bootstrap collapse only)

## Quick Start

### CDN Usage

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Page Title</title>
    
    <!-- Google Fonts (Required) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Rethink+Sans:wght@300;400;500;600;700;800&family=Newsreader:ital,wght@0,400;0,500;0,600;0,700;1,400&display=swap" rel="stylesheet">
    
    <!-- DePaul Bootstrap Theme -->
    <link rel="stylesheet" href="css/depaul-bootstrap-theme.css">
    
    <!-- Bootstrap JS (Required for navbar collapse only) -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous" defer></script>
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```

## Dependencies

### External CDNs (2)

1. **Google Fonts API** - Required for DePaul typography
   - Rethink Sans (300-800 weights)
   - Newsreader (400-700 weights, regular + italic)

2. **Bootstrap JS Bundle** (5.3.2) - Required only for navbar collapse functionality
   - Loaded from: `cdn.jsdelivr.net`
   - Can be removed if not using collapsible navigation

### Image CDNs

The framework references DePaul's official image CDNs for examples:
- `edge.sitecorecloud.io` - DePaul logo
- `dpu-p-001.sitecorecontenthub.cloud` - DePaul content hub
- `cst.brightspotcdn.com` - Stock campus imagery

Replace with your own assets in production.

## File Structure

```
depaul-bootstrap-framework/
├── css/
│   └── depaul-bootstrap-theme.css    # Main CSS framework (~35KB)
├── examples/
│   ├── demo.html                      # Component showcase
│   ├── portal-containers.html         # Pre-built section patterns
│   └── starter-template.html          # Basic page template
└── README.md
```

## Core Components

### Layout
- **Container & Grid**: 12-column responsive grid system
- **Responsive Breakpoints**: xs, sm, md, lg, xl, xxl

### Navigation
- **Navbar**: Bootstrap 5 collapse with DePaul styling
- **Mobile Menu**: Hamburger-to-X animation with full-width expansion

### Buttons
- **Variants**: Primary, Secondary, Outline (White & Primary)
- **Sizes**: Small, Default, Large
- **Auto-Arrow**: `.btn-arrow` class for automatic arrow icons
- **DePaul Signature**: Asymmetric rounded corners (top-right + bottom-left)

### Cards
- **Standard Card**: Image, title, text, buttons
- **DePaul Signature**: `.card-depaul` with asymmetric corners
- **Automatic Spacing**: Bootstrap-style spacing with `> * + *` selector

### Portal Containers

Pre-built section patterns for rapid page composition:

1. **Feature Container**: Two-column image + content layout
2. **Spotlight Accordion**: Horizontal accordion with background images
3. **Quote Banner**: Professional quote display with image
4. **Difference Makers**: Three-column alumni/testimonial cards

### Typography
- **Headings**: H1-H6 with Rethink Sans
- **Body Text**: 16px base, 1.6 line-height
- **Display Classes**: Large hero headings
- **Serif Variant**: Newsreader for editorial content

### Utilities
- Spacing (margin/padding)
- Display (flex, block, inline)
- Text alignment and colors
- Background colors
- Border utilities
- Shadow utilities
- DePaul signature corners (`.rounded-depaul`, `.img-border-radius`)

## Design System

### Colors

**Primary Blues**
- `--depaul-blue`: #003da5 (Primary)
- `--depaul-navy`: #00205b (Secondary)
- `--depaul-blue-50` to `--depaul-blue-600`: Full palette

**Neutrals**
- `--depaul-gray-50` to `--depaul-gray-900`: Complete grayscale

### Typography

**Font Families**
- Headings: Rethink Sans (Google Fonts)
- Body: Rethink Sans
- Editorial: Newsreader (serif variant)

**Font Weights**
- Light: 300
- Regular: 400
- Medium: 500
- Semibold: 600
- Bold: 700
- Extra Bold: 800

### Spacing Scale

Based on 1rem (16px):
- 0: 0
- 1: 0.25rem (4px)
- 2: 0.5rem (8px)
- 3: 1rem (16px)
- 4: 1.5rem (24px)
- 5: 3rem (48px)

### Border Radius

**Standard**
- Small: 0.25rem
- Default: 0.375rem
- Large: 0.5rem

**DePaul Signature (Asymmetric)**
- Small: `0 0.75rem 0 0.75rem`
- Medium: `0 1.5rem 0 1.5rem`
- Large: `0 4.5rem 0 4.5rem`

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile Safari (iOS 12+)
- Chrome Mobile (Android 8+)

## Examples

See the `examples/` directory for:
- **demo.html**: Complete component showcase
- **portal-containers.html**: Pre-built section patterns
- **starter-template.html**: Basic page structure

## Customization

Override CSS custom properties in your own stylesheet:

```css
:root {
  --depaul-blue: #your-color;
  --bs-font-sans-serif: 'Your Font', sans-serif;
}
```

## License

This framework is based on DePaul University's brand guidelines and is intended for DePaul-related projects.

## Credits

Built with inspiration from:
- DePaul University Brand Guidelines
- Bootstrap 5 Framework
- Modern CSS best practices

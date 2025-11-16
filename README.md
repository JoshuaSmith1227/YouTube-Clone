# YouTube Homepage Clone - HTML/CSS Practice

A responsive recreation of YouTube's homepage interface built with HTML and CSS as a learning exercise in modern web layout techniques.

## Overview

This is a static HTML/CSS project that replicates YouTube's homepage layout, created as practice for learning CSS Grid, Flexbox, and responsive design principles. The project focuses on front-end fundamentals without any JavaScript functionality or backend integration.

## Features

### Layout Components

**Header**
- Logo and navigation icons
- Search bar (visual only, no functionality)
- User profile icons

**Sidebar**
- Navigation menu with icons
- Static layout (no collapse functionality)

**Video Grid**
- Responsive CSS Grid layout
- Video thumbnails with duration labels
- Basic metadata display (title, channel, views)

### Technical Implementation

**CSS Techniques:**
- CSS Grid for video layout
- Flexbox for header alignment
- Basic responsive breakpoints
- Fixed positioning for header/sidebar

**Scope:**
- Pure HTML/CSS (no JavaScript)
- Static layout (no interactivity)
- Learning exercise for CSS fundamentals

## Technical Implementation

### File Structure

```
YouTube-Clone/
├── Build/
│   └── YouTube/
│       ├── youtube.html          # Main page structure
│       ├── styles/
│       │   ├── general.css       # Base styles and resets
│       │   ├── header.css        # Top navigation bar
│       │   ├── sidebar.css       # Left navigation menu
│       │   └── video.css         # Video grid and cards
│       ├── icons/                # SVG icons
│       ├── thumbnails/           # Video preview images
│       └── channel-pictures/     # Channel profile images
└── README.md
```

### CSS Techniques

**Grid System**
```css
.video-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  column-gap: 16px;
  row-gap: 40px;
}
```

**Flexbox Layout**
```css
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

**Positioning Strategies**
- Fixed positioning for header and sidebar
- Absolute positioning for overlays (duration, notifications badge)
- Relative positioning for tooltip containers

### HTML Structure

**Semantic Markup**
- Proper use of `<div>` containers for layout
- Descriptive class names following BEM-like conventions
- Image optimization with appropriate formats (WebP for thumbnails)
- Accessibility considerations with alt text

## Design Decisions

### Why Pure CSS?

This project intentionally avoids JavaScript to demonstrate CSS-only capabilities:
- **Learning focus:** Master CSS Grid and Flexbox
- **Performance:** Zero JavaScript overhead
- **Simplicity:** Easier to understand and maintain
- **Foundation:** Provides base for future JavaScript enhancements

### Modular CSS Architecture

Separating styles into four files provides:
- **Maintainability:** Easy to locate and update specific components
- **Reusability:** Components can be reused across pages
- **Collaboration:** Multiple developers can work on different files
- **Performance:** Browser can cache individual stylesheets

### Grid vs. Flexbox

**Grid for video layout:**
- Two-dimensional control (rows and columns)
- Automatic responsive columns
- Consistent spacing and alignment

**Flexbox for header/sidebar:**
- One-dimensional alignment
- Better for navigation bars
- Easier vertical centering

## Responsive Breakpoints

The layout adapts at these viewport widths:

| Screen Size | Columns | Target Devices |
|-------------|---------|----------------|
| < 600px | 1 column | Mobile phones |
| 600-900px | 2 columns | Tablets (portrait) |
| 900-1200px | 3 columns | Tablets (landscape), small laptops |
| > 1200px | 4 columns | Desktops, large screens |

## Browser Compatibility

**Fully Supported:**
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

**Features Used:**
- CSS Grid (2017+)
- Flexbox (2015+)
- CSS Custom Properties (2016+)
- Google Fonts API

## Usage

### Viewing Locally

```bash
cd YouTube-Clone/Build/YouTube
open youtube.html
# Or double-click youtube.html
```

## Project Scope

**What this is:**
- HTML/CSS layout practice
- Exercise in responsive design
- Static UI recreation

**What this isn't:**
- Not a functional web application
- No video playback or backend
- No JavaScript interactivity
- Learning project, not production code

## Learning Outcomes

This project provided practice with:
- CSS Grid and Flexbox layouts
- Responsive design with media queries
- Basic HTML structure
- CSS positioning techniques

---

**Note:** This is a basic HTML/CSS learning exercise. For serious web development projects, see my other repositories featuring systems programming, algorithms, and software architecture.
README_YOUTUBECLONE.md
Displaying README_YOUTUBECLONE.md.

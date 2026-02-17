# Curator Cards - Build Specification

## Project Overview
Build a static three-column card layout displaying three design movements (Bauhaus, Swiss Style, New Wave Typography) with dark theme and bright color accents. Swiss Design aesthetic with modern sensibilities.

## Layout & Structure
- **Title:** "Curator Cards"
- **Layout Type:** Equal-sized 3-column grid
  - All cards: same width, same height, same information structure
  - Responsive: 2-column on tablets, 1-column on mobile
- **Typography:** Modern sans-serif (system fonts acceptable)
- **Static:** No JavaScript, no interactivity

## Card Content & Display Format

### Every Card Shows
- Color-coded accent bar at top (4px solid)
- Movement name (Heading 2)
- Dates (e.g., "1919–1933") - uppercase, muted gray
- Full description paragraph
- Tags (multiple, small labels with subtle colored borders)
- Accountability statement (smaller text, top-bordered)

## Data Source
All content pulled from `CURATOR_NOTES.md`:
1. **Bauhaus (1919–1933)**
2. **Swiss Style / International Typographic Style (1950s–1970s)**
3. **New Wave Typography (1970s–1980s)**

## Color Scheme

### Background
- **Page/Body:** #0a0a0a (near black, very dark)
- **Card Background:** #1a1a1a (dark gray)

### Accent Colors (per movement)
- **Bauhaus:** Red (#FF0000) - top bar, tag borders
- **Swiss Style:** Blue (#0066FF) - top bar, tag borders
- **New Wave:** Yellow (#FFCC00) - top bar, tag borders

### Text Colors
- **Titles:** #ffffff (bright white)
- **Body text:** #e0e0e0 (light gray)
- **Dates:** #888888 (muted gray)
- **Tags:** #e0e0e0 with colored borders (1px, semi-transparent colored)
- **Accountability:** #999999 (dimmer gray) with #e0e0e0 for bold text

## Visual Effects
- **Drop shadows** on all cards (dark shadow for depth in dark theme)
- **Hover effect:** Slight lift (translateY -4px) + enhanced shadow
- **Card styling:** Flat design, no border-radius, 4px colored top bar
- **Flexbox layout** on cards to push accountability to bottom

## Technical Requirements
- HTML structure (semantic, accessible, static)
- CSS for layout, colors, responsive grid, shadows
- NO JavaScript - completely static page
- No external libraries required
- Responsive: 3-column (desktop) → 2-column (tablet) → 1-column (mobile)

## Files to Modify
- `index.html` - Structure (3 equal cards, all info displayed)
- `style.css` - Layout (grid), colors (dark theme + bright accents), shadows, hover effects
- `script.js` - DELETE/REMOVE (not needed for static page)

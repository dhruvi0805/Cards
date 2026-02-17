# Curator Cards - Build Specification

## Project Overview
Build an interactive bento box-style card layout displaying three design movements (Bauhaus, Swiss Style, New Wave Typography) with click-to-swap functionality and Swiss Design aesthetic.

## Layout & Structure
- **Title:** "Curator Cards"
- **Layout Type:** Bento box grid
  - Left side: 1 large card (~60% width)
  - Right side: 2 small cards stacked vertically (~40% width)
- **Typography:** Modern sans-serif (system fonts acceptable)
- **Initial State:** Bauhaus displayed as the large card on left; Swiss Style and New Wave as small cards on right

## Card Content & Display Modes

### Small Card Format
- Movement name
- Dates (e.g., "1919–1933")
- Short description (1-2 sentences max)
- Tags (as individual tag elements)

### Large Card Format
- Movement name
- Dates
- Full description paragraph
- Tags
- Accountability statement (from CURATOR_NOTES.md)

## Data Source
All content pulled from `CURATOR_NOTES.md`:
1. **Bauhaus (1919–1933)**
2. **Swiss Style / International Typographic Style (1950s–1970s)**
3. **New Wave Typography (1970s–1980s)**

## Interactivity
- **Trigger:** Click on any small card
- **Behavior:** 
  - Clicked small card expands to large card (left side)
  - Previously large card shrinks to small card and fills the clicked card's spot
  - Smooth animation/transition during swap (fade/slide)
- **No page reload** - all client-side JavaScript

## Color Scheme
- **Bauhaus:** Red accent (#FF0000 or similar bold red)
- **Swiss Style:** Blue accent (#0066FF or similar bold blue)
- **New Wave:** Yellow accent (#FFCC00 or similar bold yellow)
- **Backgrounds & Text:** Black, white, neutral grays for contrast

### Background Behavior
- Static decorative shapes positioned behind all cards (geometric shapes reflecting Swiss Design principles)
- Background color transitions to a light tint of the active card's accent color when swapped
- All shapes remain static; only background color changes

## Visual Effects
- **Drop shadows** on all cards for depth
- **Smooth transitions** when cards swap (animation duration: ~300-500ms)
- **Clean, rigid spacing** following Swiss grid principles
- Shapes (circles, rectangles, etc.) positioned asymmetrically behind cards, not obstructing card content

## Technical Requirements
- HTML structure (semantic, accessible)
- CSS for layout, colors, shadows, animations
- JavaScript for click interaction and card swapping logic
- No external libraries required (vanilla JS)
- Responsive-friendly (mobile considerations optional but welcome)

## Files to Modify
- `index.html` - Structure
- `style.css` - Layout, colors, animations
- (Optional: `script.js` or inline `<script>` tag for interactivity)

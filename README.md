# Periodic Table CSS Documentation

This document explains the CSS structure and styling for an interactive periodic table of elements.

## Table Structure

The periodic table is structured using HTML divs with the following classes:

- `.periodic`: The main container for the entire table
- `.periodic-row`: Represents a row in the periodic table
- `.cell`: Represents a cell that contains an element
- `.element`: Represents an individual element

## Element Structure

Each element is structured as follows:

```html
<div class="cell">
  <div class="element">
    <div class="at_num">Atomic Number</div>
    <div class="symbol">Element Symbol</div>
    <div class="at_details">Atomic Mass</div>
  </div>
</div>
```

## Styling

### Basic Layout

- The table adjusts its height based on the viewport width, ranging from 200px to 800px.
- Each cell takes up 5.55% of the width (18 columns).
- Elements are positioned absolutely within their cells.

### Colors

Elements are color-coded based on their types:

- Default: `rgba(0, 128, 128, 0.6)` (teal)
- Metals: `rgba(0, 160, 96, 0.6)` (green-blue)
- Non-metals: `rgba(0, 192, 64, 0.6)` (green)
- Noble gases: `rgba(64, 192, 0, 0.6)` (light green)
- Lanthanides and Actinides: `rgba(0, 96, 160, 0.6)` (blue)

Colors become more opaque on hover.

### Hover Effects

- Elements scale up to 3 times their original size on hover.
- The transform origin is adjusted for elements at the edges of the table to ensure they remain visible.

### Responsiveness

The table is responsive with different styles for various screen sizes:

- Small tablet portrait: 600px+
- Tablet landscape or small laptop: 800px+
- Normal screen: 992px+
- Large screen: 1200px+

As the screen size increases, font sizes increase and more details become visible.


## Customization

To customize the table:

1. Modify color values in the CSS to change the element type colors.
2. Adjust the `.element` transform scale for a different hover effect.
3. Fine-tune the media query breakpoints and associated styles for different screen sizes.

Remember to test any changes across various device sizes to ensure responsiveness is maintained.
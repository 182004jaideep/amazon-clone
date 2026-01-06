Technical Project Summary: Amazon Clone
1. Layout & Architecture
Component-Based CSS: Used a modular approach by separating styles into header.css, home.css, and cart.css to ensure maintainability and reusability across pages.

CSS Grid (Adaptive): Implemented grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)) for the product grid. This allows the layout to automatically adapt the number of columns based on the screen width without requiring dozens of media queries.

Flexbox Navigation: Leveraged Flexbox for the header to handle space distribution between the logo, search bar, and nav items.

2. UI/UX Features
Fixed Header: Used position: fixed with z-index: 100 to keep navigation accessible at all times. I compensated for this by adding padding-top: 100px to the body to prevent content overlap.

Interactive Elements: Added transition effects on buttons and clear :hover states (white borders for nav items, color shifts for buttons) to provide immediate visual feedback to the user.

Visual Hierarchy: Styled text lines within nav items (like "Returns & Orders") with different font weights and colors to guide the user's eye to the most important information.

3. Cart Implementation
Two-Column Layout: Used a parent Flexbox container with align-items: flex-start to create a stable checkout experience where the Order Summary stays visible even when scrolling through items.

Nested Grid: Each cart item uses its own 2-column grid to keep product images and details perfectly aligned regardless of text length.

Vertical Cart Stack: Custom-aligned the cart right section to stack the quantity, icon, and label vertically for better visibility.

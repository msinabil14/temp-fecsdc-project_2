# Trail Runner Shoe - Product Detail Page

## Intuition

The goal of this project was to build a clean, modern, accessible, and responsive product detail page for an e-commerce website. I wanted to introduce user interactivity—such as selecting a product size and displaying an order confirmation.

## Approach

1. **Semantic HTML Structure**:
   - Used `<main>` and `<article>` tags to encapsulate the product card properly.
   - Employed `<fieldset>` and `<legend>` for grouping the product size radio options clearly for assistive technologies.

2. **Styling & CSS Interactivity**:
   - Built a two-column desktop layout using CSS Flexbox (`display: flex`) with proper alignment (`align-self: flex-start`, `object-fit: cover`).
   - Hidden native input elements (`<input type="radio">` and `<input type="checkbox">`) with `position: absolute` and `opacity: 0` to preserve accessibility and keyboard navigation (`:focus-visible`).
   - Styled associated `<label>` tags to look like interactive buttons, utilizing the `:checked + label` selector to highlight selected sizes.
   - Utilized a hidden checkbox (`#order`) combined with the general sibling selector (`#order:checked ~ .order-msg`) to show the "Order placed." feedback message when the "Buy Now" button is toggled.

3. **Responsiveness**:
   - Added a `@media (max-width: 700px)` breakpoint to stack the image and details vertically (`flex-direction: column`) on smaller screens for optimum mobile usability.

## User Guide:

- **How to use it**:
  - Keep `index.html` and `style.css` in the same directory.
  - Open `index.html` in any modern web browser or run it using VS Code Live Server.
  - can order the show with selecting size

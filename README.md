<h1 align="center">GrocerGo</h1>

![image](https://github.com/BhavdeepSinghNijhawan/GrocerGo/assets/143419096/efb219ee-3ac0-476d-b5a8-555b75081feb)

## LIVE URL

- https://grocery-shopping-website-theta.vercel.app/

## TECHNOLOGY STACK

### HTML

### CSS

#### src/PAGES/Auth/AuthPage.css

1. **Global Styles:**

- **`* { margin: 0; padding: 0; }:`** Resets margin and padding for all elements to ensure consistent styling.

2. **`.authpage:`**

- Sets up the main container for the authentication page (**`<div class="authpage">`**).
- Takes up the full width (**`width: 100%`**) and at least the full viewport height (min-height: 100vh).
- Has a white background (background-color: white) and is displayed as a flex container with a column layout (flex-direction: column).
.authcont:

Container for the authentication content.
Displayed as a flex container (display: flex) with items centered vertically (align-items: center).
Has a gap of 20px between its children (gap: 20px).
Takes 80% of the width (width: 80%) and 80vh of the viewport height (height: 80vh).
Applies a box shadow and rounded corners (box-shadow, border-radius) for a card-like appearance.
Is horizontally centered (margin: 0 auto) with top and bottom margins of 10%.
Has an overflow set to hidden to hide any overflowing content.
.authcont img:

Styles the image inside .authcont.
Width set to 50% of its container and height 100%.
Uses object-fit: cover to maintain aspect ratio and cover the entire container.
.authform:

Styles the form inside .authcont.
Displayed as a flex container with column layout (flex-direction: column).
Takes 50% of the width (width: 50%) of .authcont.
Adds padding (padding: 20px) and gap (gap: 5px) between child elements.
.authform h1, .authform label, .authform input, .authform button, .authform p, .authform .or:

Styles various elements inside .authform such as headings, labels, inputs, buttons, paragraphs, and "or" text.
Defines font sizes, weights, colors, padding, margins, and background colors for consistent styling across the form.
.form-group-row:

Styles a row of form elements.
Displayed as a flex container with a gap between items (gap: 10px).
Media Queries (@media):

Adjusts styles based on screen width to ensure responsiveness:
Max-width 1500px: Adjusts layout of .form-group-row to wrap items.
Max-width 1100px: Adjusts layout of .authcont, .authform, and their children for smaller screens, such as tablets.
Max-width 500px: Further adjusts layout for very small screens, such as mobile phones, making elements full-width and adjusting font sizes.

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)

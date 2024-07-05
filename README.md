<h1 align="center">GrocerGo</h1>

![image](https://github.com/BhavdeepSinghNijhawan/GrocerGo/assets/143419096/efb219ee-3ac0-476d-b5a8-555b75081feb)

## LIVE URL

- https://grocery-shopping-website-theta.vercel.app/

## TECHNOLOGY STACK

### HTML

### CSS

#### src/COMPONENTS/Banners/BannerSlider.css

1. **Container Styling:**

- **`.bannerslider:`** The main container for the banner slider, styled to take up the full width of its parent, hide overflow content, and position its child elements relatively.

2. **Image Container Styling:**

- **`.bannerslider .imagecont:`** The container for images within the banner slider, styled with a black background, flex layout, relative positioning, full width, and a height of 60% of the viewport.

3. **Image Styling:**

- **`.bannerslider .imagecont img:`** Images within the container are positioned absolutely to cover the entire container, maintaining their aspect ratio.

4. **Content Overlay Styling:**

- **`.bannerslider .imagecont .content:`** An overlay that centers content (text, buttons) within the image container. It has a semi-transparent black background, uses flexbox for layout, and centers its child elements both vertically and horizontally.

5. **Heading and Text Styling:**

- **`.bannerslider .imagecont h1:`** The heading within the overlay, styled with a specific font size, weight, margin, and width.
- **`.bannerslider .imagecont span:`** Additional text within the overlay, similarly styled but with slightly smaller font size and weight.

6. **Button Styling:**

- **`.bannerslider .imagecont button:`** Buttons within the overlay, styled with padding, no border, a white background, black text, rounded corners, a pointer cursor on hover, and a transition effect.

7. **Button Hover Effect:**

- **`.bannerslider .imagecont button:hover:`** On hover, the button background color changes to a custom variable color and the text color changes to white.

8. **Media Query for Smaller Screens:**

- **`@media (max-width: 768px):`** Adjusts styles for screens 768px wide or smaller. It reduces the height of the image container and adjusts the font sizes and widths of the heading, text, and button for better readability on smaller screens.

#### src/PAGES/Auth/AuthPage.css

1. **Global Styles:**

- **`* { margin: 0; padding: 0; }:`** Resets margin and padding for all elements to ensure consistent styling.

2. **`.authpage:`**

- Sets up the main container for the authentication page (**`<div class="authpage">`**).
- Takes up the full width (**`width: 100%`**) and at least the full viewport height (min-height: 100vh).
- Has a white background (background-color: white) and is displayed as a flex container with a column layout (flex-direction: column).

3. **`.authcont:`**

- Container for the authentication content.
- Displayed as a flex container (display: flex) with items centered vertically (align-items: center).
- Has a gap of 20px between its children (gap: 20px).
- Takes 80% of the width (width: 80%) and 80vh of the viewport height (height: 80vh).
- Applies a box shadow and rounded corners (box-shadow, border-radius) for a card-like appearance.
- Is horizontally centered (margin: 0 auto) with top and bottom margins of 10%.
- Has an overflow set to hidden to hide any overflowing content.

4. **`.authcont img:`**

- Styles the image inside .authcont.
- Width set to 50% of its container and height 100%.
- Uses object-fit: cover to maintain aspect ratio and cover the entire container.

5. **`.authform:`**

- Styles the form inside .authcont.
- Displayed as a flex container with column layout (flex-direction: column).
- Takes 50% of the width (width: 50%) of .authcont.
- Adds padding (padding: 20px) and gap (gap: 5px) between child elements.

6. **`.authform h1, .authform label, .authform input, .authform button, .authform p, .authform .or:`**

- Styles various elements inside .authform such as headings, labels, inputs, buttons, paragraphs, and "or" text.
- Defines font sizes, weights, colors, padding, margins, and background colors for consistent styling across the form.

7. **`.form-group-row:`**

- Styles a row of form elements.
- Displayed as a flex container with a gap between items (gap: 10px).

8. **Media Queries `(@media):`**

- Adjusts styles based on screen width to ensure responsiveness:
- Max-width 1500px: Adjusts layout of .form-group-row to wrap items.
- Max-width 1100px: Adjusts layout of .authcont, .authform, and their children for smaller screens, such as tablets.
- Max-width 500px: Further adjusts layout for very small screens, such as mobile phones, making elements full-width and adjusting font sizes.

#### src/PAGES/Auth/ForgotPassword.js

1. **Imports and Setup:**

- **`import React from 'react':`** Imports the React library, which is necessary for writing React components.
- **`{ Link } from 'react-router-dom':`** Imports the **`Link`** component from React Router, used for navigation between different routes in the application.
- **`import Navbar from '../../COMPONENTS/Navbar/Navbar':`** Imports a local **`Navbar`** component from a relative path **`(../../COMPONENTS/Navbar/Navbar)`**. Adjust the path based on the project structure.
- **`import './AuthPage.css':`** Imports a CSS file (AuthPage.css) for styling this component.

2. **Functional Component Definition:**

- **`const ForgotPassword = () => { ... }:`** Defines a functional component named **`ForgotPassword`**. This component is a stateless functional component that doesn't manage its own state or lifecycle methods.

3. **JSX Structure:**

- **`Outermost Container (<div className='authpage'>):`** Wraps the entire content of the component. Uses the class name `authpage` for styling purposes.
- **`Navbar Component (<Navbar reloadnavbar={false}/>):`** Renders a `Navbar` component with a prop `reloadnavbar` set to `false`.
- **`Authentication Content Container (<div className='authcont'>):`** Contains all the content related to authentication. Uses the class name `authcont` for styling.
- **`Image Element (<img src='...' alt='signup' />):`** Displays an image fetched from a URL. The `alt` attribute provides alternative text for accessibility.
- **`Form Element (<form className='authform'>):`** Starts a form with class name `authform` for styling.
- **Form Content:**
  - **`Heading (<h1>Forgot Password</h1>):`** Displays the title "Forgot Password".
  - **`Form Groups (<div className='formgroup'>):`** Contains form elements (`<label>` and `<input>`) for email, password, and confirm password fields.
  - **`Link to Login (<Link to='/login' className='stylenone'>):`** Renders a link to navigate to the Login page with text "Try Login again?".
  - **`Link to Signup (<Link to='/signup' className='stylenone'>):`** Renders a link to navigate to the Signup page with a `<button>` labeled "Verify".
  
4. **Exporting Component:**

- **`export default ForgotPassword:`** Exports the `ForgotPassword` component as the default export, making it available for use in other parts of the application.

This component (`ForgotPassword`) is designed to display a form for users to reset their password, along with navigation links to login or sign up for verification purposes. The structure follows typical React patterns, using JSX for rendering UI elements and React Router for navigation. Styling is applied through CSS classes imported from an external stylesheet (`AuthPage.css`).

#### src/PAGES/Auth/Login.js

1. **Imports and Author Comment:**

- The **`import`** statements bring in necessary modules (**`React`**, **`Link`** from React Router, **`Navbar`**, and the CSS file).

2. **Login Functional Component:**

- **`const Login = () => { ... }:`** Defines a functional component named Login using ES6 arrow function syntax.

3. **Return Statement (JSX):**

- **`return ( ... ):`** The component returns JSX, which describes the UI of the component.

4. **HTML Structure:**

- **`<div className='authpage'>:`** Outermost **`div`** with class **`authpage`** for styling purposes.
- **`<Navbar reloadnavbar={false}/>:`** Renders the **`Navbar`** component with **`reloadnavbar`** prop set to **`false`**.
- **`<div className='authcont'>:`** Inner **`div`** with class **`authcont`** for styling.

5. **Image:**

- **`<img src='...' alt='login' />:`** Displays an image sourced from the provided URL with alt text 'login'.

6. **Form:**

- **`<form className='authform'>:`** Form element with class **`authform`** for styling.

7. **Form Inputs and Labels:**

- **`<label htmlFor='email'>Email</label>:`** Label for email input.
- **`<input type='email' id='email' />:`** Email input field.
- **`<label htmlFor='password'>Password</label>:`** Label for password input.
- **`<input type='password' id='password' />:`** Password input field.

8. **Links (React Router):**

- **`<Link to='/forgotpassword' className='stylenone'>:`** Link to '/forgotpassword' with 'stylenone' class applied.
- **`<Link to='/' className='stylenone'>:`** Link to '/' (presumably home) with 'stylenone' class applied.
- **`<Link to='/signup' className='stylenone'>:`** Link to '/signup' with 'stylenone' class applied.

9. **Buttons and Headings:**

- **`<button className='btn'>Login</button>:`** Button with 'btn' class for styling.
- **`<h2 className='or'>OR</h2>:`** Heading 'OR' with 'or' class for styling.

10. **Export:**

- **`export default Login:`** Exports the **`Login`** component as the default export.

#### src/PAGES/Auth/Signup.js

1. **Imports and Component Definition:**

- The **`React library`** is imported to use React's functionality.
- **`Link`** is imported from **`react-router-dom`** to handle navigation between different routes without a full page reload.
- **`Navbar`** is imported from a relative path to include a navigation bar component.
- The stylesheet **`AuthPage.css`** is imported to style the components.

2. **Signup Component:**

- The **`Signup`** component is a functional component that returns a JSX structure.

3. **Main Container:**

- The **`div`** with the class **`authpage`** is the main container for the signup page.
- The Navbar`** component is included with a prop **`reloadnavbar={false}`**, which might control some behavior in the Navbar.

4. **Auth Container:**

- Another **`div`** with the class **`authcont`** contains the main content of the signup page.
- An image is displayed with a **`src`** attribute pointing to a URL and an **`alt`** attribute set to 'signup'.

5. **Form Structure:**

- A **`form`** element with the class **`authform`** is used to gather user input.
- The form contains an **`h1`** heading for the signup title.
- The first form group row contains two input fields for the first name and last name.
- The second form group contains an input field for the email.
- The third form group row contains two input fields for the password and confirm password.

6. **Links and Buttons:**

- A **`Link`** component is used to navigate to the login page with a paragraph indicating the option to navigate to the login page if the user already has an account.
- Another **`Link`** component is used for the signup button, although it links to the current page, making it redundant.

7. **Export:**

- The **`Signup`** component is exported as the default export of the module, allowing it to be imported and used in other parts of the application.

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)

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

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)

# Simple Login Page - Project Documentation

## Overview
This project is a modern, responsive login page built with HTML and CSS. It features a clean layout with an image section, a login form, and options for social login. The design is modular and easy to extend.

## File Structure
- `login.html` — Main HTML file containing the structure for the login UI.
- `style.css` — Stylesheet with all custom CSS for layout and components.
- (Optional) Image assets for logos and illustrations, referenced in the HTML.

## Layout & Components
- `.containers` — The main wrapper for the page, centers content and provides a card-like appearance.
- `.container-1` — Flex container holding the image (`.content-1`) and login form (`.content-2`).
- `.content-1` — Contains the main illustration and a clickable, underlined paragraph.
- `.content-2` — Contains the login form with floating label inputs, a submit button, and additional options.
- `.container-2` — Holds additional actions and social login options.
- `.CACT` — Section for underlined, centered action text (e.g., "Create Account").
- `.LoginUsing` — Row of social login icons (e.g., Facebook, Twitter), styled for alignment and spacing.

## Key CSS Patterns
- **Flexbox Layouts:** Used throughout for responsive, side-by-side and column layouts.
- **Floating Labels:** Inputs in `.content-2` use a floating label effect for a modern look.
- **Underline Inputs:** Username and password fields are styled with only an underline, no box.
- **Card Styling:** Main container uses box-shadow, padding, and border-radius for a card effect.
- **Centered and Underlined Text:** Utility classes and selectors (e.g., `.CACT p`, `.content-1 p`) provide centered, underlined, and clickable text.
- **Social Icons:** `.LoginUsing img` styles icons for consistent size and spacing.

## Customization & Extension
- To add more social login options, add `<img>` tags inside `.LoginUsing`.
- To change the main illustration, update the `<img>` in `.content-1`.
- To add more actions (like "Forgot Password?"), use the `.CACT` section.

## Example Usage
```html
<div class="containers">
  <div class="container-1">
    <div class="content-1">
      <img src="your-image.png" alt="Login Illustration">
      <p>Some underlined, clickable text</p>
    </div>
    <div class="content-2">
      <h2>Login</h2>
      <form>
        <!-- Floating label input wrappers here -->
        <button type="submit">Login</button>
      </form>
    </div>
  </div>
  <div class="container-2">
    <div class="CACT">
      <p>Create Account</p>
    </div>
    <div class="LoginUsing">
      <span>Login using:</span>
      <img src="facebook.png" alt="Facebook">
      <img src="twitter.png" alt="Twitter">
    </div>
  </div>
</div>
```

## Notes
- All layout and component classes are defined in `style.css`.
- Adjust `min-width` and `min-height` in `.containers` and `.container-1` for different screen sizes.
- Use semantic HTML and keep content modular for easy updates.

---
Update this documentation as you add new features or change the structure.

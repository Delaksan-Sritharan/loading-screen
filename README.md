

# Loading Screen

This project demonstrates a basic loading screen using HTML and CSS. It displays a centered message with a spinning animation to indicate that something is in progress.

## Preview

<img width="1440" alt="Screenshot 2025-05-13 at 9 18 08 AM" src="https://github.com/user-attachments/assets/bba45bef-3e72-49f7-b0df-6634b813ff62" />

## Files

* `index.html`: The HTML structure for the loading screen.
* `style.css`: The CSS styles to center the content and create the spinning animation.

## How to Use

1.  Save the HTML code as `index.html`.
2.  Save the CSS code as `style.css` in the same directory as `index.html`.
3.  Open `index.html` in your web browser.

You will see a centered message "For new sidebar colors, click your workspace then Preference > Sidebar > Theme" with a smaller attribution below and a spinning circle.

## Explanation

### `index.html`

* Sets up the basic HTML structure with a title "Loading Screen".
* Links the `style.css` file for styling.
* Contains a `<section>` element with the class `loading` to hold the loading message and animation.
* Inside the `loading` section:
    * The main loading message is displayed as plain text.
    * A `<span>` with the class `loading__author` displays the attribution.
    * A `<span>` with the class `loading__anim` creates the spinning circle.

### `style.css`

* **`body`**:
    * `display: flex;`: Uses Flexbox for easy centering.
    * `justify-content: center;`: Centers content horizontally.
    * `align-items: center;`: Centers content vertically.
    * `min-height: 100vh;`: Ensures the body takes up at least the full viewport height.
* **`.loading`**:
    * `max-width: 50%;`: Sets a maximum width for the loading message container.
    * `line-height: 1.4;`: Improves readability of the text.
    * `font-size: 1.2rem;`: Sets a slightly larger font size for the main message.
    * `font-weight: bold;`: Makes the main message text bold.
    * `text-align: center;`: Centers the text within the container.
* **`.loading__author`**:
    * `font-weight: normal;`: Sets the author text to normal weight.
    * `font-size: 0.9rem;`: Makes the author text smaller.
    * `color: rgba(189,189,189,1);`: Sets the author text to a light gray color.
    * `margin: 0.6rem 0 2rem 0 ;`: Adds top, bottom, and no left/right margins for spacing.
    * `display: block;`: Makes the author text a block-level element, placing it on a new line.
* **`.loading__anim`**:
    * `width: 35px;`: Sets the width of the spinning circle.
    * `height: 35px;`: Sets the height of the spinning circle.
    * `display: inline-block;`: Allows the circle to be inline with text but with block-level properties like width and height.
    * `border: 5px solid rgba(189,189,189,0.25);`: Creates a gray border with some transparency.
    * `border-left-color: rgba(3,155,229,1);`: Sets the left border color to blue.
    * `border-top-color: rgba(3,155,229,1);`: Sets the top border color to blue.
    * `border-radius: 50%;`: Makes the element a circle.
    * `animation: rotate 600ms infinite linear;`: Applies the `rotate` animation.
* **`@keyframes rotate`**:
    * Defines the `rotate` animation.
    * `to { transform: rotate(360deg); }`: Rotates the element 360 degrees.
    * `600ms`: Sets the duration of one animation cycle to 600 milliseconds.
    * `infinite`: Makes the animation loop continuously.
    * `linear`: Makes the animation progress at a constant speed.

This simple loading screen can be easily integrated into your web projects to provide visual feedback to users while content is loading in the background. You can customize the message, colors, and animation to match your project's design.

Try a hard refresh (Ctrl+F5 or Cmd+Shift+R)

License
MIT License - Free for personal and commercial use

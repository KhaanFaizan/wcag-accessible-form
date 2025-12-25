# WCAG 2.1 AA Compliant Form Project

## Overview

This project serves as a practical demonstration of how to build web pages that strictly adhere to the Web Content Accessibility Guidelines (WCAG) 2.1 AA standards. It was designed to show that accessibility does not require complex frameworks or heavy tooling—just semantic HTML and thoughtful coding practices.

The focus here is entirely on structural integrity and assistive technology support. While the visual design is minimal, the underlying code ensures that users relying on screen readers, keyboard navigation, or other assistive tools have a first-class experience.

## Project Structure

Inside this repository, you will find three main pages:

*   **index.html**: The main sign-up page. It demonstrates accessible form validation, error handling, and the use of "honey pot" fields to prevent spam without interfering with legitimate users.
*   **thank-you.html**: A confirmation page that shows proper heading hierarchy and how to handle both meaningful and decorative images.
*   **events.html**: An events calendar listing that uses native HTML elements like `details` and `summary` to create interactive content that works perfectly with keyboards.

## Technical Note: Embedded JavaScript

You might notice there are no external `.js` files in this project. All necessary JavaScript logic (for form validation and alerts) is **lightweight and embedded directly** within `index.html`.

This design choice was made to:
1.  **Simplify deployment**: Just copy the HTML files, and it works.
2.  **Improve performance**: Reduces the number of HTTP requests.
3.  **Keep it self-contained**: Makes the code easier to review in a single file.

## Accessibility Features

We have implemented several key techniques to ensure compliance:

*   **Semantic HTML**: We use standard tags like `header`, `nav`, `main`, and `article` to give the page a meaningful structure that screen readers can navigate easily.
*   **Keyboard Navigation**: Every interactive element can be reached and operated using only a keyboard. Focus states are clearly visible.
*   **ARIA Labels**: When visual cues aren't enough, we use ARIA (Accessible Rich Internet Applications) attributes to provide context to blind users (e.g., announcing when a form has errors).
*   **Live Regions**: The form uses a "live region" to announce status updates immediately, so users know if their submission was successful or if they need to fix errors.

## How to Run

Since this is a static HTML/CSS project, you do not need to install any dependencies.

1.  Simply download or clone this folder.
2.  Open `index.html` in any modern web browser.

## Testing for Accessibility

If you want to verify the accessibility features yourself:

*   **Try navigating without a mouse**: Use the `Tab` key to move through links and form fields. Ensure you can see where you are at all times.
*   **Listen with a Screen Reader**: If you have tools like NVDA (Windows) or VoiceOver (Mac), turn them on and try to sign up. You should hear clear labels for every field and immediate feedback if you make a mistake.

## License

This project is open for educational use. Feel free to use it as a template for your own accessible web applications.

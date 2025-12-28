# daisyui-theme-arc

A faithful Arc Dark theme for daisyUI, inspired by the classic GTK Arc theme.

This project provides a CSS-only daisyUI theme using OKLCH colors.
No JavaScript configuration is required.

Included theme:
- arc-dark

---

## Requirements

- Tailwind CSS
- daisyUI

This repository only provides a custom theme file.
It does not install or configure Tailwind or daisyUI for you.

---

## Installation

### 1. Copy the theme file

Copy `arc-dark.css` into your project, for example:

src/styles/arc-dark.css

### 2. Import it in your main Tailwind CSS file

In your main CSS entry file (for example `app.css`, `main.css`, or `input.css`):

@import "tailwindcss";
@plugin "daisyui";

/* Import Arc Dark theme */
@import "./arc-dark.css";

---

## Usage

Enable the theme by setting `data-theme="arc-dark"`.

On the root element:

<html data-theme="arc-dark">
  ...
</html>

Or on a specific container:

<div data-theme="arc-dark">
  ...
</div>

---

## Customization

Open `arc-dark.css` and adjust the OKLCH variables as needed.

Common tweaks:

- --color-base-content for text readability
- --color-base-100, --color-base-200, --color-base-300 for surface contrast
- --color-primary for the Arc accent blue

The Arc look relies on subtle contrast and low saturation.
Small changes usually work better than large shifts.

---

## Notes on text colors

In daisyUI, text-secondary uses --color-secondary rather than
--color-secondary-content.

Because this theme uses secondary as a surface color,
you may prefer to use base-content or opacity-based utilities
for secondary or muted text.

---

## License

MIT License.
See the LICENSE file for details.

---

## Credits

Inspired by the classic Arc Dark GTK theme.
Built for the daisyUI theming system.

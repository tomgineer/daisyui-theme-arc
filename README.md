# daisyui-theme-arc

A faithful Arc Dark theme for daisyUI, inspired by the classic GTK Arc theme.

This repository provides a CSS-only daisyUI theme using OKLCH color tokens.
No JavaScript configuration is required.

## Preview

![Arc Dark theme mockup](./arc-dark-mockup.png)

## Included themes

- arc-dark

## Requirements

- Tailwind CSS
- daisyUI

This repository only provides a theme file. It does not install or configure Tailwind or daisyUI for you.

## Installation

### 1. Copy the theme file into your project

Copy `arc-dark.css` into your project, for example:

```text
src/styles/arc-dark.css
```

### 2. Import the theme in your main Tailwind CSS file

In your main CSS entry file (for example `app.css`, `main.css`, or `input.css`):

```css
@import "tailwindcss";
@plugin "daisyui";

/* Import Arc Dark theme */
@import "./arc-dark.css";
```

## Usage

Enable the theme by setting `data-theme="arc-dark"`.

On the root element:

```html
<html data-theme="arc-dark">
  ...
</html>
```

Or scope it to a container:

```html
<div data-theme="arc-dark">
  ...
</div>
```

## Customization

Open `arc-dark.css` and adjust the OKLCH variables as needed.

Common tweaks:

- `--color-base-content` for text readability
- `--color-base-100`, `--color-base-200`, `--color-base-300` for surface contrast
- `--color-primary` for the Arc accent color

The Arc look relies on subtle contrast and low saturation. Small changes usually work better than large shifts.

## Notes on text colors

In daisyUI, `text-secondary` uses `--color-secondary` rather than `--color-secondary-content`.

Because this theme uses `secondary` as a surface color (similar to Arc), you may prefer:

- `text-base-content` for readable secondary text, or
- opacity-based utilities for muted text (for example, 70 percent or 50 percent opacity).

## License

MIT License. See the `LICENSE` file for details.

## Credits

Inspired by the classic Arc Dark GTK theme.
Built for the daisyUI theming system.

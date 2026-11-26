# CTU Naga Campus Website

A simple campus information website made with HTML and CSS.

## Project files

- `index.html` contains the words, pictures, links, and sections on the page.
- `style.css` controls the colors, spacing, sizes, and page layout.
- `images` contains the CTU logo and campus banner.

## How to change the website

- To change a heading or paragraph, edit the text in `index.html`.
- To change a color, open the `:root` section at the top of `style.css`.
- To change the layout or sizes, edit the matching section in `style.css`.

## Understanding the colors

The color names beginning with `--` are CSS variables. They store the color codes in one place.

For example:

```css
:root {
    --navy: #14264d;
}
```

Use the color with `var()`:

```css
header {
    background-color: var(--navy);
}
```

You do not need to remember the number. Remember the name `--navy`. CSS gets the color code from `:root`.

## Position properties used in this project

- `static` keeps an element in its normal page position.
- `relative` keeps an element in the normal page flow and lets positioned children use it as their reference.
- `absolute` positions an element using its nearest positioned parent. The welcome label uses this.
- `fixed` keeps an element in the same place on the screen while scrolling. The back-to-top button uses this.

## Mobile layout

The `@media (max-width: 600px)` section changes some sizes and spacing on screens that are 600 pixels wide or smaller.

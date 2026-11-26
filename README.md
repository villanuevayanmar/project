# CTU Naga Campus Website

A simple campus information website made with **HTML and CSS**.

Live website: https://villanuevayanmar.github.io/villanueva-yanmar/

## 1. Project files

| File or folder | What it is for |
|---|---|
| `index.html` | The page content: headings, paragraphs, pictures, navigation, and sections. |
| `style.css` | The design: colors, text sizes, spacing, borders, and layout. |
| `images/ctu-logo.jpg` | The CTU logo shown in the header. |
| `images/campus-banner.jpg` | The campus image shown in the welcome section. |

The website does not use JavaScript or a database. It is a static website, which means its content is written directly in the HTML file.

## 2. What is already on the website?

- **Header:** CTU logo and campus name.
- **Navigation:** links to Home, About, Campus News, and Student Services.
- **Welcome:** a welcome message and campus banner.
- **About:** a short introduction to the campus.
- **Campus News:** two general announcement examples.
- **Student Services:** information about the Registrar, Library, and Computer Laboratory.
- **Upcoming Events:** two general event examples.
- **Footer:** campus name and website description.
- **Top link:** returns the visitor to the Home section.

## 3. What is still missing or needs checking?

These are things to finish or confirm. They are not features that have already been built.

| Missing or unfinished item | What needs to be done | Where to edit |
|---|---|---|
| Events navigation link | Add an **Events** link so visitors can jump to the Upcoming Events section. The section already exists. | `index.html` |
| Real campus announcements | Replace the general examples with actual announcements, dates, and details confirmed by the campus. | `index.html`, inside `id="news"` |
| Real event schedules | Replace "To be announced" when official event dates and details are available. | `index.html`, inside `id="events"` |
| Complete campus information | Confirm whether the About section needs more accurate campus details. | `index.html`, inside `id="about"` |
| Student service details | Add confirmed office locations, office hours, or contact details if required. | `index.html`, inside `id="services"` |
| Contact information | Add an official campus contact method if one is available and required. | `index.html` and `style.css` |

**Important:** Do not invent announcements, event dates, office hours, addresses, or contact details. Use information confirmed by the campus.

The website currently has no login, admin panel, search, contact form, live news feed, or database. Changes to text and pictures must be made in the project files. These features are not part of the current simple version.

## 4. How to edit the website

### Change words or headings

1. Open `index.html`.
2. Find the heading or paragraph you want to change.
3. Replace only the text between the HTML tags.

Example:

```html
<h2>Welcome to CTU Naga Campus</h2>
```

Change the words inside the tags. Keep the opening and closing tags.

### Change a color or design

1. Open `style.css`.
2. Find the section you want to change, such as `/* Header */` or `/* Navigation */`.
3. Change the CSS value.

This project uses named CSS colors, so you can write names such as:

- `navy`
- `darkred`
- `gold`
- `white`
- `black`
- `ivory`
- `lightgray`

Example:

```css
header {
    background: navy;
    color: white;
}
```

You do not need to memorize hexadecimal color numbers for these colors.

### Change an image

The image locations are written in `index.html`:

```html
<img src="images/ctu-logo.jpg" alt="Cebu Technological University logo">
```

Keep the image in the `images` folder and make sure its filename matches the `src` value. If you change the filename, update the HTML too.

## 5. CSS properties used in this project

| CSS property | Simple meaning |
|---|---|
| `background` | Sets the background color. |
| `color` | Sets the text color. |
| `padding` | Adds space inside an element. |
| `margin` | Adds space outside an element. |
| `width` | Sets the element's width. |
| `font-size` | Changes the text size. |
| `text-align` | Aligns text, such as center or left. |
| `display: flex` | Places items in a flexible row or layout. |
| `gap` | Adds space between flex items. |
| `border` | Adds a line around an element. |

## 6. Positioning used in this project

- **Static:** the default position. An element stays in the normal page order. Most elements use this.
- **Relative:** keeps an element in the normal page order and makes it a reference point for an absolutely positioned child. The `.welcome` section uses this.
- **Absolute:** positions an element inside its nearest positioned parent. The welcome label uses this.
- **Fixed:** keeps an element in the same place on the screen while scrolling. The Top link uses this.

Example from the project:

```css
.welcome {
    position: relative;
}

.welcome-label {
    position: absolute;
}
```

The welcome section is the reference point for the welcome label.

## 7. Mobile layout

At the bottom of `style.css`, this rule applies styles to screens that are 600 pixels wide or smaller:

```css
@media (max-width: 600px) {
    /* Mobile styles are written here. */
}
```

It makes some text and spacing smaller and makes each card use the full available width.

## 8. Before submitting the website

- [ ] Check that the CTU logo and campus banner appear.
- [ ] Check every navigation link.
- [ ] Add an Events navigation link.
- [ ] Replace example announcements with confirmed campus information.
- [ ] Add real event schedules when available.
- [ ] Confirm the campus and student service information.
- [ ] Open the live website on both a phone and a computer.

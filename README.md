# website_demo

A collection of small, static HTML/CSS/JavaScript UI demos: a fixed navigation menu, a full-width slider, a testimonial carousel, parallax sections, hover effects and more. It started as a landing-page prototype for an "MBO Platform" site and works as a snippet library you can copy from.

No build step and no backend. Open the HTML files in a browser.

## What's inside

| File | Demo |
|---|---|
| `index.html` | Landing page: fixed navbar with a mobile toggle, hero slider, and content sections |
| `slider.html` | Standalone hero slider |
| `testimonial.html` | Testimonial carousel (Owl Carousel) |
| `Button.html` | Button style experiments |
| `accordianStyle2.html`, `accordian4Service.html` | Accordion variants |
| `iconsNText.html` | Icon and text blocks |
| `squareGrid.html` | Square grid layout |
| `parallaxBg.html` | Parallax background section |
| `razorBladDiv.html` | Slanted ("razor blade") section dividers |
| `textHover.html` | Hover text effect ("WhyUS" heading) |
| `textNelement.html` | Header with left/right icon-and-text blocks |
| `footer.html` | Footer layout |
| `index.php` | One-line redirect to `/index.html` (for PHP hosts) |

## Built with

- HTML5 and CSS3 (custom styles in `css/style.css`, `css/slider.css`, `css/testimonial.css`)
- [jQuery](https://jquery.com/) (bundled as `js/jquery.min.js`)
- [Owl Carousel](https://owlcarousel2.github.io/OwlCarousel2/) (`css/owl.*`, `js/owl.carousel.min.js`)
- [Font Awesome](https://fontawesome.com/v4/) 4 icons (`css/font-awesome.min.css`, `fonts/`)

## Run it locally

Just open `index.html` in a browser. To serve it over HTTP (recommended, so fonts and relative paths behave like production):

```bash
# any one of these, from the repo root
python3 -m http.server 8000
npx serve .
php -S localhost:8000
```

Then visit `http://localhost:8000`.

## Project structure

```
website_demo/
├── index.html              Main landing page
├── *.html                  One file per component demo
├── css/                    Stylesheets (site styles + vendor CSS)
├── js/
│   ├── menu.js             Toggles the mobile menu (.menu.show)
│   ├── slider.js           Hero slider behaviour
│   ├── testimonial.js      Testimonial carousel setup
│   └── jquery.min.js, owl.carousel.min.js   Vendored libraries
├── fonts/                  Font Awesome font files
├── images/                 Image assets
└── index.php               Redirect to index.html
```

## Reusing a component

1. Open the demo file for the component (for example `slider.html`).
2. Copy its markup into your page.
3. Copy the matching rules from `css/` and the script from `js/`, and keep the same load order: jQuery first, then plugins, then your own script.

## Notes and limitations

- The page copy is placeholder text (Lorem ipsum, "Project name 1") and the logo area is empty. Replace it with your own content.
- Menu links in `index.html` point to `#`; wire them to real sections or pages.
- Some demos set no `<title>`; add one if you publish them.
- Libraries are vendored, not installed from npm, so they will not update automatically.

## Author

[Manoj Mallick](https://github.com/manojmallick)

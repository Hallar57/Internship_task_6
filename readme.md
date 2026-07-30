# whitepace landing page

A responsive landing page built with Bootstrap 5, based on a Figma design across 5 widths (320px, 768px, 1152px, 1400px, 1920px).

## How to view it

Just open `index.html` in any browser (double click it, or right click and choose "Open with" your browser). No install needed, it pulls Bootstrap from a CDN link, so you'll need an internet connection for the styling to load.

## Folder structure

```
whitepace/
├── index.html
├── README.md
└── images/
    ├── logo.svg
    ├── element.png
    ├── avatar1.jpg
    ├── avatar2.jpg
    ├── avatar3.jpg
    └── (hero, sponsor, and other section images)
```

Create the `images` folder next to `index.html` and drop your exported files in there.

## Images still needed

These are currently placeholder boxes or icons in the code:

- Logo (navbar and footer)
- Hero image
- Project Management section image
- Use as Extension section image
- Customise it to your needs section image
- Sponsor logos (Apple, Microsoft, Slack, Google)
- 3 testimonial avatar photos

## Swapping a placeholder for a real image

Find the placeholder line, it looks like this:

```html
<div class="placeholder-box w-100" style="aspect-ratio: 4/3;"></div>
```

Replace it with an image tag pointing to your file:

```html
<img src="images/yourfile.png" alt="describe the image here" class="w-100 rounded">
```

## Notes

- The navy color is a custom CSS variable (`--wp-navy`) since it isn't a default Bootstrap color.
- Everything else uses standard Bootstrap classes, so changing spacing or layout is mostly a matter of swapping class names (like `col-lg-6` to `col-lg-4`) rather than writing new CSS.
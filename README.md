# GATOS-ASTRO - A Website for GATOS

---

This repository hosts the content of the official
[GATOS website](https://gatos-astro.com).

## Repository structure

The structure of this repository is as follows:

```text.
.
├── .vale.ini                   # Configuration file for vale linting
├── docs                        # All website page files
│   ├── CNAME                   # Custom domain configuration
│   ├── *.html                  # HTML files for the website pages
│   ├── images                  # Website images
│   │   ├── collaborations      # Images used by collaborations.html
│   │   ├── logo_cropped.png    # GATOS logo for the navigation bar
│   │   ├── news                # Images used by news.html
│   │   └── *.jpg               # Images used by gallery.html
│   └── style.css               # CSS styling for the website
├── LICENSE                     # MIT license for this repository
└── README.md                   # Repository documentation
```

## Maintenance

Changes to the website can be made by editing the HTML and CSS files, or by
adding, removing, or replacing documents linked from the HTML pages. The CSS file
contains comments describing the major styling rules. The annotated template
below shows the HTML structure shared by the main website pages. Page-specific
content should be placed inside the `<main>` element.

```html
<!-- Set document language -->
<html lang="en">
  <!-- Webpage head -->
  <head>
    <!-- Set character set to UTF-8 -->
    <meta charset="UTF-8" />

    <!-- Set website scaling for different screen sizes -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <!-- Page title; replace [page name] with the name of the page, e.g., "Home" -->
    <title>[page name] - GATOS</title>

    <!-- Load fonts -->
    <link
      href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Source+Sans+3:wght@400;500;600&display=swap"
      rel="stylesheet"
    />

    <!-- Load CSS stylesheet -->
    <link rel="stylesheet" href="style.css" />
  </head>

  <!-- Webpage body -->
  <body>
    <!-- Webpage header -->
    <header>
      <!-- GATOS logo and text in the header -->
      <div class="logo">
        <img src="images/logo_cropped.png" alt="GATOS" class="logo" />
        <span class="logo-text">GATOS</span>
      </div>

      <!--
      Navigation bar. The current page or section is marked using
      class="active" on the relevant <a> element.
      -->
      <nav>...</nav>
    </header>

    <!-- Page-specific content -->
    <main></main>

    <!-- Footer -->
    <footer>&copy; GATOS 2026</footer>
  </body>
</html>
```

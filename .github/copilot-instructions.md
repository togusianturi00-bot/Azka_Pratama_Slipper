# Workspace instructions

## Project overview
- The website source is in the `eBusiness/` subdirectory of this workspace. It is a static, multi-page Bootstrap 5.3.6 corporate website based on the BootstrapMade eBusiness template.
- There is no package manifest or build/test configuration. HTML pages load CSS and JavaScript directly from `eBusiness/assets/`.
- Main pages: `eBusiness/index.html`, `eBusiness/portfolio-details.html`, `eBusiness/service-details.html`, and `eBusiness/starter-page.html`. `eBusiness/index-old.html` is an older page; do not treat it as the primary homepage unless requested.

## Architecture and assets
- `eBusiness/assets/css/main.css` contains site styles and theme variables. Prefer using existing CSS variables and component conventions; avoid editing minified vendor CSS.
- `eBusiness/assets/js/main.js` contains shared site interactions and initializes global libraries loaded from `eBusiness/assets/vendor/` (Bootstrap, AOS, PureCounter, Swiper, GLightbox, imagesLoaded, and Isotope).
- Images are in `eBusiness/assets/img/`; keep references relative to each HTML page.
- Contact and newsletter forms post to PHP files in `eBusiness/forms/`. Their PHP Email Form dependency is not included (the form README notes it is available with the template's pro version), and the contact recipient is a placeholder. Do not claim these forms send email without configuring and providing that dependency.

## Working conventions
- Keep page markup semantic and responsive, following the existing Bootstrap grid and template structure.
- Shared changes that affect multiple pages should be applied consistently to all relevant HTML pages.
- Preserve BootstrapMade attribution and licensing notices. Do not remove or replace vendor assets unless explicitly requested.
- Use the existing local assets and libraries before introducing new dependencies. Avoid adding a build system for simple static-site changes.
- For validation, inspect changed HTML/CSS/JavaScript and check local asset paths. No automated test or build command is currently configured. PHP form behavior requires a PHP-capable server and the missing PHP Email Form library.

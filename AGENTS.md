## Architecture

This is a simple static-pages project. No build step, no framework.

- Each page is a single self-contained `.html` file (inline `<style>` in the `<head>`, no separate CSS files unless a page grows large enough to need one).
- No JavaScript unless the task explicitly asks for interactivity.
- New pages go in the repo root, named after their content in lowercase-with-hyphens (e.g. `waterford-ireland.html`).
- `home.html` is the site index: a simple list of links to every other page. Whenever a new page is created, add a link to it in `home.html` in the same task -- don't leave pages orphaned.

## Conventions

**CSS class names:** lowercase, hyphen-separated (kebab-case), prefixed by the page/section they belong to.

- Good: `hero-title`, `about-section`, `contact-form-input`
- Bad: `HeroTitle`, `about_section`, `input1`

**Structure inside a page:**
- Use semantic HTML tags (`<header>`, `<main>`, `<section>`, `<footer>`) over generic `<div>` soup where reasonable.
- Keep inline styles in one `<style>` block in `<head>`, not scattered `style=""` attributes, unless it's a one-off tweak.

## Change log

- Added `winterfell-fest.html` page for Winterfell Fest in Waterford, Ireland.
- Created `home.html` and added a link to the Winterfell Fest page.
- Added `waterford-ireland.html` page for the GAA in Waterford, Ireland.
- Updated `home.html` with a link to the new page.
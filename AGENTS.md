# AGENTS.md

## Architecture

This is a simple static-pages project. No build step, no framework.

- Each page is a single self-contained `.html` file (inline `<style>` in the `<head>`, no separate CSS files unless a page grows large enough to need one).
- No JavaScript unless the task explicitly asks for interactivity.
- New pages go in the repo root, named after their content in lowercase-with-hyphens (e.g. `waterford-ireland.html`).

## Conventions

**CSS class names:** lowercase, hyphen-separated (kebab-case), prefixed by the page/section they belong to.

- Good: `hero-title`, `about-section`, `contact-form-input`
- Bad: `HeroTitle`, `about_section`, `input1`

**Structure inside a page:**
- Use semantic HTML tags (`<header>`, `<main>`, `<section>`, `<footer>`) over generic `<div>` soup where reasonable.
- Keep inline styles in one `<style>` block in `<head>`, not scattered `style=""` attributes, unless it's a one-off tweak.

## Change log

(Agent: append a one-line entry below after each completed task -- what page/file, what it does. Keep it factual, no restating these conventions.)

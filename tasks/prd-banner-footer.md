# PRD: Banner and Footer UI Enhancement

## Introduction

Add a visible header banner and dynamic footer to the Hello World practice app. The banner identifies this as a practice app built with Amp + Ralph, while the footer displays the current year dynamically using JavaScript.

## Goals

- Display a clear identification banner at the top of the page
- Show a footer with the dynamically generated current year
- Keep changes minimal, safe, and easy to review
- Avoid touching build/deploy configuration

## User Stories

### US-001: Add header banner
**Description:** As a visitor, I want to see a banner at the top of the page so I know this is a practice app built with Amp + Ralph.

**Acceptance Criteria:**
- [ ] Banner appears at the very top of the page (above existing content)
- [ ] Banner text reads: "Practice App – built with Amp + Ralph"
- [ ] Banner is visually distinct (e.g., background color, centered text)
- [ ] Banner is responsive and readable on mobile
- [ ] Verify in browser

### US-002: Add dynamic year footer
**Description:** As a visitor, I want to see a footer at the bottom of the page showing the current year so I know the site is maintained.

**Acceptance Criteria:**
- [ ] Footer appears at the bottom of the page
- [ ] Footer displays the current year (e.g., "© 2025")
- [ ] Year is generated dynamically via JavaScript (not hardcoded)
- [ ] Footer is styled consistently with the page
- [ ] Verify in browser

## Functional Requirements

- FR-1: Add a `<header>` or `<div>` element at the top of `<body>` containing the banner text
- FR-2: Style the banner with a background color and centered text in `css/style.css`
- FR-3: Add a `<footer>` element at the bottom of `<body>` with a placeholder for the year
- FR-4: In `js/main.js`, insert the current year into the footer using `new Date().getFullYear()`
- FR-5: Style the footer to match page aesthetics in `css/style.css`

## Non-Goals

- No navigation links in the banner or footer
- No build or deploy configuration changes
- No additional pages or routes
- No external dependencies or libraries

## Technical Considerations

- Modify only: `index.html`, `css/style.css`, `js/main.js`
- Use semantic HTML elements (`<header>`, `<footer>`)
- JavaScript should run after DOM is ready (file already loads at end of body)

## Success Metrics

- Banner is visible immediately on page load
- Footer displays correct current year
- No console errors
- Page remains fully functional

## Open Questions

None – scope is intentionally minimal.

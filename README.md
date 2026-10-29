# Navya T — Illustrated Daydream Portfolio

A dreamy, illustrated personal portfolio for **Navya T**, a second-year Computer Science and Engineering student at Jawaharlal College of Engineering and Technology (JCET), Palakkad, Kerala.

The website combines a warm journal aesthetic with a developer portfolio, using sage green, warm ivory, dusty pink, butter yellow, and muted lavender.

## Features

- Responsive layout for desktop, tablet, and mobile.
- Illustrated hero section with subtle floating decorations.
- About me and education timeline.
- Learning-focused skills and interests.
- Music journal with mood-based sections and configurable playlist links.
- Travel postcards with sample destinations clearly labelled as inspiration.
- Project gallery with placeholder projects until real projects are added.
- Accessible mobile navigation with a hamburger menu.
- Reveal-on-scroll animations and reduced-motion support.
- Contact form with required-field and email validation. It opens a pre-filled email draft through the visitor's default email application; it does **not** send email automatically.
- SEO title and meta description.
- HTML, CSS, and JavaScript combined in one file.

## Files

```text
navya-portfolio/
└── index.html
```

Save the website code as `index.html`. This project does not require a build step or package installation.

## Run locally

1. Download or save `index.html` to a folder.
2. Open `index.html` in a modern browser.
3. To edit the website, open the file in a code editor such as VS Code and update the HTML, CSS, or JavaScript.

An internet connection is needed to load the Google Fonts included in the page. If unavailable, the website uses system fallback fonts.

## Personalisation

Near the bottom of `index.html`, find the `SITE_CONFIG` object:

```javascript
const SITE_CONFIG = {
  email: "YOUR_EMAIL@example.com",
  links: {
    github: "",
    linkedin: "",
    instagram: "",
    music1: "",
    music2: "",
    music3: ""
  }
};
```

Update these values:

- `email`: Navya's real email address.
- `github`, `linkedin`, `instagram`: real social profile URLs.
- `music1`, `music2`, `music3`: real playlist URLs.

Use full URLs, including `https://`. Leave a link empty until the real URL is available. The contact form will not prepare an email draft until a valid recipient email address is configured.

### Updating website content

- **About and education:** Edit the text in the matching sections in `index.html`.
- **Skills:** Change the labels in the Skills section to reflect current learning interests.
- **Music:** Edit the mood tiles, playlist titles, descriptions, and configured playlist URLs.
- **Travel:** Replace sample inspiration postcards with real destinations or memories. Update the labels so they accurately reflect their status.
- **Projects:** Replace placeholder titles, descriptions, technologies, and links only when actual projects and URLs are available.
- **Colours and layout:** Edit the CSS variables at the top of the `<style>` block.

## Contact form behaviour

The contact form:

1. Checks that all fields are filled in.
2. Validates the visitor's email address format.
3. Builds a `mailto:` link with the configured recipient, subject, and message.
4. Opens the visitor's email application with a draft, where the visitor must press **Send**.

The form does not use a backend service and does not transmit or store messages itself. Some devices may not have a default email application configured.

## Accessibility and responsiveness

- Semantic page sections and labelled form fields.
- Accessible menu state via `aria-expanded` and descriptive labels.
- Keyboard support for closing the mobile menu with Escape.
- Visible focus styling on form inputs.
- Reduced-motion preference support.
- Responsive layouts and mobile-friendly touch targets.

## Publishing

This is a static website and can be hosted by any service that supports static HTML, such as GitHub Pages, Netlify, or Cloudflare Pages.

For a simple deployment, upload `index.html` as the site's entry page. Before publishing, configure the email address and any real social or playlist links, and replace placeholder content as appropriate.

## Customisation notes

- The avatar and decorative artwork are created with CSS and emoji, so no local image assets are required.
- Google Fonts are loaded externally; system fallback fonts are provided.
- Placeholder projects and travel destinations are intentionally not presented as verified achievements or visited places.

## Credits

Created as a personal student portfolio concept for Navya T.

**Made with curiosity and a little daydream.**

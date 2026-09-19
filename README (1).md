# Terra Bloom Community Garden Website

A 4-page HTML5 website built for a fictional community garden organization, created to demonstrate mastery of semantic HTML structure, navigation, tables, and forms.

## Theme

The site represents **Terra Bloom Community Garden**, a fictional volunteer-run community garden focused on sustainable growing, environmental education, and bringing neighbors together. The site includes a home page introducing the garden, an about page sharing its story, a services/projects page listing programs offered, and a contact page for inquiries.

## File Organization

```
terra-bloom-website/
│
├── index.html          # Home page — intro articles about garden programs
├── about.html           # About page — mission, story, and figure/caption
├── services.html        # Services/Projects page — table of programs offered
├── contact.html         # Contact page — inquiry form
│
└── images/              # (optional) local image assets, if not using external URLs
```

All four HTML pages live in the root folder so that relative links (e.g. `href="about.html"`) resolve correctly both locally and when hosted on GitHub Pages. Each page shares an identical `<header>` and `<nav>` menu for consistent site-wide navigation.

## Challenges Faced

- **Broken navigation links:** Early on, clicking "Home" from other pages returned a "failed to load" error. This turned out to be a filename/case-sensitivity mismatch between the link (`href="index.html"`) and the actual file — a good reminder that relative paths must match exactly, including capitalization, especially once hosted on a case-sensitive server like GitHub Pages.
- **Structuring the table correctly:** Getting `<thead>`, `<tbody>`, and `<tfoot>` to render in the right order (footer content still needs to be written *before* the closing `</table>`, even though it displays at the bottom) took some trial and error.
- **Balancing semantic tags naturally:** Fitting in required elements like `<aside>`, `<time>`, `<mark>`, `<blockquote>`, and `<details>`/`<summary>` on the About page without them feeling forced took a few rewrites to keep the content readable.
- **Keeping the form usable without CSS or JS:** Since styling wasn't allowed, extra care went into using `<fieldset>` and `<legend>` to visually group related form fields so the contact form stayed organized and readable in plain HTML.

## Author

Jordan Hayes — 2026

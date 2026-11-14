# web_dev_104

Portfolio site for Jamaar E. Peters (WEB DEV 104). Milestone 2 styles the three-page skeleton with a shared stylesheet, Flexbox, and CSS Grid.

## Milestone 2: Responsive Design with Flexbox & Grid

`styles.css` is linked from `index.html`, `projects.html`, and `about.html`. Layout is mobile-first and stays on an 8px spacing scale (`--space-1` through `--space-8`).

- **Flexbox** lays out the header and navigation. Links stack on small screens and sit in a row from 768px.
- **CSS Grid** (`.split`) places paired regions side by side from 768px: the Quick Overview figure and Highlights on the home page, the two project cards, and Bio beside Contact.
- **1200px and up**, `.container` is centered at a max width of 1140px and the type scale steps up.

### Color palette

Custom properties in `styles.css`:

| Token | Hex | Use |
| --- | --- | --- |
| `--color-bg` | `#0f172a` | Page background |
| `--color-panel` | `#1e293b` | Header, cards, and footer |
| `--color-text` | `#f8fafc` | Body text |
| `--color-accent` | `#f59e0b` | Headings and the active nav link |
| `--color-secondary` | `#38bdf8` | Links and subheadings |
| `--color-muted` | `#94a3b8` | Captions, intro, and footer |

### Fonts

Google Fonts, with preconnect, on every page:

- Headings: Poppins
- Body: Inter

### Live site

https://jpeters-coder.github.io/web_dev_104/

## Milestone 3: Accessible & Designed

### Accessibility — WAVE results (Nov 14, 2026)

WAVE was run on all three pages after the Milestone 3 changes. All three passed with zero errors, zero contrast errors, and zero alerts (AIM 10/10 on every page), so no fixes were needed.

- The contact form was built accessibly from the start: every field has a linked `<label>`, the inquiry-type radios are grouped in a `<fieldset>` with a `<legend>`, and validation errors appear as visible text messages in the page (linked with `aria-describedby` and `aria-invalid`) instead of pop-up alerts, so screen-reader users hear the error right at the field.
- All text/background color combinations pass WCAG AA (4.5:1 for normal text), verified with the WCAG contrast formula: body text 17.06:1 on the page background and 13.98:1 on panels; muted captions 6.96:1 and 5.71:1; accent headings 8.31:1 and 6.81:1; secondary links and subheadings 8.33:1 and 6.83:1; the active nav link 8.31:1; form error text 9.41:1.

### Gestalt principles

- **Proximity:** I used proximity to group each card's heading, text, and list tightly together while widening the gap between cards, so each card reads as one unit.
- **Similarity:** I used similarity by giving every card the same panel background, border, padding, and corner radius, and every nav link the same shape, so items that work the same way look like they belong together.

### Accessible contact form

Added to `about.html`: Name, Email, Inquiry type (radio group), and Message — four fields with linked labels, fieldset/legend grouping, and error messages shown in the page and announced with `role="alert"`.

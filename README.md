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

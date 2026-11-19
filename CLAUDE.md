# CLAUDE.md

## Purpose
One-page marketing site for **Ghat Side Chai Co.**, a (sample) chai and filter-coffee cafe in Nashik. Visitors browse the menu, read the story, and order or book a table via WhatsApp.

## Structure
- `index.html` — the entire site: markup, inline `<style>` (design tokens on `:root`), and a small inline `<script>`. No build step, no dependencies beyond Google Fonts (Hind, Rozha One).
  - Sections: header/hero (`#top`), `#menu`, `#story`, `#visit` (with the `#enquiry` form), plus a floating WhatsApp button.
  - The enquiry form builds a prefilled `wa.me` link from the form fields.
- `README.md` — one-line description.

## Notes
- `WHATSAPP_NUMBER` in the script, and the hard-coded `wa.me/919999999999` links in the hero and floating button, are placeholders. Update all three together.
- Keep it a single static file unless there is a clear reason to split it.

## Preview locally
Open `index.html` directly in a browser, or serve the folder:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deployment
Not deployed yet. There is no hosting or CI configured.

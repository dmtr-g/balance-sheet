# Balance Sheet

An interactive financial balance sheet built with HTML, CSS, and vanilla JavaScript. No frameworks, no build step — just open the file in a browser and it works.

---

## What it does

Tracks assets, liabilities, and net worth across multiple years (2020–2026) in a clean table layout. You can enter values directly in the table, switch between currencies, toggle which years are visible, and export the sheet as a PDF or Word document. Totals update live as you type.

---

## Demo

./Screenshot.png

> **To run locally:** open `index.html` directly in any browser. No server needed.

---

## Stack

| Layer | Tech |
|---|---|
| Structure | HTML5 — semantic tables, `fieldset`, `caption` |
| Styling | CSS3 — custom properties, flexbox, media queries, keyframe animation |
| Logic | Vanilla JavaScript — DOM manipulation, Blob API, `window.print()` |
| Fonts | Segoe UI / system font stack |

No npm. No dependencies. No build step.

---

## Getting started

```bash
# Clone the repo
git clone https://github.com/dmtr-g/balance-sheet.git
cd balance-sheet

# Open in browser (pick your OS)
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or just double-click `index.html` in your file explorer.

---

## Features

- **Editable company name** — click the title field and type your own
- **Year toggle** — checkboxes show/hide any column from 2020 to 2026
- **Live totals** — assets, liabilities, and net worth recalculate as you type
- **Currency switcher** — USD, EUR, GBP, JPY, INR
- **Export to PDF** — triggers the browser's print dialog (works everywhere)
- **Export to Word** — downloads a `.doc` file with the current table data
- **Responsive** — horizontal scroll on narrow screens, mobile-friendly controls
- **Accessible** — screen-reader labels on all visually hidden elements (`sr-only`)

---

## Project structure

```
Balance-Sheet/
├── index.html      # Markup + embedded JavaScript
├── styles.css      # All styling (variables, layout, responsive breakpoints)
└── README.md
```

---

## What I learned / Why I built this

This started as a freeCodeCamp CSS exercise focused on pseudo-selectors and `sr-only` accessibility patterns. I extended it with JavaScript to make it actually functional.

Key things practised:

- CSS attribute selectors (`span[class~="sr-only"]`) and accessibility-first `!important` overrides
- CSS custom properties for consistent theming without a preprocessor
- Sticky positioning for the year header bar while scrolling
- DOM traversal using `querySelectorAll` with `data-year` attribute filters
- Blob API for generating client-side Word file downloads
- `window.print()` as a zero-dependency PDF export

---

## Author

**Dumitru Gafincu** — [github.com/dmtr-g](https://github.com/dmtr-g) — 115009621+dmtr-g@users.noreply.github.com

---

*Built as part of the freeCodeCamp Responsive Web Design curriculum, extended with additional JavaScript functionality.*

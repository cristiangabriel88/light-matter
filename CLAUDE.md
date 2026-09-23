# Light & Matter

Single-page portfolio for handmade lamps. The live page is `light-and-matter.html` (HTML, CSS and JS all inline).

## Rules

- **No em dashes anywhere in the project**: not in site copy, code, comments, or commit messages. Use a colon, comma, period, middle dot (`·`) or parentheses instead. En dashes in number ranges (`3–5 weeks`, `€240–290`) are fine.
- **Every text change goes in both languages, English and Romanian.** If you add, edit or remove English copy, update the Romanian to match in the same change. Never leave one language behind.

## How the translation works

The page is written in English. Romanian is swapped in string by string from dictionaries keyed by the exact English:

- `var RO = { ... }` in the first `<script>`: all page copy, `alt` / `aria-label` / `data-label` attributes, and the photo deck (`PIECES`) text.
- A second `var RO = { ... }` in the second `<script>`: the Full specification popup (`SPECS`).

Keys must match the English exactly as the page holds it: whitespace collapsed to single spaces, inner HTML kept (`<br>`, `<b>`, `&amp;`), and `\'` for apostrophes. If a key doesn't match, that line silently stays in English. When you change English text, change its key too, and remove keys whose English no longer exists on the page.

# Pink theme notes (soft pastel version)

All colours live in the `:root` block at the top of `index.html`. Variable names are unchanged (`--ube`, `--mango` and so on), only the values changed. Meaning now: `--ube` = dusty rose, `--ube-deep` = deeper dusty rose, `--ube-mist` = blush, `--mango` = pale gold, `--pink` = petal.

| Variable | Original | First pink | Soft pink (now) |
|---|---|---|---|
| `--ube` | #4A2C85 | #8F3058 | #9E4A68 |
| `--ube-deep` | #35205F | #6E2447 | #8A3F5D |
| `--ube-mist` | #EDE6F8 | #FDEAF1 | #FEF1F5 |
| `--mango` | #F4B63F | #F2C078 | #FBE0B0 |
| `--pink` | #F27C8A | #F4A3BF | #F7B8CD |
| `--dahon` | #2E6B52 | #8A3B5C | #9A4562 |
| `--white` | #FFFEFA | #FFFAF5 | #FFFAF5 |
| `--ink` | #2A1B47 | #3B1A2B | #4A2636 |

Also softened: `theme-color` meta (#8A3F5D), confetti and ambient colours, scratch-card gold, lightbox backdrop, cake heart, `images/og-image.png` (1200x630).

## Contrast (WCAG 2.x, computed; AA needs 4.5 for text)

| Text on background | Ratio | AA |
|---|---|---|
| cream on rose | 5.57 | pass |
| cream on deep rose | 6.86 | pass |
| gold on rose (timeline times, labels) | 4.51 | pass |
| gold on deep rose | 5.56 | pass |
| deep rose on gold (buttons) | 5.56 | pass |
| deep rose on gold hover #FDE9C6 | 5.98 | pass |
| rose on cream (titles, ghost button) | 5.57 | pass |
| rose on blush | 5.26 | pass |
| ink on cream (body) | 12.48 | pass |
| ink on blush | 11.79 | pass |
| rose accent on cream | 5.95 | pass |
| rose accent on blush | 5.62 | pass |
| error red #A3262A on blush | 6.66 | pass |

## Notes
- The darkest rose pages are as light as they can go while keeping cream text at 4.5 or more (cream on rose is the tightest at the low end of this table with gold on rose). A lighter surface would need dark text, which means changing rules beyond colour variables.
- Decorative only, no text: petal #F7B8CD, heart #D1668C, confetti.
- Tap targets and reduced-motion rules untouched. `#openBtn` measures 42px high in headless Chrome at 390px, same CSS as main; not changed.

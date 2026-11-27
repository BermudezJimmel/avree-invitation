# Pink theme notes

All colours live in the `:root` block at the top of `index.html`. The variable names are unchanged (`--ube`, `--mango` and so on), only the values changed, so no rule needed rewriting. Names now mean: `--ube` = rose, `--ube-deep` = deep rose, `--ube-mist` = blush, `--mango` = soft gold, `--pink` = petal.

| Variable | Old | New |
|---|---|---|
| `--ube` | #4A2C85 | #8F3058 (rose) |
| `--ube-deep` | #35205F | #6E2447 (deep rose) |
| `--ube-mist` | #EDE6F8 | #FDEAF1 (blush) |
| `--mango` | #F4B63F | #F2C078 (soft gold) |
| `--pink` | #F27C8A | #F4A3BF (petal) |
| `--dahon` | #2E6B52 | #8A3B5C (rose accent text) |
| `--white` | #FFFEFA | #FFFAF5 (warm cream) |
| `--ink` | #2A1B47 | #3B1A2B |

Also changed: `theme-color` meta (#6E2447), confetti and ambient colours, scratch-card gold, lightbox backdrop, cake heart, `images/og-image.png` (1200x630).

## Contrast (WCAG 2.x, computed)

| Text on background | Ratio | AA (4.5, text) |
|---|---|---|
| cream on rose | 7.41 | pass |
| cream on deep rose | 10.09 | pass |
| gold on rose (timeline times, labels on rose page) | 4.61 | pass |
| gold on deep rose | 6.27 | pass |
| deep rose on gold (buttons) | 6.27 | pass |
| deep rose on gold hover | 7.11 | pass |
| rose on cream (titles, ghost button) | 7.41 | pass |
| rose on blush | 6.67 | pass |
| ink on cream (body) | 14.8 | pass |
| ink on blush | 13.3 | pass |
| rose accent (`--dahon`) on cream / blush | 7.1 / 6.4 | pass |
| error red #A3262A on cream | 7.1 | pass |

## Notes
- Rose pages are deeper than a pastel on purpose: white text on a pale pink would fail AA. Light pages use blush and cream.
- Decorative only, no text: petal `#F4A3BF`, heart `#C23B73`, confetti.
- Tap targets: unchanged. `#openBtn` measured 42px high in headless Chrome at 390px, same CSS as on main (`min-height: 2.75rem`); not changed.
- Reduced-motion rules untouched.

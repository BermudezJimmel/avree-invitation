# Pink theme notes (light pastel version)

All colours live in the `:root` block at the top of `index.html`. Variable names from the original page are kept (`--ube`, `--mango` and so on), only their values changed. Three variables were added for the light pages: `--petal-bg`, `--petal-bg2`, `--plum`.

This version turns the old mid-tone rose pages (Welcome banig, How the day goes, Make a wish, curtain) into light pastel surfaces. Text on them is now dark plum or deep rose. Deeper rose stays only on small accents: the bottom bar, checked choices, the thank-you card, borders and icons.

| Variable | Original | Soft pink (8ec3a59) | Light pastel (now) |
|---|---|---|---|
| `--ube` (rose accent) | #4A2C85 | #9E4A68 | #9E4A68 |
| `--ube-deep` (deep rose) | #35205F | #8A3F5D | #8A3F5D |
| `--ube-mist` (blush) | #EDE6F8 | #FEF1F5 | #FEF1F5 |
| `--mango` (pale gold) | #F4B63F | #FBE0B0 | #FBE0B0 |
| `--pink` (petal) | #F27C8A | #F7B8CD | #F7B8CD |
| `--dahon` (rose accent text) | #2E6B52 | #9A4562 | #9A4562 |
| `--white` (cream) | #FFFEFA | #FFFAF5 | #FFFAF5 |
| `--ink` | #2A1B47 | #4A2636 | #4A2636 |
| `--petal-bg` (new) | - | - | #FBDDE8 |
| `--petal-bg2` (new) | - | - | #F8CFDE |
| `--plum` (new) | - | - | #5E2540 |

Where they are used now: page body, banig, "How the day goes" = `--petal-bg`; "Make a wish" and curtain halves = `--petal-bg2`; curtain card = blush with a rose border; text on those = `--plum`, titles, surname, timeline times and the outline microphone button = `--ube-deep`. `images/og-image.png` (1200x630) regenerated as light petal with plum and deep rose text.

## Contrast (WCAG 2.x, computed; AA needs 4.5 for normal text)

| Text on background | Ratio | AA |
|---|---|---|
| plum text on petal (welcome, program pages) | 9.15 | pass |
| plum text on deep petal (cake page) | 8.25 | pass |
| plum text on blush (curtain card) | 10.53 | pass |
| deep rose titles/times on petal | 5.63 | pass |
| deep rose titles/buttons on deep petal | 5.08 | pass |
| deep rose on gold (buttons) | 5.56 | pass |
| deep rose on gold hover #FDE9C6 | 5.98 | pass |
| cream on deep rose (bottom bar, checked choice) | 6.86 | pass |
| gold on deep rose (bottom bar dot/progress) | 5.56 | pass |
| cream on rose (thank-you card) | 5.57 | pass |
| rose on cream (titles, ghost button) | 5.57 | pass |
| rose on blush | 5.26 | pass |
| ink on cream (body) | 12.48 | pass |
| ink on blush | 11.79 | pass |
| rose accent on cream | 5.95 | pass |
| rose accent on blush | 5.62 | pass |
| error red #A3262A on blush | 6.66 | pass |

## Notes
- Decorative only, no text: petal #F7B8CD, heart #D1668C, confetti, banig pattern, cake tiers.
- Tap targets and reduced-motion rules untouched. `#openBtn` measures 42px high in headless Chrome at 390px, same CSS as main; not changed.

# Avree invitation: what changed

File: `index.html` (single file, no libraries, no CDN). Backup of the old page: `../avree-invitation-backups/index-before-interactive.html`.
Copy, dates, venue, links and the ninong/ninang list are unchanged. Edit details in the `CONFIG` block near the bottom of `index.html`.

## New features and how to try them

| Feature | How to try it |
|---|---|
| Curtain opening | Drag the curtain sideways, or tap "Open the invitation". |
| Page turns | Tap Next/Back, swipe left/right, or use arrow keys. |
| Progress dots and bar | Bottom bar. Tap a dot to jump. |
| Floating balloons and sparkles | Welcome page. Tap a balloon to pop it. Decor is hidden with reduced motion. |
| Scratch card | Save the date page. Scratch the gold card, or tap "Show the date without scratching". |
| Live countdown | Appears after the scratch. Days, hours, minutes, seconds to the event. |
| Add to calendar | Google link and `.ics` download (Apple/Outlook) on When and where. Map buttons still work. |
| Blow out the candle | Make a wish page. Tap the candle or use the microphone. Confetti, smoke, then write a wish. |
| Wish wall | Wishes are saved on that device only (localStorage). |
| Hold to promise | A request page. Press and hold the button. |
| Reply | Reply page. The form builds the text and opens a prefilled text message, or "Copy my reply". Uses the contact number already in the page. |
| Scroll reveals | Items fade in as each page shows. |

## Photo spots (new)

Eight framed spots, one per page, in order: Welcome, Save the date, When and where, How the day goes, Make a wish, Gifts, A request, Reply.

- Put photos in `images/` named `avree-1.jpg` to `avree-8.jpg`. See `images/README.txt` (about 1200px wide, under 300 KB).
- Missing file: a soft pink frame shows "Avree photo N / Photo coming soon". Nothing breaks.
- File present: the photo shows with a gentle zoom-in fade. Tap it to enlarge. Close with the Close button, Esc, or a tap outside.
- Images use `loading="lazy"`, `object-fit: cover`, and alt text "Avree photo N".
- The old "tap to add a photo" picker and the `photo` setting in `CONFIG` were removed. The Welcome photo is now `images/avree-1.jpg`.
- To change the folder or extension, edit `PHOTO_DIR` and `PHOTO_EXT` in the "Photo spots" script section.

## Accessibility

- `prefers-reduced-motion`: animations, tilt, zoom and decor are turned off.
- Keyboard: all controls are real buttons. Arrow keys turn pages, except while a photo is enlarged.
- Screen readers: labels on controls, live regions for the countdown message, wish and form status.
- Layout uses fluid sizes aimed at 320px width.

## Not done / limits

- Music toggle not added: the page has no audio file.
- Testing: HTML tags balance and the script passes `node --check`. Headless Chrome could not start here (sandbox error), so there was no browser run and no console check. Please open the page once on your phone.
- Reply and wishes need no backend. Wishes stay on the guest's own device.

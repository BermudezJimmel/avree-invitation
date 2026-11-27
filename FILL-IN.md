# Fill-in list for Avree's invitation

**Warning: this repo is public.** Anything you commit can be read by anyone, and git history keeps it even after you delete it.
Do **not** commit the GCash number or the GCash QR image. Do not commit a home address you want private.
Send the GCash number and QR to guests in a private message, or host the page somewhere private.

The page still has only placeholders. No real phone, GCash number or address is in it.

## In the CONFIG block (`<script>` near the bottom of `index.html`)

| Field | Now | Fill in |
|---|---|---|
| `start` | `2026-12-12T10:00:00+08:00` (placeholder) | Real date and binyag time, Philippine time (+08:00) |
| `events[0]` Binyag | "Your church name here", "Church address, City, Philippines" | Church name, address, map search text (`mapQuery`), time |
| `events[1]` Handaan | "Your venue name here", "Venue address, City, Philippines" | Venue name, address, map search text, time |
| `program` | Sample times | Real program times (format `9:30 AM`) |
| `rsvpNote` | "reply by December 1, 2026" | Real reply deadline |
| `rsvpPhone` | empty (text button hidden) | Digits only, e.g. `639171234567` |
| `rsvpMessenger` | empty (button hidden) | Messenger username, the part after `m.me/` |
| `rsvpViber` | empty (button hidden) | Digits only, e.g. `639171234567` |
| `giftOptions[1]` GCash | `09XX XXX XXXX` | Prefer to leave the number out of the public repo. See the warning above |
| `godparents` | empty (block hidden) | Ninong and ninang names, one per line |

## In the HTML (plain text, edit by hand to match the CONFIG values)

| Where | What to change |
|---|---|
| `<head>` `og:url`, `og:image`, `twitter:image` | Your real page address. The three now say `https://bermudezjimmel.github.io/avree-invitation/` (a guess). Link previews need full `https://` addresses |
| `<noscript>` block (top of `<body>`) | Date, church, venue, reply deadline, and the "Contact: your phone number here" line |

## Image files in `images/`

| File | Status |
|---|---|
| `og-image.png` | A simple 1200x630 placeholder card is included. Replace it with a nicer one if you like (keep 1200x630, under 300 KB) |
| `avree-1.jpg` to `avree-8.jpg` | Not added yet. About 1200px wide, under 300 KB each. Order: Welcome, Save the date, When and where, How the day goes, Make a wish, Gifts, A request, Reply |
| `gcash-qr.png` | Do not add to the public repo |

## Before you send it

1. Fill in the table above, then open the page on one Android and one iPhone.
2. Open it inside Messenger and Viber too. In-app browsers behave differently.
3. Paste the link into a chat to check the preview card (Facebook may cache an old preview. Use the Sharing Debugger to refresh it).

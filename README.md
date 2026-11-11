# Best Days Behind: show & ticket page

One-page ticket landing page for Best Days Behind. Right now it sells the
UNWARPED show (Sat Nov 14, 2026, West End Trading Co, Sanford, FL).

- Live (free): https://goodstory23.github.io/best-days-behind-tickets/
- Facebook pixel: "Best Days Behind - Ticket Page" (ID 1071895152533133), in the
  Good Story business, connected to the Good Story Ad Account.

## How the page handles future shows
- All show details live in one list called `UPCOMING`, near the bottom of `index.html`.
- The page always shows the soonest show that hasn't finished yet.
- 6 hours after doors open, a show drops off by itself. Old shows are never shown.
- With no upcoming shows, the page switches to "Next show coming soon" and its
  buttons point to the band's Facebook page.

## Adding a new show
1. Open `index.html` and find `var UPCOMING = [`.
2. Copy the whole `{ ... }` block for a show, paste it after a comma, and change
   the details: name, doors time, price, venue, ticket link, bands and the four "why" cards.
3. Put the new flyer in `images/` and point `flyer:` at it. Use `logos: ''` if there's
   no logo picture.
4. Doors time format: `'2027-02-06T19:00:00-05:00'` (use `-05:00` Nov to Mar and `-04:00` Mar to Nov).
5. Also update the share preview at the top of the file (`og:title`, `og:description`,
   `og:image`) and `share.jpg`, because texted links can't read the show list.

## What the pixel tracks
- **PageView** for every visit.
- **InitiateCheckout** (with the ticket price) every time someone taps a "Get Tickets" button.
- The ticket sale itself happens on Opendate, so this pixel can't see completed purchases.

## Putting it on bestdaysbehind.info/tickets
1. In your website host's file manager, make a folder called `tickets` next to your home page.
2. Upload `index.html`, `share.jpg` and the whole `images` folder into it.
3. In `index.html`, swap the web addresses that start with
   `https://goodstory23.github.io/best-days-behind-tickets/` for `https://bestdaysbehind.info/tickets/`.

## Changing the page
Edit `index.html`, then commit and push. GitHub Pages updates in about a minute.

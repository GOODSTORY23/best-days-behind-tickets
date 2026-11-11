# Notes for Tommy

Things I noticed but did not change:

- **No Facebook event for Nov 14.** The band's Facebook Events tab shows no upcoming events, only past ones.
  A Facebook event for UNWARPED that links to this page would help people find it.
- **bestdaysbehind.info "Show Dates" are old.** It still lists May 28 Tampa, May 29 Lake Worth,
  May 30 Miami and May 31 Orlando, and doesn't list Nov 14.
- **Pixel lives under Good Story.** The Best Days Behind Facebook page isn't owned by any of your business
  accounts, so the pixel went into the Good Story business and was connected to the Good Story Ad Account.
  If ads will run from another ad account, the pixel needs to be shared with it in Business Settings.
- **The pixel can't count ticket sales,** only taps on "Get Tickets", because checkout happens on Opendate.
  If Opendate lets you add a Meta pixel to the event, adding this same pixel ID there would count real purchases.
- The logo on bestdaysbehind.info is a tiny file (50 pixels wide), so I cut a sharper logo badge out of
  the lineup picture you sent instead.
- **Leftovers on SiteGround (2026-11-11).** Inside bestdaysbehind.info → public_html → tickets there's an empty
  `bdb-tickets` folder and the `bdb-tickets.zip` upload file. Neither one affects the page. I left them alone
  (no deleting without your OK). There's also a copy of `bdb-tickets.zip` on your Desktop.
- **bestdaysbehind.info home page still lists Shawn Courters on drums** (in "Who We Are" and "The Band"),
  not Ryan Via. Noticed 2026-11-11; not changed.
- **Two copies of the page now.** bestdaysbehind.info/tickets (SiteGround) and the GitHub address. A change pushed
  to GitHub does NOT update the SiteGround copy, so it has to be re-uploaded there too.

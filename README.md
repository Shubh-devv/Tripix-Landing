# Triplix Holidays — landing page

Upload this whole folder to Netlify (drag and drop) or any static host. No build step.

## Photos
Destination and package photos are free Unsplash / Pexels photos (commercial use allowed, no credit
required). Each one has the client's own photo from /assets as an automatic fallback.

To host every photo yourself (recommended before going live):

    node download-photos.mjs        # Node 18+, saves them into assets/photos/

Then in index.html set  localPhotos: true  inside CFG. The script tells you if any photo fails —
replace that URL in the PHOTOS block and run it again.

## Editing
Everything editable is near the top of the <script> in index.html:

- CFG.wa — WhatsApp number every button sends to (currently 919971798730)
- PHOTOS — web photo URL + local fallback for each place
- PACKAGES — each trip: title, route, price, was (struck-out price), highlights, day-by-day, exclusions, notes
- DEST — the "Where do you want to go?" tiles (India / World), best-time months and "We also plan" chips
- ON_REQUEST, SERVICES, WHY, INCL, EXCL, TERMS — the other lists on the page

Logo: assets/triplix-logo.png (the client's original file, trimmed).

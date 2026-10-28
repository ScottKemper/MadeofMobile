THE MOBILE COLLECTION - coaster QR landing page

DEPLOY ON RENDER (Static Site)
  1. Put this folder in a GitHub repo (index.html at the top level, images/ beside it).
  2. Render > New > Static Site > pick the repo.
  3. Build Command:      (leave blank)
     Publish Directory:  .
  4. Deploy. Add your own domain under Settings > Custom Domains.

QR CODE LINKS (one per stop; add a unique code per coaster later)
  https://YOURDOMAIN/?stop=uss-alabama
  https://YOURDOMAIN/?stop=exploreum
  https://YOURDOMAIN/?stop=history-museum
  https://YOURDOMAIN/?stop=saenger-theatre
  https://YOURDOMAIN/?stop=carnival-museum
  https://YOURDOMAIN/?stop=gulfquest
  https://YOURDOMAIN/?stop=phoenix-fire-museum
  https://YOURDOMAIN/?stop=richards-dar-house
  With serialized coasters:  ...?stop=gulfquest&c=7K2QX9
  No ?stop= shows the general Mobile Collection page.

EDIT IN index.html (the SETTINGS block near the bottom)
  customGoodsUrl, mapUrl, sponsors (name, link, logo image in images/).

PASSPORT SAVING
  The page runs in PREVIEW MODE until CONFIG.passport is connected: stamps show
  but are not saved, and a bar at the top says so. Connecting sign-in by text code
  and the stamp database (Supabase, Firebase or your own API) means filling in the
  four functions described in CONFIG: load, stamp, sendCode, verify.

Zoe Llaine Simeon's Baptism - Jollibee FairyTale Land invitation website
(Sunday, October 4, 2026 - Guiguinto, Bulacan)
==========================================================================

Files
  index.html                 the whole site (HTML + CSS + JS + Lottie data in one file)
  images/                    WebP images, the waving GIF, and the 1200x630 link-preview thumbnail
                             (zoe-llaine-simeon-baptism-invitation-og.jpg)
  audio/fairytale-lullaby.mp3   background music (original music-box waltz composed for this site, ~76 s loop)
  animations/celebration-confetti.json   the Lottie sparkle animation (also embedded in index.html)
  robots.txt, sitemap.xml    search-engine files

Before you publish
  1. Find & replace  https://www.example.com/  with your real address in:
       index.html (canonical, hreflang, og:url, og:image, twitter:image, JSON-LD)
       robots.txt and sitemap.xml
  2. Upload the whole folder to any static host (Netlify Drop, Cloudflare Pages, GitHub Pages, Vercel...).
  3. Link previews (Messenger, Viber, WhatsApp, Facebook, X) show the thumbnail only once the page is live
     at your real address, because the image must be reachable by its full URL. If an app shows an old or
     missing preview, refresh it with the Facebook Sharing Debugger (developers.facebook.com/tools/debug).
  4. Optional: submit sitemap.xml in Google Search Console.

Event details (edit in index.html - search for the words)
  10:30 am  Baptism mass - San Ildefonso Parish Church, Poblacion, Guiguinto, Bulacan (Diocese of Malolos)
  12:00 noon  Celebration - Jollibee Sta. Cruz, Guiguinto
  Assumed end times (not given): the countdown's "thank you" message and the Google Calendar entry
  assume the day wraps up around 3:00 pm / 2:30 pm. Change END in the <script> at the bottom of index.html
  and the dates=... part of the "Add to Google Calendar" link if that is wrong.
  "View map" links search by venue name; swap in exact Google Maps share links if you have them.

Background music
  Browsers block sound autoplay until a visitor interacts with the page, so the page tries to autoplay
  and, if the browser says no, starts the music on the first tap / click / key press (a small hint and a
  pulsing music button at the bottom left tell people). The music button toggles it; the choice is remembered.
  To use your own track, replace audio/fairytale-lullaby.mp3 (keep the file name, or update the <audio> tag).

Waving GIF
  images/zoe-llaine-simeon-waving.gif was made by animating Zoe's photo (arms lifted and lowered), not from
  video. If you have a real GIF or short clip of her waving, save it over that file (440x500 works best).
  Visitors who prefer reduced motion see a still image instead.

Celebration animation (Lottie)
  Plays on page load, on "Enter FairyTale Land", at "See you!", and whenever the wand button (bottom right)
  is tapped. Skipped automatically for visitors with "reduce motion" on (the button still works for them).
  To use a different Lottie, paste its JSON into <script type="application/json" id="lottie-confetti">.
  Player: lottie-web 5.12.2 from cdn.jsdelivr.net.

Countdown
  Counts down to Oct 4, 2026, 10:30 am Philippine time (UTC+8), then shows "It's Zoe's big day!".

Privacy note
  The page is set to be indexed by search engines. To keep it private to people who have the link, change
  <meta name="robots" content="index, follow, ..."> to <meta name="robots" content="noindex, nofollow">
  and in robots.txt use  Disallow: /

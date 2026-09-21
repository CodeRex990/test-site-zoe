Zoe Simeon's Baptism - static invitation website  (Sunday, Oct 4, 2026)
=========================================================================

Files
  index.html                  the whole site (HTML + CSS + JS + Lottie data in one file)
  images/                     optimized WebP images
    zoe-simeon-baptism-invitation-og.jpg   1200x630 THUMBNAIL used for link previews
  animations/celebration-confetti.json      the Lottie animation (also embedded in index.html)
  robots.txt, sitemap.xml     search-engine files

Before you publish
  1. Find & replace  https://www.example.com/  with your real address in:
       index.html (canonical, hreflang, og:url, og:image, twitter:image, JSON-LD)
       robots.txt and sitemap.xml
  2. Upload the whole folder to any static host (Netlify Drop, Cloudflare Pages,
     GitHub Pages, Vercel, or regular web hosting).
  3. Link previews (Messenger, WhatsApp, Viber, Facebook, X) only show the thumbnail
     once the page is live at your real address, because the image must be reachable
     by its full URL. If a chat app shows an old or missing preview, refresh it with the
     Facebook Sharing Debugger (developers.facebook.com/tools/debug) - it also updates Messenger.
  4. Optional: submit sitemap.xml in Google Search Console.

Things to double-check (carried over from the earlier invitation)
  - Times and venues: church 11:00 am, Jollibee Northbay 1:00 pm, Biclar Residence 3:30-10:00 pm
  - Gift ideas and dress code
  - "View map" links search by venue name; swap in exact Google Maps share links if you have them
  Everything is plain text in index.html - search for the words to edit them.

Countdown
  Counts down to Oct 4, 2026, 11:00 am Philippine time (UTC+8). After that it shows
  "It's Zoe's big day!" and, after 10:00 pm, a thank-you message.
  Change START / END in the <script> at the bottom of index.html if plans change.

Celebration animation (Lottie)
  Plays on page load, when "Join the fun!" is tapped, at the "See you!" sign-off, and
  whenever the party-popper button (bottom right) is tapped. It is skipped automatically
  for visitors who have "reduce motion" turned on (the button still works for them).
  To use a different Lottie, paste its JSON over the contents of
  <script type="application/json" id="lottie-confetti"> in index.html.
  The player is lottie-web 5.12.2, loaded from cdn.jsdelivr.net.

Privacy note
  The page is set to be indexed by search engines. To keep it private to people who
  have the link, change  <meta name="robots" content="index, follow, ...">  to
  <meta name="robots" content="noindex, nofollow">  and in robots.txt use  Disallow: /

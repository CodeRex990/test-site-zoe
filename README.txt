Aki's Baptism & 1st Birthday - static invitation website
=========================================================

Files
  index.html      the whole site (HTML + CSS + JS in one file)
  images/         optimized WebP images + og-cover.jpg (social share preview)
  robots.txt      crawler rules
  sitemap.xml     sitemap for search engines

Before you publish
  1. Find & replace  https://www.example.com/  with your real address in:
       index.html (canonical, hreflang, og:url, og:image, twitter:image, JSON-LD)
       robots.txt and sitemap.xml
  2. Optional: swap the three "View map" links for exact Google Maps share links
     (search for "maps/search" in index.html). Biclar Residence and Event Place
     currently searches by name only.
  3. Upload the whole folder to any static host
     (Netlify Drop, Cloudflare Pages, GitHub Pages, Vercel, or regular web hosting).
  4. Submit sitemap.xml in Google Search Console.

Privacy note
  The page is set to be indexed by search engines. To keep it private to people
  who have the link, change   <meta name="robots" content="index, follow, ...">
  to   <meta name="robots" content="noindex, nofollow">   and in robots.txt use
  "Disallow: /".

Countdown
  Counts down to Sept 20, 2026, 11:00 am Philippine time (UTC+8). After that it
  shows "It's party day!" and, after 10:00 pm, a thank-you message.
  Change START / END in the <script> at the bottom of index.html if plans change.

VIP LANDMARK WEBSITE  (static, no server needed)
Prepared 3 November 2026 for AEVUM Ventures / VIP Landmark.

WHAT IS HERE
  index.html      the whole site: one page with anchored sections (project, location, Club VIP,
                  sites and price, villa option, master plan, documents, gallery, FAQ, site visit)
  images/         photographs (drone stills and site photos, October 2026), two renders marked as
                  such, the master plan, AEVUM logo, marble texture, WhatsApp QR

HOW TO HOST IT (any of these works)
  1. Shared hosting (cPanel / Hostinger / GoDaddy): upload index.html and the images folder to
     public_html. Done.
  2. Netlify, Cloudflare Pages or Vercel (free): drag the folder onto the dashboard, then point
     the domain (viplandmark.in) to it from the DNS panel they show you.
  3. GitHub Pages: put the folder in a repository, enable Pages, add the domain.
  Fonts load from Google Fonts; everything else is in this folder.

BEFORE GOING LIVE
  - Change nothing in the compliance footer without AEVUM: promoter line, K-RERA number, DTCP number.
  - Prices: the launch rate (Rs 2,349) and the three lakh figures appear in the top bar, the hero,
    the Sites and price section and the FAQ. Search the file for "2,349" and "28.2" when the rate changes.
  - Primary call number is 88612 05108 (header, hero, visit section, floating call button, SMS). WhatsApp
    links and the QR use 96068 28756 because the printed flyers carry that QR. Search for "8861205108",
    "9606828756" (links) and the spaced forms (text) to change them.
  - Plot picker: the site list is embedded in index.html inside <script id="pk-data">. Each row is
    [site, dimension, area, facing, corner, east, main road, PLC %, plot value, price]. When sites sell,
    delete their rows (or ask for a regenerated list from the live inventory sheet). A site removed from
    pk-data stops being clickable on the plan automatically.
  - Graphical picker: <script id="pk-map"> holds each site's box on images/masterplan.jpg as
    [x, y, width, height] in image pixels (1720 x 2767). If the plan image is ever replaced, these
    boxes must be re-measured; otherwise leave them alone. By choice the picker shows no prices:
    buyers ask for the cost sheet on WhatsApp or by phone.
  - Concierge (gold chat button): a scripted helper, no server and no AI. Its answers are in the
    "A" object inside the concierge script block; edit the text there when prices or timings change.
    It ends by handing the visitor to WhatsApp or a call.
  - The enquiry form opens WhatsApp, SMS or email with the details filled in; nothing is stored. To collect leads on a
    server instead, add a form service (Formspree, Web3Forms or your CRM) to the <form> tag.
  - Add Google Analytics or Meta Pixel before </head> when the ad campaigns start.
  - A Kannada page can be added as kn.html with the same layout; ask for it when needed.

SITE FILES (upload everything, keep the names)
  - index.html, 404.html, favicon.ico, robots.txt, sitemap.xml, images/
  - Every photo has a half-size twin (name-800.jpg) that phones and thumbnails load; the full file
    opens in the gallery viewer. If you replace a photo, replace both files.
  - images/og.jpg (1200x630) is the preview card WhatsApp, Facebook and LinkedIn show when the link is
    shared. The links in <head> point to https://viplandmark.in/; if the site goes on another domain,
    search index.html and sitemap.xml for "viplandmark.in" and change it.
  - Set 404.html as the "not found" page in the hosting panel (Hostinger/cPanel: Error Pages, or
    ErrorDocument 404 /404.html in .htaccess).
  - After going live: submit https://viplandmark.in/sitemap.xml in Google Search Console and test the
    page with https://search.google.com/test/rich-results (it carries FAQ, project and agent markup).

NOT ON THIS SITE, BY CHOICE
  - No "proposed" amenities, no brochure button that goes nowhere, no drafting notes, no landmarks
    that are not within reach of Bagepalli. Every photograph was taken at the site except the two renders.
  - Landsphere is not named anywhere; the Jakkur office appears as "Jakkur office".

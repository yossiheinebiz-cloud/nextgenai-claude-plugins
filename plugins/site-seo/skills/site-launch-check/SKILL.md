---
name: site-launch-check
description: Pre-launch and post-deploy checklist for a small business or startup website on any stack. Checks broken links, alt text, mobile layout, forms, analytics, legal pages, security headers, sitemap and robots. Use when the user asks to check, QA or audit a site before or after going live.
---

# Site launch check

Run what can be run (build, link checker, curl). Report what needs a human.

## Checks
1. **Build** passes with no warnings you cannot explain.
2. **Links:** every internal link and #anchor resolves. External links return 200.
3. **Content:** one h1 per page, meaningful alt text on every image, no lorem ipsum, no placeholder prices.
4. **Mobile:** at 375px width there is no horizontal scroll, tap targets are at least 44px, and text is at least 16px.
5. **Forms:** each form submits, shows a confirmation and stores or sends the data. It has a consent checkbox and a link to the privacy policy. Test the spam trap.
6. **Contact paths:** phone, WhatsApp and email links open the right app with the right number.
7. **SEO:**
   - title and description on every page;
   - canonical URL;
   - sitemap.xml;
   - a robots.txt that does not block the site;
   - no noindex on pages that should rank.
8. **Analytics:**
   - the tag fires once per page view;
   - key events (form, WhatsApp click) arrive;
   - cookie consent is shown where required.
9. **Legal (Israel):** accessibility statement (הצהרת נגישות), privacy policy, and terms if selling.
10. **Security:**
    - HTTPS with redirect;
    - HSTS, X-Content-Type-Options and a Content-Security-Policy;
    - no secrets in client code;
    - server version hidden.
11. **Speed:**
    - images in modern formats with width and height;
    - fonts preloaded or swapped;
    - Largest Contentful Paint under 2.5 s on mobile.

## Report
A table with check, status (pass / fail / needs human), evidence (command output or URL) and fix. Failures first.

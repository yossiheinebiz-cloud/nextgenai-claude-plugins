---
name: page-seo-geo
description: Write SEO and GEO metadata for website pages or blog posts. Covers search keywords, a title under 60 characters, a 120 to 160 character meta description, and a short FAQ that answer engines (ChatGPT, Gemini, Google AI Overviews) can quote. Use when the user asks for SEO, meta tags, keywords, descriptions, GEO, structured data, or to make pages show up in ChatGPT answers.
---

# Page SEO and GEO

Work page by page. Read each page's real content before writing anything for it.

## For each page produce
- **keywords:** 6 to 10 phrases a real searcher types or asks, main topic first. Mix the local language (natural questions, e.g. "כמה עולה בוט וואטסאפ לעסק") with the English product terms people search. No single generic words.
- **seoTitle:** max 60 characters, main keyword near the start, brand at the end only if it fits.
- **description:** 120 to 160 characters, includes the main keyword, says what the visitor gets. Unique per page.
- **faq:** 3 to 4 questions phrased the way people ask them. Answers are 1 to 3 sentences with the direct answer first. Facts must match the page exactly (prices, terms, process). Skip if the page already has a FAQ.

## Where it goes
Detect the stack and put the data where it belongs: frontmatter (Astro, MDX, Hugo), a per-route metadata export (Next.js), or a central map keyed by path. Emit:
- `<title>`, `<meta name="description">`, Open Graph and Twitter tags, canonical URL.
- JSON-LD: Article for posts, Service or LocalBusiness for business pages, BreadcrumbList, and FAQPage only when the FAQ is visible on the page.
- An `/llms.txt` that lists the main pages with one line each, if the site has none.

## GEO: what answer engines quote
- Put a one or two sentence direct answer at the top of each page ("התשובה הקצרה").
- Use question headings that match how people ask.
- State concrete facts: price ranges, time frames, who it is for, with a date when facts change.
- Keep entity names consistent (brand, product, person) across pages and in Organization schema with `sameAs` links.

## Rules
- Never invent prices, reviews, ratings, clients or statistics. Do not add AggregateRating without real reviews.
- No keyword stuffing. The description is written for a person.
- FAQ schema must match visible text.
- Finish with a check: list pages missing a description, descriptions outside 70 to 170 characters, and duplicate titles or descriptions.

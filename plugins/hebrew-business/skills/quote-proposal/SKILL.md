---
name: quote-proposal
description: Write a price quote or project proposal in Hebrew (הצעת מחיר) for an Israeli small business or freelancer. Use when the user asks for הצעת מחיר, proposal, quote, or to turn notes from a client call into an offer.
---

# Hebrew price quote / proposal

Produce a clear, client-ready הצעת מחיר in Hebrew, right-to-left, in the user's business voice.

## Gather first (ask only what is missing)
- Business name, עוסק מורשה / חברה, contact line.
- Client name and the problem in their words.
- Scope: what is included, what is not.
- Price model: fixed price, per hour, or per milestone. Currency ₪.
- Whether prices include VAT (מע״מ). Never assume the rate; ask, or write "בתוספת מע״מ כחוק".
- Timeline and payment terms (שוטף + X, advance payment).
- Validity of the offer (default: 14 days).

## Structure
1. כותרת: הצעת מחיר ל[לקוח]: [פרויקט], date, offer number.
2. הבעיה והמטרה: 2 to 3 sentences in the client's language.
3. מה כלול: numbered deliverables, each one testable.
4. מה לא כלול: explicit list. This prevents scope disputes.
5. לוח זמנים: milestones with dates or weeks.
6. מחיר: a table (item, quantity, price, total), subtotal, VAT line, total.
7. תנאי תשלום ותוקף ההצעה.
8. הצעד הבא: one clear action (approve by reply, sign, pay advance).

## Rules
- Numbers and prices stay left-to-right inside Hebrew text: write "3,000 ₪" and never put a Hebrew word directly after "25+".
- No em dash or en dash. Use commas or periods.
- Plain Hebrew, no hype words (מהפכני, חדשני ביותר). Short sentences.
- Never invent prices, discounts, client names or past results. If the user gave none, leave a clearly marked placeholder like [מחיר].
- Output as Markdown ready to paste, or as .docx if a document skill is available and the user asks.

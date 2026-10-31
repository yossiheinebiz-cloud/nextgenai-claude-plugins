---
name: receipt-finder
description: Find receipts and invoices (קבלות, חשבוניות) in Gmail for a period. Lists vendor, date, amount and VAT, and can save attachments to a Google Drive folder for the accountant. Use when the user asks to find receipts, invoices or expenses, or to prepare documents for the bookkeeper (רואה חשבון, הנהלת חשבונות).
---

# Receipt and invoice finder

Read-only in Gmail. Write to Drive only after the user confirms the folder.

## Steps
1. Ask for the period if not given (default: last calendar month).
2. Search Gmail with several queries and merge the results, for example:
   - `has:attachment (קבלה OR חשבונית OR "חשבונית מס" OR receipt OR invoice) after:YYYY/MM/DD before:YYYY/MM/DD`
   - `from:(billing OR invoice OR receipts OR noreply) (receipt OR invoice) after:YYYY/MM/DD before:YYYY/MM/DD`
   - Known vendors the user names (Google, Meta, Wix, a supplier).
3. For each message record:
   - vendor and date;
   - amount and currency, plus VAT if shown;
   - document number;
   - whether a PDF is attached;
   - a link to the email.

   Read amounts from the email subject and body. Many Gmail connectors see only attachment names and sizes, not their contents: if the amount is only inside the PDF and you cannot open it, write "לא זוהה" and keep the link, never guess.
4. Remove duplicates: messages with the same vendor, amount and date count once. A receipt and an invoice for the same payment are one row; note both documents.
5. Output a table sorted by date, totals per currency, and a list of payments that seem to have no document.
6. Offer a CSV or spreadsheet for the bookkeeper. If your tools can copy attachments to Google Drive, offer to save them to a folder named `קבלות YYYY-MM` (confirm first). Otherwise give the list of email links so the user can forward them in one pass.

## Rules
- Never forward emails or send anything to the accountant yourself.
- This collects documents and is not tax advice. Say so if the user asks what is deductible.

---
name: daily-briefing
description: Morning briefing from Google Calendar and Gmail. Covers today's meetings, tasks hidden in emails, and threads waiting for a reply. Use when the user asks what is on today, for a daily summary (סיכום יומי), or to plan the day. Needs Google Calendar and Gmail tools (connectors or MCP servers).
---

# Daily briefing

Read-only. Never send, archive, delete, label or accept anything unless the user explicitly asks in this session.

## Steps
1. Check which tools exist (Google Calendar, Gmail). If one is missing, say so and continue with what you have.
2. **Calendar:** today's events in the user's time zone (default Asia/Jerusalem). For each event give time, title, attendees, location or link, and any prep needed (a doc to read, a question to answer).
3. **Gmail, the last 24 hours plus anything unread from the last 3 days:**
   - Tasks: requests addressed to the user ("can you", "תוכל", "נא לשלוח", deadlines, dates).
   - Waiting on the user: threads where the last message is from someone else and asks something.
   - Money: invoices, payment requests, failed payments.
   - Skip newsletters, promotions and automated notifications unless they contain a deadline.
4. **Write the briefing** in the user's language (Hebrew if they write Hebrew):
   - שורה תחתונה: the 1 to 3 things that matter most today.
   - פגישות היום (table).
   - משימות מהמיילים: each with sender, what is asked, due date and a link to the thread.
   - ממתינים לתשובה שלך.
   - כסף ותשלומים.
5. Offer drafts for up to 3 replies. Drafts only. The user sends.

## Run it every morning
In Claude Code, ask for a scheduled routine or recurring task that runs `/daily-assistant:daily-briefing` at 07:30 on workdays (Sunday to Thursday in Israel). In the Claude app, use a scheduled task with the same instruction if your plan has it.

## Privacy
- Quote only what is needed. Do not copy full email bodies into the briefing.
- Leave out one-time codes, passwords, and full card or ID numbers. If you see them, mention only that a security email arrived.

# Chaser: unpaid invoice tracker for freelancers

**Problem:** A freelance graphic designer needs to track unpaid invoices across several clients, while their spreadsheet keeps slipping out of date.

## Problem analysis

| Pain point | Root cause | How Chaser solves it |
|---|---|---|
| Spreadsheet goes stale | Status ("overdue", "due soon") is typed by hand | Status is calculated from the due date every time the page opens |
| Hard to see who owes what | Rows are mixed across clients | "Owed by client" list, sorted by amount |
| Unclear what to chase first | No sense of how late each invoice is | Aging bar plus invoices sorted by due date |
| Chasing is awkward and slow | Writing reminders from scratch | One click copies a polite reminder with the right numbers |
| Updating feels like a chore | Many columns to maintain | Adding an invoice takes 5 fields, due date is auto-filled from terms |

## Features

- Add invoices with client, number, amount, issue date and payment terms
- Auto status: not due, due soon, overdue (with days late), paid
- Totals: outstanding, overdue, due in 7 days, paid in last 30 days
- Aging bar (not due, 1 to 30, 31 to 60, over 60 days late)
- Filters: unpaid, overdue, paid, all
- Mark paid, undo, delete
- Copy a ready-to-send reminder message
- Export to CSV, multiple currencies, sample data
- Works offline, data saved in the browser (localStorage), light and dark mode

## Run locally

Open `index.html` in a browser. There is no build step.

## Deploy

Static site, deploy on Vercel with the default settings (Framework Preset: Other, no build command).

## Limitations and next steps

Data lives in one browser only. Possible upgrades: a database (Supabase) with login, recurring invoices, email reminders.

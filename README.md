# ChipSync — Lead & Quotation CRM

A lead-management and quotation dashboard built for a Dubai IT/electronics
retail client. Tracks leads through their pipeline (new → quoted → ordered →
closed), a customer book with order history and lifetime value, and a
quotation builder that generates numbered quotes per lead.

**Live demo:** enable GitHub Pages on this repo, or open `index.html` directly.
Demo login: `demo` / `demo1234` (all data is fictional — no real client data).

## Stack — intentionally no build step

This is React and Babel loaded straight from a CDN, with in-browser JSX
transpilation (`<script type="text/babel">`), rather than a bundled
Vite/webpack project. That was a deliberate choice for a single-page internal
tool with no deployment pipeline of its own: open `index.html` and it runs,
no `npm install`, no build. State persists to the browser's `localStorage` —
there is no backend.

Two versions exist in this repo:
- `index.html` — the full CRM (leads, customers, quotations, login).
- `ChipSync Dashboard.html` / `tweaks-panel.jsx` — an earlier lead-management-
  only iteration.

## What it does

- **Leads pipeline** — status tracking (New / Quoted / In Progress / Ordered /
  Closed / Lost), assignment to sales reps, follow-up dates, source tracking.
- **Quotations** — generates a numbered, printable quote per lead.
- **Customer book** — aggregates order history and lifetime value per company.
- **Role-based login** — Admin / Sales / Manager views.

## Notes

- The account list and sample leads in this repo are fictional demo data.
- No API keys, tokens, or real credentials are stored anywhere in this repo.

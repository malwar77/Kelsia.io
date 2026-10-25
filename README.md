# Kelsia

This is a **static demo website for GitHub Pages**. It is **NOT the full Kelsia app**.

## What it is

A single, self-contained `index.html` (inline CSS/JS, no build step, no external
dependencies) that shows what Kelsia looks like: Dashboard, Super Agent, Agents,
Tasks, Social, Outreach, Ads, Finance, Memory, Artifacts, Approvals,
Integrations, and Settings — in the original order.

## What it is NOT

- It has **no backend, no database, and no login**. Anything that looks like
  data is demo/seed data in the page itself, or saved only in the visitor's
  own browser (demo chat, demo artifacts, demo approval state).
- **Nothing posts, sends, or charges from here.** All 10 integrations
  (Twitter/X, SendGrid + IMAP, Tavily, Google Ads, Meta Ads, PayPal, GitHub,
  Telegram, WhatsApp Cloud API, Ollama) are shown as **Not connected**.
- It never asks for API keys, secrets, tokens, or passwords. Real connections
  belong in the full self-hosted Kelsia app or a secure connection flow —
  never in this demo page or in chat.
- Finance shows `$0` / `—` only, with "Last snapshot: none yet". No PayPal
- PayPal is the owner's normal personal receiving account; entries are manual, with no automatic PayPal sync.
  figures are invented. The evening summary is a placeholder, not an invented
  summary. There are no ads, no analytics, no tracking, and no fake
  testimonials or numbers.

## How to publish it (GitHub Pages)

1. Put `index.html` and this `README.md` in the repository (for example, the
   root of the `Kelsia.io` repo).
2. In the repo: Settings → Pages → Build and deployment → Source: Deploy from
   a branch → Branch: `main`, Folder: `/ (root)` → Save.
3. Wait for GitHub Pages to publish, then open the Pages URL and check that
   every tab renders.

## For real Kelsia

Real execution — with approval-first mode, so agents queue actions for approval
before anything posts, sends, or charges — requires the full self-hosted
Kelsia app (FastAPI + Next.js + Postgres/Redis/Celery) or the private Muse
app. This static site is a demo and a placeholder for that, not a replacement.

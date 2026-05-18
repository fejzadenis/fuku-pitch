# bets.fuku.ag — Execution Roadmap (Pitch Site)

A single-page presentation site you can deploy to Vercel in under 60 seconds.

## What's in here

```
fuku-pitch/
├── index.html       # The entire pitch — self-contained, no build step
├── vercel.json      # Vercel config (clean URLs, security headers)
└── README.md        # This file
```

No build tools. No dependencies. No framework. Just an HTML file with embedded CSS and minimal JS.

## Deploy to Vercel — three options

### Option 1 — Drag and drop (no CLI)

1. Go to https://vercel.com/new
2. Drag the entire `fuku-pitch` folder into the import area
3. Click **Deploy**
4. You'll get a URL like `fuku-pitch-xxxx.vercel.app` in ~15 seconds

### Option 2 — Vercel CLI

```bash
npm i -g vercel
cd fuku-pitch
vercel --prod
```

Answer the prompts (link to your account, accept defaults). Done.

### Option 3 — GitHub → Vercel

1. Create a new GitHub repo, push this folder to it
2. In Vercel dashboard: New Project → Import from GitHub
3. Select the repo → Deploy

Subsequent commits auto-deploy.

## Custom domain

In Vercel project settings → Domains → add `pitch.fuku.ag` (or whatever subdomain you want) and point a CNAME at Vercel. Live in ~2 minutes.

## Editing

Open `index.html` in any editor. All content is inline. All styles are in the `<style>` block at the top. The countdown timer updates automatically from JavaScript — change the kickoff date at the bottom of the file if needed.

## Tech notes

- **Fonts:** Loaded from Google Fonts CDN — Boldonse (display), Fraunces (serif italics), JetBrains Mono (body/data), Shippori Mincho B1 (Japanese characters)
- **Aesthetic:** Trading-terminal × Japanese-fortune-scroll. Black background, fortune red `#e84a3f`, cream foreground `#f0ead6`
- **Responsive:** Mobile breakpoint at 900px
- **No tracking, no analytics** — add Plausible or PostHog if you want stats

## What this document represents

A condensed, presentable version of the full 60-day execution roadmap. It's designed to be skimmed in 5 minutes by busy stakeholders, or read carefully in 15. The full unabridged roadmap lives in `bets-fuku-roadmap.md` (separate document).

— 福 —

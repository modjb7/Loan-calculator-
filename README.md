# Loan Calculator | கடன் கணிப்பான்

Bilingual (English/Tamil) loan calculator — Flat Rate or Reducing Balance,
forward mode (find monthly payment) or reverse mode (find interest rate from
a known payment). Auto-redirects to slglitz.blogspot.com 10 seconds after
showing results.

## Deploy on GitHub Pages

1. Create a new GitHub repo.
2. Upload `index.html` and `og-image.png` to it.
3. Settings → Pages → Source: Deploy from a branch → `main` / root. Save.
4. Your live URL appears after ~1 minute:
   `https://YOUR-USERNAME.github.io/YOUR-REPO/`

## One edit needed for the shareable photo to show

Open `index.html`, find these two lines near the top:

```html
<meta property="og:image" content="https://YOUR-USERNAME.github.io/YOUR-REPO/og-image.png" />
<meta property="og:url" content="https://YOUR-USERNAME.github.io/YOUR-REPO/" />
```

Replace `YOUR-USERNAME` and `YOUR-REPO` with your real GitHub Pages URL, then
commit and push. This is what makes WhatsApp (and other apps) show the
picture/title card when someone shares your link. If WhatsApp shows a stale
preview while testing, share the link once with `?v=2` appended to force a
refresh.

## What changed in this version

- **Months field fixed**: entering 12 or more months now automatically
  rolls the extra into years (e.g. 15 months → 1 year 3 months) instead of
  going out of range. Negative values are clamped to 0.
- **Shareable preview photo added**: `og-image.png` is the card WhatsApp
  (and Facebook, Telegram, etc.) will show when your link is shared.

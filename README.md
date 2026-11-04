# JekApps

Source for [jekapps.com](https://jekapps.com): a single-page about site for Jacob Fullerton, covering
[TrackYourCash](https://cash.jekapps.com), [1Poker](https://1poker.app) and a prediction-market trading
system, plus a web version of the résumé.

It is plain static HTML and CSS with no build step and no third-party requests.

| File | Purpose |
|---|---|
| `index.html` | The page: intro, projects, résumé, contact |
| `styles.css` | Styles, including dark mode and a print stylesheet that turns the page into a clean résumé |
| `favicon.svg` | Site icon |

## Preview locally

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Deploy

Any static host works: publish the repository root as-is (Cloudflare Pages with no build command and output
directory `/`, GitHub Pages from `main` / root, or similar), then point `jekapps.com` at it.

## Keeping it public-safe

This repository is public. Keep personal contact details (phone, home address, personal email) and details of
the trading system's venues and strategy out of every file, commit message and history.

# Senora Asset Management — Website

A clean, responsive marketing site for Senora Asset Management — an India-centric,
pure large-cap focused, long-only fund (SEBI-registered CAT III AIF), powered by the
proprietary **StaG Framework**.

## Stack
- Static HTML / CSS / vanilla JS — no build step
- Light & teal design system
- Responsive, with mobile navigation and scroll reveals

## Files
| File | Purpose |
|------|---------|
| `index.html` | Page structure & content |
| `styles.css` | Theme and layout |
| `script.js` | Mobile nav, smooth scroll, form feedback |
| `vercel.json` | Hosting config + security headers (HSTS, etc.) |

## Run locally
Open `index.html` in a browser, or serve it:

```bash
npx serve .
```

## Deploy
Hosted on Vercel — HTTPS is automatic. Every push to `main` triggers a deploy.

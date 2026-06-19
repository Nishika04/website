# DNS Setup for senoraamc.com → Vercel

Hi! We've deployed the Senora Asset Management website on Vercel. To make it live on
our domain **senoraamc.com**, two DNS records need to be added in the Squarespace account
that manages the domain. This is the only step remaining — it takes about 2 minutes.

## Steps in Squarespace

1. Log in to **Squarespace**.
2. Go to **Settings → Domains** and select **senoraamc.com**.
3. Open **DNS Settings** (also called "DNS" or "Custom Records").
4. Add the following **two records**:

| Type    | Host (Name) | Value / Data            |
|---------|-------------|-------------------------|
| `A`     | `@`         | `76.76.21.21`           |
| `CNAME` | `www`       | `cname.vercel-dns.com`  |

   - The **A record** points the main domain (`senoraamc.com`) to Vercel.
   - The **CNAME record** points `www.senoraamc.com` to Vercel.
   - If Squarespace won't accept `@` for the Host, leave the Host field **blank** — it means the same thing.

5. **Save**.

## What happens next

- Vercel automatically detects the records, verifies the domain, and issues a free
  SSL certificate (HTTPS) — usually within a few minutes.
- Full DNS propagation can take up to an hour.
- Once done, **https://www.senoraamc.com** will show the website, secured with HTTPS.

## Notes

- Please do **not** change the domain's nameservers — only add the two records above.
- If there are any existing conflicting `A` records on `@` or a `CNAME` on `www`,
  those may need to be removed/updated. Happy to help if anything looks unclear.

Thank you!

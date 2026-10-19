# River and Palace Website

Static coming-soon website for **River and Palace**, the iOS **Chinese Chess / Xiangqi** game.

This interim site is designed for GitHub Pages project hosting at:

```text
https://mint5auce.github.io/river-and-palace-website/
```

The custom domain is intentionally not configured yet. Do not add a `CNAME` file until `riverandpalace.com` DNS is ready.

## Local Preview

Open `index.html` directly, or run:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## TestFlight Privacy And Support

The TestFlight preparation includes privacy and support sections at `/#privacy` and `/#support`.
The owner approved the complete policy, operator/contact details, 12-month retention period, and publication on 19 October 2026.
The support mailbox passed a receive/reply test on the same date.
No public TestFlight link, signup form, tracking, or email subscription is included.
The app links to `https://riverandpalace.com/#privacy` and `https://riverandpalace.com/#support`.
Publish approved changes through the existing GitHub Pages workflow.

## Publishing

Publish from the `main` branch at the repository root using GitHub Pages.

When the custom domain is ready, add `CNAME` with `riverandpalace.com`, configure the Pages custom domain, update DNS for the apex and `www`, and enable HTTPS only after GitHub reports the certificate is ready.

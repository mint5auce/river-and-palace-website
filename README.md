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

## Future TestFlight Privacy Note

When adding a public TestFlight link, also add a short privacy notice explaining
that beta distribution is through Apple TestFlight and any TestFlight
feedback/crash information shared with River and Palace is used only to improve
the app.

## Publishing

Publish from the `main` branch at the repository root using GitHub Pages.

When the custom domain is ready, add `CNAME` with `riverandpalace.com`, configure the Pages custom domain, update DNS for the apex and `www`, and enable HTTPS only after GitHub reports the certificate is ready.

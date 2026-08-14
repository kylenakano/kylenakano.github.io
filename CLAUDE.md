# kylenakano.github.io

Personal site at **kylenakano.com** (apex + www). Static — hand-written `index.html` + `css/style.css`, no build step, no dependencies. Edit and push; that's the whole workflow.

## Deploy

GitHub Pages serves `main` directly. Push to deploy. `CNAME` holds the custom domain — **don't delete or rewrite it**; losing it drops the domain binding.

## Non-negotiables

- **No build tooling.** If a change seems to want npm/Vite/a generator, it doesn't belong here — this repo is deliberately three files.
- Migrated off GCP App Engine 2026-08-07. If the TLS cert ever fails to issue, the fix is to unset and re-set the custom domain in Pages settings (that's what worked).
- `nas.kylenakano.com` and `photos.kylenakano.com` are **live QuickConnect forwards**, unrelated to this repo. Don't touch those DNS records while editing here.

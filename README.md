# Annum Shahid — Portfolio

Personal portfolio site for **Annum Shahid**, Growth-Focused Digital Marketing Head (Lahore, Pakistan).

Single-file static site — no build step, no framework.

## Structure

```
index.html        entire site (markup, styles, scripts)
assets/           photo, video, certificates, JS libraries
```

- `annum-hero.jpg`, `annum-avatar.jpg` — professional headshot
- `annum-video.mp4` — video portfolio
- `cert-*.jpg` — certifications (Google Ads, GA4, Meta, Semrush, Klaviyo, Socially Devoted)
- `three.min.js`, `gsap.min.js`, `ScrollTrigger.min.js`, `logo-paths.js` — vendored locally so the
  site has no runtime CDN dependency

## Local preview

```bash
npx serve -l 4180 .
```

Or just open `index.html` in a browser.

## Deployment

Hosted on Vercel, connected to this GitHub repository.
Every push to `main` triggers an automatic redeploy — no manual step.

## Editing

All content lives in `index.html`:

| What | Where to look |
|---|---|
| Roles / timeline | `const ROLES` |
| Skills cards | `const SKILLS` |
| Toolbox chips | `const TOOLBOX` |
| Certification badges | `const CERTS` |
| Certificate carousel | `const CERT_IMGS` |
| Colours | `:root` custom properties |

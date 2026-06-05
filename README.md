# GZ-Diplomacy Support Form

Static GitHub Pages bug-report form for GZ-Diplomacy.

## Files

- `index.html` — public report form
- `thank-you.html` — redirect page after submission
- `.nojekyll` — keeps GitHub Pages from trying to process the site with Jekyll

## Email provider

This version uses FormSubmit:

```html
<form action="https://formsubmit.co/factoriolegion+diplomacy@gmail.com" method="POST">
```

The first real submission will trigger a confirmation email to:

```text
factoriolegion+diplomacy@gmail.com
```

Open that email and confirm the address. After that, reports should go to the inbox.

## Before publishing

In `index.html`, replace this placeholder:

```html
<input type="hidden" name="_next" value="https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPOSITORY/thank-you.html" />
```

with the actual GitHub Pages URL after you know it.

Example:

```html
<input type="hidden" name="_next" value="https://GIZMOD.github.io/gz-diplomacy-support/thank-you.html" />
```

## GitHub Pages setup

1. Create a public GitHub repository, for example `gz-diplomacy-support`.
2. Upload `index.html`, `thank-you.html`, `.nojekyll`, and this `README.md`.
3. Go to repository Settings → Pages.
4. Deploy from branch.
5. Select `main` and `/root`.
6. Save.
7. Open the generated GitHub Pages URL.
8. Submit one test report.
9. Confirm the activation email from FormSubmit.

## Mod portal link text

Suggested link text:

```text
GZ-Diplomacy bug report form:
https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPOSITORY/
```

Suggested note:

```text
For crashes/desyncs, include factorio-current.log and the relevant files from Factorio/script-output/GIZMOD_logs/.
```

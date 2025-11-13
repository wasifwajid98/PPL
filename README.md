# Paint Party Lab — Product Selection (Static Web App)

This is a small static web app (single `index.html`) that implements the Paint Party Lab product selection and QR/payment view provided by the user.

Usage

- Open the file directly in a browser: double-click `/workspaces/PPL/index.html` or use your editor's preview.
- Or serve with a simple static server (recommended) and open `http://localhost:8000`:

```bash
# from the repository root
python3 -m http.server 8000

# then open http://localhost:8000/index.html in your browser
```

Notes

- Images used in the page are loaded from external URLs (the user's provided links).
- The page is purely client-side; the `Save edits` button sends a postMessage to `window.parent` (no server integration included).

If you want, I can add a small Node/Express server, bundle assets, or add persistent saving of edits. Which would you like next?

Publishing to GitHub Pages

- This repository can be published to GitHub Pages using the included GitHub Actions workflow. When you push to the `main` branch, the workflow will upload the repository contents and publish them.
- Expected Pages URL (after a successful deployment): `https://wasifwajid98.github.io/PPL/` — the site may take a minute to appear after the workflow completes.

How to publish

1. Commit and push your changes to GitHub:

```bash
cd /workspaces/PPL
git add .
git commit -m "Add site and GitHub Pages workflow"
git push origin main
```

2. Open the repository's Actions tab on GitHub and confirm the `Deploy to GitHub Pages` workflow ran successfully.
3. Visit `https://wasifwajid98.github.io/PPL/` (or the Pages URL shown in your repo settings) to view the live app.

If you want, I can also:
- Set up a custom domain (CNAME) and add HTTPS configuration.
- Use a deploy preview (Netlify/Vercel) instead for faster previews.

# PPL
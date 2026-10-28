# Happy Birthday Darla

A small birthday surprise built as a single static page. Dark theme, small hearts floating across the screen, a birthday wish, and then two questions, "Do you love me?" and "Will you marry me?", each with a Yes button and a No button that runs away.

No build step and no dependencies. It is one file: `index.html`.

## Put it online with GitHub Pages

1. Create a new repository on GitHub, for example `darla-birthday`.
2. Upload `index.html`, `README.md` and `.nojekyll` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then save.
5. Wait about a minute. The site will be live at `https://<your-username>.github.io/darla-birthday/`.

Send that link to Darla.

If you prefer the command line:

```bash
git init -b main
git add .
git commit -m "Birthday page for Darla"
git remote add origin https://github.com/<your-username>/darla-birthday.git
git push -u origin main
```

## Make it yours

Everything you may want to change is in `index.html`:

- **Her name:** `HER_NAME` near the top of the `<script>` block.
- **The wish and the final message:** the text inside the two `<main>` sections.
- **The lines the No button says:** the `lines` array in the script.
- **Colors:** the variables at the top of the `<style>` block.

To test locally, open `index.html` in a browser. Add `#ask` or `#marry` to the address to jump straight to a question page.

## Notes

- Fonts load from Google Fonts, so the page needs an internet connection to look its best. It still works without them, using the fallback fonts.
- The page respects the "reduce motion" setting on phones and computers.

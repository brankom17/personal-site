# Personal Site

A single-page personal website — plain HTML, CSS, and JS. No build step.
Clean minimal layout with a dark default and a light/dark toggle.

## Edit your content

Everything you need to change is in **`index.html`**, marked with
`<!-- ====== EDIT ... ====== -->` comments:

- **Name, tagline, bio** — in the hero section
- **Experience** — duplicate a `<li class="timeline__item">` block per role
- **Contact links** — update the GitHub / LinkedIn `USERNAME` and email
- **Résumé** — drop your PDF at `assets/resume.pdf`

The **Projects** section is commented out near the middle of `index.html`.
Delete the comment wrapper (`<!-- ... -->`) to turn it on when you're ready.

Colors and styling live in **`styles.css`** under the theme tokens at the top.

## Preview locally

Just open `index.html` in a browser, or run a tiny local server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a repo. For a personal site at `https://<username>.github.io`,
   name the repo exactly `<username>.github.io`. Any other name works too and
   the site will live at `https://<username>.github.io/<repo>/`.
2. Push these files to the `main` branch.
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from
   a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait ~1 minute, then visit your URL.

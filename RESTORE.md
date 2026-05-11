# Bringing Tiwa's portfolio back online

The full portfolio is preserved in this repo as `portfolio.html` (+ `styles.css`,
`images/`, `website-content.md`). Right now the live site only shows the
"coming soon" page (`index.html`).

To go live again:

```bash
rm .vercelignore
rm index.html
git mv portfolio.html index.html
git add -A && git commit -m "chore: relaunch portfolio"
vercel deploy --prod --yes      # from this directory
```

Then open a PR (via the Trueflutter fork) so the GitHub repo stays in sync.

The original "coming soon" page lives in git history on the `feature/under-construction`
branch if it's ever wanted again.

# The Blue Goose Memorial

A static Jekyll/GitHub Pages memorial for **James Ervin “Snowie” Zittel** and the **U.S.S. Honolulu (CL-48)**.

## Publish on GitHub Pages

1. Create a new GitHub repository and upload every file in this folder to the repository root.
2. In **Settings → Pages**, set **Source** to **GitHub Actions**.
3. Push to the `main` branch. The included workflow builds and deploys the site.
4. For a project repository such as `username.github.io/blue-goose`, no manual `baseurl` is needed because the workflow supplies it during the build.

## Preview locally

```bash
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Most important edits

- `_data/site.yml` — Snowie’s biography, verified ship details, and contact email.
- `_crew/james-ervin-snowie-zittel.md` — Snowie’s full profile.
- `_data/timeline.yml` — ship and family timeline events.
- `_data/gallery.yml` — gallery captions and categories.
- `_accounts/` — one Markdown file per personal account.
- `_crew/` — one Markdown file per sailor.

## Original database warning

The old Angular/Express project loaded crew, battles, awards, ship data, and personal accounts from MongoDB. Those database records were not present in the uploaded ZIP, so this package includes a complete static structure plus starter content. Export any surviving MongoDB data before retiring the old system.

The original route files also contained database credentials. Revoke or rotate those credentials and purge them from public Git history before reusing the old repository.

## Image credits and historical sourcing

The included photographs came from the original project archive. Add a source/credit field to gallery entries whenever the original catalog information is known. Official starting points include the Naval History and Heritage Command’s ship history, action reports, war-damage reports, and photograph catalog.

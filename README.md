# xidist.xyz

Static portfolio page for Kidist Wosenyeleh / xidist.

## Local preview

```powershell
python -m http.server 4173
```

Open `http://localhost:4173`.

## Notion source

The `td projects` section is integrated from this public Notion gallery:

https://fortune-gallium-33b.notion.site/f53668f197054b88a9cc5be3441d987c

The latest integrated card is `new username xidist.xyz creating a site`, created May 17, 2026 at 4:53 PM.

## Publish on GitHub Pages at xidist.xyz

This repository is configured for GitHub Pages through `.github/workflows/pages.yml`.
Push to `main` to deploy. The `CNAME` file sets the custom domain to `xidist.xyz`.

## Notion automation

The Notion setup card notes that automated publishing needs these GitHub Actions repository secrets:

- `NOTION_TOKEN`
- One of `NOTION_DATA_SOURCE_ID` or `NOTION_DATABASE_ID`
# dummy

Static portfolio page for Kidist Wosenyeleh / xidist.

## Local preview

```powershell
python -m http.server 4173
```

Open `http://localhost:4173`.

## Publish on GitHub Pages at xidist.xyz

1. Create an empty GitHub repo named `dummy` under `xidist`.
2. Push this folder:

```powershell
git remote add origin https://github.com/xidist/dummy.git
git branch -M main
git push -u origin main
```

3. In GitHub, go to `Settings` -> `Pages` and set the source to `GitHub Actions`.
4. In Porkbun DNS, point the apex domain to GitHub Pages and make `www` a CNAME.

The included workflow deploys the static files from `main`. The `CNAME` file sets the custom domain to `xidist.xyz`.

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

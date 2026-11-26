# Lu Yang — GitHub Pages portfolio

This folder is a standalone, single-page static portfolio for `https://luisa106.github.io`.

It uses no build system or framework:

- `index.html` contains the complete profile, résumé sections and project previews.
- `profile.jpg` is the portrait shown in the left sidebar.
- `favicon.svg` is the site icon.
- `projects/*.html` are the two embedded interactive dashboards.

## Preview locally

From this folder, run:

```bash
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/`.

The server is optional for basic viewing, but it is recommended because it makes the relative dashboard paths behave the same as GitHub Pages.

## Publish to GitHub Pages

In a separate terminal, clone the GitHub Pages repository and copy this folder's contents into it:

```bash
git clone https://github.com/Luisa106/luisa106.github.io.git
cd luisa106.github.io
cp -R /Users/luisa/Documents/Work/Code_Projects/remix/github-pages/. .
git add .
git commit -m "Create Lu Yang portfolio"
git push origin main
```

On GitHub:

1. Open the `Luisa106/luisa106.github.io` repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Choose `main` and `/ (root)`, then click **Save**.

GitHub Pages should publish the site at:

- `https://luisa106.github.io/`

If the browser shows an old version after deployment, wait a minute and hard-refresh with `Cmd + Shift + R`.

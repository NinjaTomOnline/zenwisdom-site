# Zen Wisdom public site template

Recommended public repo name: `zenwisdom-site`

Public repo URL:

`https://github.com/NinjaTomOnline/zenwisdom-site`

This template is meant to be exported from the private Zen Wisdom app repo into a separate public GitHub repo for GitHub Pages hosting.

Expected GitHub Pages URL:

`https://ninjatomonline.github.io/zenwisdom-site/`

The source of truth lives in the private app repo under `Release/HostedPages/`.

## Refresh Flow

1. From the private app repo, run:

   ```bash
   ruby scripts/export_hosted_site.rb --force
   ```

2. Copy the exported bundle from `/tmp/zenwisdom-site` into the root of this public repo.
3. Push `main`.
4. GitHub Actions publishes the site automatically through Pages.

## Files Included

- `index.html`
- `support.html`
- `privacy.html`
- `terms.html`
- `404.html`
- `site.css`
- `robots.txt`
- `sitemap.xml`
- `site.webmanifest`
- `assets/`
- `screenshots/`
- `.github/workflows/publish-pages.yml`
- `.nojekyll`

## Custom Domain Later

If Zen Wisdom moves from GitHub Pages to a custom domain later, update these values in the private app repo first:

- `launch-config.yml`
- `AppStore/AppStore_Metadata_Package.md`
- `ZenWisdom2020/ZenWisdom2020/Resources/Config/app_config.json`

# ZK Games Website

Static website for ZK Games, including game download links and the privacy policy.

## GitHub Pages

This site is ready to publish from the repository root with GitHub Pages.

- Entry page: `index.html`
- Privacy policy: `privacy-policy.html`
- Not found page: `404.html`
- Stylesheet: `style.css`
- Images: `images/`
- Custom domain: `zkgamestudios.com`
- GitHub Pages support: `.nojekyll`, `CNAME`, `404.html`
- Hostinger support: `.htaccess`

## Custom Domain DNS

For GitHub Pages, the root domain must point only to GitHub Pages.

Use these `A` records for `zkgamestudios.com`:

```txt
A  @  185.199.108.153
A  @  185.199.109.153
A  @  185.199.110.153
A  @  185.199.111.153
```

Optional IPv6 records:

```txt
AAAA  @  2606:50c0:8000::153
AAAA  @  2606:50c0:8001::153
AAAA  @  2606:50c0:8002::153
AAAA  @  2606:50c0:8003::153
```

Use this for `www`:

```txt
CNAME  www  YOUR-GITHUB-USERNAME.github.io
```

Do not keep extra root `A`, `AAAA`, `ALIAS`, or `ANAME` records from another host when using GitHub Pages.

## HTTPS

After DNS is correct, open GitHub repository settings:

1. Go to `Settings` -> `Pages`.
2. Set the custom domain to `zkgamestudios.com`.
3. Wait for GitHub to finish the DNS/certificate check.
4. Enable `Enforce HTTPS`.

If certificate provisioning gets stuck, remove the custom domain in GitHub Pages settings, save, add `zkgamestudios.com` again, and save.

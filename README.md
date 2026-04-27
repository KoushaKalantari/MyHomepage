# Kousha Kalantari Personal Website

Static personal website for `www.koushakalantari.com`, designed to publish cleanly on GitHub Pages with no build step.

## Files

- `index.html` - homepage content, metadata, and structured data.
- `styles.css` - responsive visual design.
- `CNAME` - tells GitHub Pages to serve the site at `www.koushakalantari.com`.
- `.nojekyll` - keeps GitHub Pages from running Jekyll processing.

## Publish on GitHub Pages

1. Create a GitHub repository, for example `MyHomepage`.
2. Push these files to the repository's `main` branch.
3. In GitHub, open the repository settings.
4. Go to `Pages`.
5. Set the source to deploy from the `main` branch and `/root`.
6. Confirm the custom domain is `www.koushakalantari.com`.
7. Enable `Enforce HTTPS` after GitHub finishes provisioning the certificate.

## GoDaddy DNS

Keep the domain registered at GoDaddy. Update DNS so:

- `www` is a `CNAME` record pointing to your GitHub Pages host, usually `<your-github-username>.github.io`.
- The apex domain `koushakalantari.com` either redirects to `https://www.koushakalantari.com` or uses GitHub Pages apex records if you want GitHub to handle the redirect.

DNS updates often appear quickly, but can take up to 48 hours globally.

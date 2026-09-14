# Royal Power Mart Website

This repository is designed for the existing Cloudflare Worker `royal-power-mart`.

## Easiest file to edit

Open:

`public/config.js`

That is where normal business changes are made:
- phone numbers
- WhatsApp numbers
- email
- branch addresses
- Google Maps links
- brand list
- hero wording

The website design is in `public/style.css`. Normally you do not need to edit it.

## Cloudflare

The included `wrangler.jsonc` is already configured for the Worker named `royal-power-mart` and serves the files from `public/`.

For an existing Worker, connect this GitHub repository from:

Workers & Pages → royal-power-mart → Settings → Builds → Connect

After the first successful connection, future pushes to the configured branch can automatically build and deploy the website.
Website connected to Cloudflare.

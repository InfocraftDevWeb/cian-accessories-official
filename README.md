# Cian Accessories — public storefront and private product panel

The working storefront is `index.html` (same public catalog as `catalog.html`); `admin.html` is the separate management interface. They use the dedicated Supabase project described in `../README.md`. Deploy only the contents of this `web/` folder as a new isolated static site. The browser config contains only the public Supabase publishable key; never include `sb_secret_`, `service_role`, login credentials, bearer tokens, or private keys.

## Current publication state

Owner authorized the official public site and a free trial (2026-11-01). The storefront starts with an empty catalog and does not invent products, prices, stock or photographs. The verified public Instagram profile describes Cian Accessories C.A as accessories, clothing, shoes and perfumes in Puerto La Cruz, Calle Bolívar, Monday–Saturday 9:30 a.m.–6 p.m., with national shipping, RIF J-502004670. Public Facebook lists +58 412-879-6779; that opens the WhatsApp inquiry link. Confirm all operational details with the owner before relying on them. Map link is a search, not a verified pin. USD/VES amounts only appear after an administrator records current confirmed USD and complete dated rate/source/amount data. This site has no checkout or online payment.

`config.js` contains only the public publishable key for the isolated Supabase project. Admin visibility and writes are protected by Auth UID check and server-side RLS. Admin URL: `/admin.html`; public catalog: `/` or `/catalog.html`. Do not add product information without verifying exact details and approved images with the store.

The CSS loads DM Sans and Playfair Display from Google Fonts; system fonts remain as fallbacks. Images are absent from product listings until Cian approves exact product media. The supplied Cian logo was reused from the existing local proposal; confirm authorization to continue its official public use.

## Deployment

Publish this directory as an independent new repository/site only. Do not change any unrelated hosting project. Configure the host build directory to `web` (or upload its contents); no build command is needed. Configure routes so `/` serves `index.html` and preserve `/admin.html` and its assets. HTTPS required for Supabase Auth. Verify live anonymous empty catalog and test admin login on the exact deployed hostname, then test phone viewport. No Firebase billing or paid services are needed for this Supabase-backed static app. Hosting URLs and publication claims must be verified after deployment.
